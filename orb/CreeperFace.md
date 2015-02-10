# Creeper Face

**Wizard:** Umbris

**Source:** https://the-codespells-forum.herokuapp.com/t/creeper-face-for-the-minecraft-fans/164

![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/CreeperFace01.png)

## Orb Spell
![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/CreeperFace03.png)

### Compiled JS

```Javascript
function onCreate( orb ) {
   orb.setVelocity( 5 );
}

function onHit( orb, other ) {
   orb.destroySelf();
}
```

## Creeper Face Spell
![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/CreeperFace02.png)

### Eval

```Javascript
var dist = 0.3;
orb.transform.Translate(Vector3.left * 2.5 * dist);
orb.transform.Translate(Vector3.up * 2.5 * dist);
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 3 * dist); 
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);

orb.transform.Translate(Vector3.left * 5 * dist);
orb.transform.Translate(Vector3.down * 1 * dist);
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 3 * dist); 
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);

orb.transform.Translate(Vector3.down * 1 * dist);
orb.transform.Translate(Vector3.left * 3 * dist);
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);

orb.transform.Translate(Vector3.down * 1 * dist);
orb.transform.Translate(Vector3.left * 2 * dist);
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);

orb.transform.Translate(Vector3.down * 1 * dist);
orb.transform.Translate(Vector3.left * 3 * dist);
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 1 * dist); 
orb.createOrb("Orb",5);

orb.transform.Translate(Vector3.down * 1 * dist);
orb.transform.Translate(Vector3.left * 3 * dist);
orb.createOrb("Orb",5);
orb.transform.Translate(Vector3.right * 3 * dist); 
orb.createOrb("Orb",5);
```

### Compiled JS

```Javascript
function onActivate( orb ) {
   orb.destroySelf();
}

function onCreate( orb ) {
   orb.setVelocity( 0 );
   eval('
      var dist = 0.3;
      orb.transform.Translate(Vector3.left * 2.5 * dist);
      orb.transform.Translate(Vector3.up * 2.5 * dist);
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 3 * dist); 
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);

      orb.transform.Translate(Vector3.left * 5 * dist);
      orb.transform.Translate(Vector3.down * 1 * dist);
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 3 * dist); 
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);
      
      orb.transform.Translate(Vector3.down * 1 * dist);
      orb.transform.Translate(Vector3.left * 3 * dist);
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);
      
      orb.transform.Translate(Vector3.down * 1 * dist);
      orb.transform.Translate(Vector3.left * 2 * dist);
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);
      
      orb.transform.Translate(Vector3.down * 1 * dist);
      orb.transform.Translate(Vector3.left * 3 * dist);
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 1 * dist); 
      orb.createOrb("Orb",5);
      
      orb.transform.Translate(Vector3.down * 1 * dist);
      orb.transform.Translate(Vector3.left * 3 * dist);
      orb.createOrb("Orb",5);
      orb.transform.Translate(Vector3.right * 3 * dist); 
      orb.createOrb("Orb",5);
   ');
}
```
