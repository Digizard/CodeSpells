# Fireworks

**Wizard:** geniusidiot

**Source:** https://the-codespells-forum.herokuapp.com/t/fireworks-contest-entry/152

## Dud Spell
![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/Fireworks01.png)

### Compiled JS

```Javascript
function onCreate( orb ) {
   orb.setVelocity( 15 );
}
```

## Firework Spell
![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/Fireworks02.png)

### Compiled JS
```Javascript
function onCreate( orb ) {
   orb.setVelocity( 15 );
}

function onActivate( orb ) {
   for (var count = 0; count < 8; count++) {
      orb.createOrb( 'dud', 2 );
      orb.turnRight( 135 );
      orb.turnUp( 90 );
   }
}
```

## Fireworks Spell
![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/Fireworks03.png)

### Compiled JS

```Javascript
var boom;

function onCreate( orb ) {
   orb.setVelocity( 50 );
   orb.turnRight( 30 );
   boom = 1;
   
   if (boom < 6) {
      for (var count = 0; count < 3; count++) {
         orb.turnLeft( 15 );
         boom = boom + 1;
         orb.createOrb( 'firework', 30 );
      }
   }
}
```
