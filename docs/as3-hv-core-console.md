# as3.hv.core.console.*

-----------------------------------
*Simple command line console for debugging, logging and monitoring.*

-----------------------------------

## Description:

![Console](https://github.com/HerbertV/as3-hv/blob/master/images/console.png?raw=true)

The Consoles visibility can be toggled by default with ^ (220).
Type help to get a command list.

### Code Snippets:

	// adding console to stage
	var c:Console = Console.getInstance();
	addChild( c );

	// activates the time stamp for each message
	c.setShowTimeStamp(true);
	
	// remaps the toggle key to F1
	c.setToggleKey( Keyboard.F1 );

### Commands:
Here a list of the basic commands.

- help
- clr
- dlvl
- exit
- fps
- mem
- system
- time

### Class as3.hv.core.console.Console
TODO

### Class as3.hv.core.console.DebugLevel
TODO

### Interface as3.hv.core.console.cmd.IConsoleCommand
For defining your own commands.
