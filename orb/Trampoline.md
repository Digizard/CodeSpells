# Trampoline

**Wizard:** sertar

**Source:** https://the-codespells-forum.herokuapp.com/t/trampoline-spell/132

>> The code is pretty straightforward. When the main spell hits something, it creates four "pinWithDelay" spells in opposite directions. Each one moves a little then go up a little and stop.


![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/Trampoline01.png)
![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/Trampoline02.png)

## Pin With Delay Spell
![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/Trampoline04.png)

### Compiled JS

```Javascript
function upALittle() {
   orb.transform.rotation = Quaternion.LookRotation(Vector3.up, orb.transform.up);
   orb.setTimeout("stop2",1);
}

function stop2() {
   orb.setVelocity( 0 );
}

function onCreate( orb ) {
   orb.setVelocity( 15 );
}

function onActivate( orb ) {
   orb.destroySelf();
}

function onHit( orb, other ) {
   orb.createPhysicalConnection( other );
   orb.setTimeout("upALittle", 0.5);
}
```

## Trampoline Spell
![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/Trampoline03.png)

### Compiled JS

```Javascript
function onCreate( orb ) {
   orb.setVelocity( 15 );
}

function onHit( orb, other ) {
   if (other.rigidbody && !other.rigidbody.isKinematic) {
      for (var count = 0; count < 4; count++) {
         orb.turnLeft( 90 );
         orb.createOrb('pinWithDelay', 40);
      }
   }
}
```
