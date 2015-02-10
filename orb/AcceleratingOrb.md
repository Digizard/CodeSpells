# Accelerating Orb

**Wizard:** Umbris

**Source:** https://the-codespells-forum.herokuapp.com/t/accelerating-orb-aka-eval-works/125

>> Cast this and the orb begins slowly, but picks up speed. This shows that you can use the eval block to write your own code, even to manipulate pre-built objects like "orb."

![Screenshot](https://raw.githubusercontent.com/SittingFox/CodeSpells/master/orb/images/AcceleratingOrb.png)

# Eval Code

```Javascript
orb.setVelocity(speed);
```

# Compiled JS

```Javascript
var speed;

function Accelerate() {
   speed = speed + 1;
   eval('orb.setVelocity(speed);');
}

function onCreate( orb ) {
   speed = 1;
   orb.setInterval("Accelerate", 0.1);
}

function onActivate( orb ) {
   orb.destroySelf();
}

function onHit ( orb, other ) {
   orb.destroySelf();
}
```
