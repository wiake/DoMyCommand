# DoMyCommand

DoMyCommand is a GUI front end to store and re-use your favourite bash, sh, or dash commandlines. It can be used, for example, as an enhanced Premote replacement to control commandline clients such as rdesktop (Remote Desktop Client to MS Windows desktops using rdp protocol), vnc, secure shell (ssh), wget and curl, or to convert or record media files using your favourite ffmpeg command pipe sequencies. The creative user could also add commands to provide outputs via yad, gtkdialog, or similar.
_____

Changes in version 9.0.3: hijack addon modules now use .hijack as their extension.

'hijack' expansion capability (as per DoMyFile, Precord etc) expanded to allow modular plugin addition of new main code, new functions, new gui panels and new gui general config buttons, More details on that simple facility, which can be used, for example, for modularly adding a new panel to the foot of the GUI can be found here:

http://www.murga-linux.com/puppy/viewtopic.php?p=656913#656913
_____

DoMyCommand depends only on bash and gtkdialog for basic functionality. For some commandlines it will of course require any underlying commandline utility you wish to use to be installed (e.g. rdesktop for rdp, openssh-client for ssh client, ffmpeg for media conversions etc). Some of the provided combobox commandlines depend on Xdialog, xterm or rxvt, or sometimes the system text editor for outputs.

On pressing the 'play' button, DoMyCommand operates just as if the displayed command was typed into a console window and the 'Enter key pressed', but it brings the following advantages of a GUI environment:

* A dropdown list of pre-saved commands, which can be edited (modified, deleted, or appended to) in your system default text editor by pressing the Edit button on the righthand side of the dropdown list.

* New commands can thus be entered and permanently saved for re-use.

* Entry boxes (variables), which can, for example be used, for remote Computer URL address (A), remote login User name (U), remote login Password (P), and local Target Directory (TD). Note, however, that what you use the entry boxes to store is actually entirely up to you for the particular commandline you wish to run. The dropdown command can refer to these using standard bash shell syntax (i.e. $A, $U, $P, $TD).

* Entry data can be input manually, or via drag and drop, or cut and paste from your system filemanager.

* DoMyCommand also provides brief tool-tip text over most elements of its GUI, which becomes visible when the mouse is hovered over each element.

* Pretty much any bash commandline including quote marks and \ can be entered.

----

Commandline Usage

In a console enter command: domycommand --help
for brief commandline usage.
----

Tips:

To keep domycommand as the top window,
right-click on its window bar, and select Layer -> Above

In addition to outputting command results to a controlling xterm or rxvt terminal or to an Xdialog window, it is also possible to pipe command outputs to the 'leafpad' editor.

Alternatively, if you start domycommand from a terminal you can redirect its command output to that terminal using the syntax >/dev/tty 
