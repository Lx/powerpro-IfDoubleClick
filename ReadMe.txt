¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
IfDoubleClick
¯¯¯¯¯¯¯¯¯¯¯¯¯
Version 2.0
Wednesday, 10 September 2003
________________________________________________________________________

What?
¯¯¯¯¯
The IfDoubleClick script enables you to add double-click functionality
to bar buttons, system tray icons, hotkeys, or any other event that you
have defined in your PowerPro configuration. This allows you to give
your bar buttons etc. twice as much functionality than without it.

You can also use the IfDoubleClick script to have certain bar buttons
etc. ignore any accidental double-clicks, which may be handy if you find
yourself often launching two copies of a command by accident.

The IfDoubleClick script can also enable certain bar buttons etc. to
only respond to double-clicks.
________________________________________________________________________

Requirements
¯¯¯¯¯¯¯¯¯¯¯¯
The ‘Use quote ' for escape in expression strings’ checkbox, found under
Setup > Advanced Setup > Characters, must be ticked for the script to
work. This option is not ticked by default.

This script also uses the Events plugin (included with PowerPro).
________________________________________________________________________

Installation
¯¯¯¯¯¯¯¯¯¯¯¯
Extract the IfDoubleClick.txt file, into your Scripts folder (generally
C:\Program Files\PowerPro\Scripts).
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

The default time for the double-click timeout can be modified if you
prefer a faster or slower timeout. This is done by modifying the line in
the script itself, that defines the DblClickTimeout variable.
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
v2.0 (10/9/2003)
* Script:
  * Complete rewrite
  * Added accidental double-click detection
  * Global variables are no longer created or modified
* Explanatory message box:
  * Entered complete usage information
* Documentation:
  * Removed my Little Story :-)
  * Added requirement note regarding option in Advanced Setup

v1.1 (20/8/2003)
* Explanatory message box:
  * Added title
  * Corrected typo

v1.0 (19/8/2003)
* Initial Release
________________________________________________________________________