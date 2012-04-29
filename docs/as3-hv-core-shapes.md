# as3.hv.core.shapes.*

-----------------------------------
*Contains drawing helper Classes for different shapes*

-----------------------------------
## Class as3.hv.shapes.DebugShapes

### Description:


### Class Overview:


#### Static functions:

-	drawDebugCross(
				g:Graphics,
				x:Number, 
				y:Number,
				thickness:Number=1.0,
				color:uint=0xFF0000,
				alpha:Number=1.0
			):void


-----------------------------------
## Class as3.hv.shapes.EdgedRectangle

### Description:
![Edged Rectangle Sample](https://github.com/HerbertV/as3-hv/blob/master/images/EdgeRectangle.png)

### Class Overview:


#### Static functions:

-	drawGraphics(
				g:Graphics,
				x:Number,
				y:Number,
				w:Number,
				h:Number,
				insets:Array,
				lThickness:Number,
				lColor:uint,
				lAlpha:Number,
				filled:Boolean=false,
				fColor:uint=0x000000,
				fAlpha:Number=1.0
			):void


-----------------------------------
## Class as3.hv.shapes.PenroseTriangle

### Description:
![Penrose Triangle Sample](https://github.com/HerbertV/as3-hv/blob/master/images/Penrosetriangle.png)


### Class Overview:


#### Static functions:

-	drawGraphics(
				g:Graphics,
				center:Point, 
				len:Number,
				lThickness:Number,
				lColor:uint,
				lAlpha:Number,
				filled:Boolean,
				fColors:Array,
				fAlphas:Array
			):void
-	drawSingleSegment(
				g:Graphics,
				center:Point, 
				len:Number,
				lThickness:Number,
				lColor:uint,
				lAlpha:Number,
				filled:Boolean,
				fColor:uint,
				fAlpha:Number,
				angle:uint
			):void
- 	drawTriangle(
				g:Graphics, 
				center:Point, 
				len:Number
			):void