¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
IfDoubleClick
¯¯¯¯¯¯¯¯¯¯¯¯¯
Version 2.2
Tuesday, 5 October 2004
________________________________________________________________________

What?
¯¯¯¯¯
The IfDoubleClick script enables you to add double-click functionality
to bar buttons, system tray icons, hotkeys, or any other event that you
have defined in your PowerPro configuration. This allows you to give
your bar buttons etc. twice as much functionality than without it.

For example, you could set up the Win+C key combination to be able to
launch either Calculator, or the Command Prompt. (Please refer to the
Usage section if you're interested.)

You can also use the IfDoubleClick script to have certain bar buttons
etc. ignore any accidental double-clicks, which may be handy if you find
yourself often launching two copies of a command by accident.

The IfDoubleClick script can also enable certain bar buttons etc. to
only respond to double-clicks.
________________________________________________________________________

Requirements
¯¯¯¯¯¯¯¯¯¯¯¯
This script uses features found only in PowerPro versions v4.1 and
above.
________________________________________________________________________

Installation
¯¯¯¯¯¯¯¯¯¯¯¯
Extract IfDoubleClick.PowerPro to your Scripts folder, e.g.:
C:\Program Files\PowerPro\Scripts\ColourSpy.PowerPro
________________________________________________________________________

Usage
¯¯¯¯¯
.IfDoubleClick(OnDoubleClick, OnSingleClick, DblClickTimeout)

OnDoubleClick and OnSingleClick are PowerPro commands to run when double
and single clicks are detected, respectively.

Specify both a double- and single-click command to give your bar button,
tray icon, hotkey etc. different functionality depending on whether it
is executed once or twice in a given timeframe (as specified by the
optional DblClickTimeout argument, or 500 milliseconds by default).

Specify only a double- and no single-click command for your bar button
etc. to only respond to double clicks.

Specify only a single- and no double-click command for your bar button
etc. to perform that command, and then ignore any accidental double-
click that follows (technically, any second click within DblClickTimeout
of the first click, or 500 milliseconds by default).

For example, to set up the Win+C key combination to be able to launch
either Calculator or the Command Prompt, you could assign this command
to the key combination in your Key/Mouse settings:

.IfDoubleClick("Cmd", "Calc")

Then, after saving your configuration, you will be able to use the Win+C
combination to launch Calculator, and Win+CC to launch the Command
Prompt. (This is actually a combination I use!)

The default time for the double-click timeout can be modified if you
prefer a faster or slower timeout and don't wish to explicitly specify
it each time. This is done by modifying the line that defines the
DblClickTimeout variable in the script.
________________________________________________________________________

To Conclude
¯¯¯¯¯¯¯¯¯¯¯
I'd really like to know if you need any help with this script, or if it
grows on you, so please feel free to Email me with any questions or
comments that you may have. My Email address can be found through the
Yahoo! PowerPro group, at:

> http://groups.yahoo.com/group/power-pro/

...or you can just leave a message at the Group — there's a good chance
that I'll see it just as quickly.

Lastly, a special thanks to Bruce Switzer for giving us a lifetime with
PowerPro! :-)

Best regards,
Alex Peters
________________________________________________________________________

Version History
¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
v2.2 (5/10/2004)
*  The script no longer conforms to Standard Configuration and should
   now function without modification on any PowerPro v4.1 configuration

v2.1 (21/9/2003)
*  Script:
   *  The script no longer references its filename, so the script file
      can now be renamed without problems
   *  Small optimisation to the way the event is killed
*  Documentation:
   *  Added Win+C and Win+CC examples

v2.0 (10/9/2003)
*  Script:
   *  Complete rewrite
   *  Added accidental double-click detection
   *  Global variables are no longer created or modified
*  Explanatory message box:
   *  Entered complete usage information
*  Documentation:
   *  Removed my Little Story :-)
   *  Added requirement note regarding option in Advanced Setup

v1.1 (20/8/2003)
*  Explanatory message box:
   *  Added title
   *  Corrected typo

v1.0 (19/8/2003)
*  Initial release
________________________________________________________________________