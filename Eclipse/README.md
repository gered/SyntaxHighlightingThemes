# Eclipse Pre-configured Theme & Syntax Coloring Settings

This is an initial Eclipse workspace configuration and plugin that apply a
dark style UI theme and editor syntax coloring.

A very slightly modified copy of the 
[Dark Juno](http://rogerdudler.github.io/eclipse-ui-themes/) theme plugin by 
Roger Dudler is used. Only a couple of colors have been changed.

Syntax color settings are present for Java, Clojure, Javascript, CSS, HTML 
and XML.

Language plugins used:

* [Counterclockwise](https://code.google.com/p/counterclockwise/) (Clojure)
* Eclipse Web Developer Tools (HTML, CSS, XHTML)
* JavaScript Development Tools

## Usage

**This has only been tested with fresh Eclipse Juno installations. Attempts to 
use with an existing installation are done at your own risk!**

Extract Eclipse, as per a normal installation of Eclipse. Before running it
for the first time, do the following:

* Copy the contents of the ```eclipse_root/dropins``` folder to the ```dropins``` folder located in the root of your Eclipse installation.
* Copy the ```your_workspace/.metadata``` folder to the folder you will be using as your workspace in this Eclipse installation.
* Run Eclipse, choosing the same workspace folder that we set up with the existing ```.metadata``` in the previous step.

If this was completed successfully, you should immediately notice Eclipse is
using the Dark Juno theme.

* Now install the plugins listed above (if needed). The existing snytax color settings we copied over should be picked up by them.

## Known Issues

* The Dark Juno theme is unfortunately not perfect due to limitations in the CSS styling support in Eclipse. Specifically, certain SWT controls like scrollbars and table/grid headers cannot be styled and will render as per the OS's default styling.
* There is a somewhat annoying 2px gray/white border line at the top of some tabs / editing windows. This ***can*** be styled, but there doesn't appear to be a unique CSS class/id for it, making it difficult to style without affecting something else in the process.
* The text on the Perspective switching toolbar is unfortunately too dark. I can't seem to style this any better ???
* Some text on the bottom status line (e.g. the column/line indicator) doesn't seem to stick to the color style applied to it. There might be some way to get around this. ??
* Minimized tabs/windows appear in an ugly off-color box.
* Probably a ton of stuff I don't use at all in Eclipse isn't styled consistently. Oh well.
