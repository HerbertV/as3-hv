# as3.hv.core.console.*

-----------------------------------
*Simple command line console for debugging, logging and monitoring.*

-----------------------------------

## Description:

![Console](https://github.com/HerbertV/as3-hv/blob/master/images/console.png?raw=true)

The Consoles visibility can be toggled by default with F1.
Type help to get a command list.

### Code Snippets:

	// adding console to stage
	var c:Console = Console.getInstance();
	addChild( c );

	// activates the time stamp for each message
	c.setShowTimeStamp(true);
	
	// remaps the toggle key to F2
	c.setToggleKey( Keyboard.F2 );

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

### Interface as3.hv.core.console.cmd.IAutoCompleteable
For defining your commands that support auto completion.