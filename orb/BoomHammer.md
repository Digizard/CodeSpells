# Boom Hammer

**Wizard:** geniusidiot

**Source:** https://the-codespells-forum.herokuapp.com/t/boom-hammer-contest-entry/149

>> what it does is it creates a push shield 11 feet/meters in front of you.
it has no real purpose other than creating a small amount of push spells but I just thought it would look bossome jumping up, casting the spell, and slamming the spell in to the ground when you land, at least through the mind's eye.

![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/BoomHammer.png)

## Compiled JS

```Javascript
function onCreate( orb ) {
   orb.setVelocity( 5 );
   orb.lockToPlayerRotation(9999);
}

function onHit ( orb, other ) {
   orb.createOrb( 'Push Shield', 40 );
}
```
