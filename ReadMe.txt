¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
IfDoubleClick
¯¯¯¯¯¯¯¯¯¯¯¯¯
Version 1.0
Tuesday, 19 August 2003
________________________________________________________________________

What?
¯¯¯¯¯
The IfDoubleClick script enables you to add double-click functionality
to bar buttons, system tray icons, key combinations, or any other event
that you have defined in your PowerPro configuration.

After receiving an event, it waits a certain amount of time for the same
event. One of two actions are then executed depending on the outcome.
________________________________________________________________________

A Little Story
¯¯¯¯¯¯¯¯¯¯¯¯¯¯
My PowerPro configuration includes a couple system tray icons, one of
these being a sort of PowerPro ‘control’ icon. The left and right mouse
buttons each display a menu, while the middle mouse button launches the
PowerPro Configuration editor.

The problem with this, is that I find left double-clicking a lot easier
than clicking the ‘middle’ mouse button (which is actually situated on
the side of my Logitech MouseMan), and so, failing to find a double-
click feature native to PowerPro, I scripted one myself. :-)
________________________________________________________________________

Requirements
¯¯¯¯¯¯¯¯¯¯¯¯
This script uses the Events plugin (included with PowerPro), which is
limited to 50 simultaneous events. So your PowerPro configuration must
use less than 50 simultaneous events. :-)
________________________________________________________________________

Installation
¯¯¯¯¯¯¯¯¯¯¯¯
Extract the IfDoubleClick.txt file, included with this archive, into
your Scripts folder.
________________________________________________________________________

Usage
¯¯¯¯¯
The command usage, with optional parameters in [square brackets], is:
.IfDoubleClick(OnDoubleClick[, OnSingleClick][, DblClickTimeout])

OnDoublelick and OnSingleClick are PowerPro commands to run when double-
and single-clicks are detected, respectively. OnSingleClick is an
optional parameter.

The optional DblClickTimeout parameter specifies a time in milliseconds
to wait for a second click, before assuming a single-click. The default
wait is 500 milliseconds, which can be changed by editing the
IfDoubleClick script.
________________________________________________________________________

To Conclude
¯¯¯¯¯¯¯¯¯¯¯
I'd really like to know if this script grows on you, so please feel free
to Email me with any questions or comments you may have. You can reach
me through the Yahoo! PowerPro group, at:

> http://groups.yahoo.com/group/power-pro/

Lastly, a special thanks to Bruce Switzer for making life on the
computer enjoyable again! :-)

Best regards,
Alex Peters
________________________________________________________________________

Version History
¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
v1.0 (19/8/2003)
* Initial Release
________________________________________________________________________
