open-budget-frontend
====================

Install on OS X
---------------

###Install Brew

First make sure you have npm installed, if not install it according to the instructions here: http://brew.sh/

###Install NPM

    $ npm install
    
###Install the project

Checkout the project from ```https://github.com/OpenBudget/open-budget-frontend/``` and then go into the open-budget directory and run these in the command line:

    $ npm install
    $ npm install -g bower
    $ bower update
    $ npm install -g grunt-cli
    $ patch -p0 < ./bootstrap-rtl.less.patch
    $ grunt
    $ grunt serve
 

Install on Windows
------------------
(tested on Windows XP SP3)

###Install git

If you don't already have git installed, get it at: http://git-scm.com/download/win

###Install node.js (includes npm)

Get the Windows installer from: http://nodejs.org/download/

###Fix up npm

(This section handles a known issue with npm, see https://github.com/npm/npm/issues/6106)

Open Git Bash. run:

    $ npm

If you get an error that looks like:

    ENOENT, stat '<some directory>\npm'

Then run this command:

    $ mkdir "%APPDATA%\npm"

###Install the project

Same instructions as under OS X above.

Enjoy!
