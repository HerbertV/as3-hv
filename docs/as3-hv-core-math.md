# as3.hv.core.math.*

-----------------------------------
## Class as3.hv.math.TrueRandom

### Description:
A class for solving the basic problems with random Numbers in as3.
Including a seeded generator based on:

[Lehmer random number generator](http://en.wikipedia.org/wiki/Lehmer_random_number_generator) 


### Class Overview:
For detailed info see the comments inside the class file.


#### Static functions:

- trunc(
				num:Number, 
				percision:uint
			):Number
- generateRangedInt(
				min:int, 
				max:int=-1
			):int
- generateRandomSignedMultiplier():int

#### Constructor:

 * TrueRandom(
				isSeeded:Boolean=false,
				cacheSizeOrSeed:uint=10
			)

#### Public functions:

- setupGenerator(
				generator:Function,
				min:Number,
				max:Number
			):void
- fillUpCache(e:Event):void
- nextCachedNumber():Number
- getInitialSeed():uint
- nextSeededInt():uint
- nextSeededNumber(
				percision:uint=0
			):Number
- nextRangedSeededInt(
				min:int, 
				max:int=-1
			):uint
- nextRangedSeededNumber(
				min:Number, 
				max:Number,
				percision:uint=0
			):Number

### Examples:
See the CS3_TrueRandomExample.fla how it works.

Or use the snippets below:

	import as3.hv.core.math.TrueRandom;

Example for seeded random generator setup:

	var trSeeded:TrueRandom = new TrueRandom(
			true,	// true = seeded
			1		// seed
		);

Example for non-seeded random generator setup:

	var trNonSeeded:TrueRandom = new TrueRandom(
			false,	// false = non-seeded
			20		// cache size
		);
	
	trNonSeeded.setupGenerator(
			TrueRandom.generateRangedInt, // callback
			1, // from
			10 // to
		);

	// now add event listener to stage to fill our cache
	this.addEventListener(
			Event.ENTER_FRAME, 
			trNonSeeded.fillUpCache 
		);

Example to access a generated number:
	
	// ranged seeded number (float) from 1-10
	trSeeded.nextRangedSeededNumber(1,10);
	
	// generates as defined above unsigned int from 1-10
	trNonSeeded.nextCachedNumber()

	// Direct access without cache
	TrueRandom.generateRangedInt(1,10);

