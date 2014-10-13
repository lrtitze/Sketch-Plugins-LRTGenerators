# LRTGenerator Sketch Plugins

For various projects there was a need to create Sketch 3 plugin scripts which could generate object collections. I'll share them with you here since they could be useful or serve as examples for solving your own problems.

**WARNING:** I'm trying to track down a bug that causes Sketch to crash after the second or third time these scripts are run with block counts higher than 50. Be very careful and make sure that you save all of your work before trying to use these with high block counts.

This bug may be related to an [issue currently under investigation](https://github.com/ccgus/CocoaScript/issues/8) in the CocoaScript Github repository.

## Script #1 - Random Colored Box Grid

This command creates a square group of boxes whose colors are randomly selected from three preset colors. The colors, number of squares per side and the size of the squares can be set by modifying the script.

```
// Set the number of blocks on a side and their size.
var blockCount = 30;
var blockSize = 10;

// Default colors
var darkColor  = [MSColor colorWithRed:0.2 green:0.0 blue:0.0 alpha:1.0];
var midColor   = [MSColor colorWithRed:0.5 green:0.1 blue:0.1 alpha:1.0];
var lightColor = [MSColor colorWithRed:1.0 green:0.0 blue:0.0 alpha:1.0];
```

As provided, the script generates this group of objects:

![](http://lrtitze.github.io/Sketch-Plugins-LRTGenerators/images/RandomNoiseBox.png)


## Script #2 - Random Colored Bitmap Grid

This command creates the same pattern as #1 but inserts a single image bitmap to Sketch instead of a group of shape objects.

This could be a starting point for anyone who wants to draw into an NSImage and place the result into the Sketch document. The idea for this drawing method came from looking at the *NSImage Draw Buttons* example in the [CocoaScript GitHub repository](https://github.com/ccgus/CocoaScript).

```
// Set the number of blocks on a side and their size.
var blockCount = 30;
var blockSize = 10;

// Default colors
var darkColor  = [NSColor colorWithRed:0.0 green:1.0 blue:0.0 alpha:1.0];
var midColor   = [NSColor colorWithRed:0.1 green:0.5 blue:0.1 alpha:1.0];
var lightColor = [NSColor colorWithRed:0.0 green:0.2 blue:0.0 alpha:1.0];
```

As provided, the script generates this bitmap:

![](http://lrtitze.github.io/Sketch-Plugins-LRTGenerators/images/RandomNoiseBitmap.png)

---

### More to come

I have a few more similar plugins to add soon.

When there's extra time I'll add a UI for setup (or leave it as an exercise for the reader.)

### Contact
On App.net or Twitter I can be found at: lrtitze
