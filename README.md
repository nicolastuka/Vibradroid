# Vibradroid
Haxe Extension for vibrate Android mobiles devices.

# Installation

· haxelib install vibradroid

### Example Use Extension (Vibration during x milliseconds):

```haxe

import extension.vibradroid.Vibradroid;

class SimpleExample
{
    function AnyFuntion():Void
    {
        Vibradroid.Vibrate(500); //milliseconds
    }
}
```

### Example Use Extension (Vibration indefinitely non cancelable):

```haxe

import extension.vibradroid.Vibradroid;

class ExampleIndefinitely
{
    function AnyFuntion():Void
    {
        Vibradroid.VibrateIndefinitely();
    }
}

```

### Example Use Extension (Vibration with patterns):

```haxe

import extension.vibradroid.Vibradroid;

class ExamplePatterns
{
    function AnyFuntion():Void
    {
        var pattern:Array<Int> = new Array<Int>();
        pattern.push(1000);
        pattern.push(500);
        pattern.push(1000);
        pattern.push(300);
        pattern.push(1000);
        pattern.push(100);
        pattern.push(1000);
        pattern.push(10);
        pattern.push(1000);
        pattern.push(1000);
        pattern.push(500);
        pattern.push(2000);
        Vibradroid.VibratePatterns(pattern);
    }
}

```

### License

The MIT License (MIT) - LICENSE.md

Copyright © 2019 MilköGames (http://www.milkogames.xyz)

Author: Nicolás Capel
