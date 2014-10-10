# LRTGenerator Sketch Plugins

For various projects there was a need to create Sketch 3 plugin scripts which could generate object collections. I'll share them with you here since they could be useful or serve as examples for solving your own problems.

## Random Colored Box Grid

![](http://lrtitze.github.io/Sketch-Plugins-LRTGenerators/images/RandomNoiseBox.png)

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


### More still to come

I have a few more of these that will be added soon.

### Contact
On App.net or Twitter I can be found at: lrtitze
