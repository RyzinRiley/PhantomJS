Please see also: https://phantomjs.org/releases.html

2016-01-23: Version 2.1.0

    New features

      * Upgraded Qt to 5.5.1 (issue #13377)
      * Added support for SSL Client Authentication (issue #11275)
      * Added support for context menu event (issue #11429)
      * Allow remote debugging to use random port assigned by the OS (issue #13432)

    Improvements

      * Allow outer context to access arbitrary URLs (issue #11217)
      * Fixed --local-storage-path and localStoragePath config option (issue #11596)
      * Restored --local-url-access=no regression (issue #13412)
      * Fixed an issue with loading JS modules contains a last-line comment (issue #12868)
      * Fixed an issue with returning binary content in WebServer module (issue #13026)
      * Fixed encoded URL loading on Windows (issue #12953)
      * Fixed building with GCC 5 (issue #13518)
      * Fixed file upload (issue #12506)
      * Fixed latest OS detection (issue #13829)

2015-01-23: Version 2.0.0

    New features

      * Switched to Qt 5 and updated WebKit (issue 10448)
      * Implemented clearing of memory cache (issue 10357)
      * Added support for HTTP header change for every request (issue 11299)

    Improvements

      * Fixed rendering of CJK text by always linking the codecs (issue 10249)
      * Ensured onResourceReceived is still fired on an error (issue 11163)
      * Fixed possible crash in handling network requests (issue 11252)
      * Removed hardcoded GhostDriver launching message (issue 12681)
      * Allowed disk cache more than 2 GB (issue 12303)

    Examples

      * Netsniff example should exit when fails to load (issue 11333)

2014-01-25: Version 1.9.7

      * Reverted to GhostDriver 1.1.0 instead of 1.1.1 (issue 11915)
      * Fixed another warning of obsolete userSpaceScaleFactor on OS X 10.9 (issue 11612)

2014-01-20: Version 1.9.6

      * Updated GhostDriver to version 1.1.1 (issue 11877, 11893)

2014-01-19: Version 1.9.3

      * Fixed CoreText performance note on OS X 10.9 (issue 11418)
      * Fixed warning of obsolete userSpaceScaleFactor on OS X 10.9 (issue 11612)

2013-09-06: Version 1.9.2

      * Fixed graphical artifacts with transparent background on Windows (issue 11276, 11007, 11366)
      * Updated GhostDriver to version 1.0.4 (issue 11452)

2013-06-04: Version 1.9.1

    Critical bug fixes:

      * Fixed problems with specifying proxy server (issue 10811, 11117)
      * Fixed UTF-8 encoding with system.stdout and system.stderr (issue 11162)
      * Ensured that onResourceReceived will be always invoked (issue 11163)
      * Fixed module loading from an absolute path on Windows (issue 11165)
      * Fixed typo in the command-line option for setting the cache size (11219)
      * Fixed possible crash when handling network requests (issue 11252, 11338)

2013-03-20: Version 1.9.0 "Sakura"

    New features

      * Added spawn and execFile to execute external programs (issue 10219)
      * Added the ability to abort network requests (issue 10230)
      * Added system access to stdin, stdout, and stderr (issue 10333)
      * Added support for custom CA certificates location (issue 10916)
      * Added seek function to the File stream (issue 10937)
      * Implemented file read for a specified number of bytes (issue 10938)
      * Added a callback to handle network error (issue 10954, 10997)
      * Added custom encoding support when opening a page (issue 11043)
      * Implemented require.stub() support for a factory function (issue 11044)
      * Added page loading indicator and progress (issue 11091)
      * Added a timeout option for network requests (issue 11129)

    Improvements

      * Fixed the build on FreeBSD (issue 10597)
      * Ensured a consistent 72 dpi for Linux headless rendering (issue 10659)
      * Fixed possible PDF error due to invalid CreationDate field (issue 10663)
      * Fixed crash when uploading non existing files (issue 10941)
      * Improved the autocomplete internal of the interactive/REPL mode (issue 10943)
      * Fixed possible crash when accessing inline frames (issue 10947)
      * Changed Linux binary package setup to be built on CentOS 5 (issue 10963)
      * Extended SSL ignore setting to synchronous XHR (issue 10985)
      * Added convenient constants for modifier keys (issue 11056)
      * Fixed incorrect date handling in the cookies (issue 11068)
      * Updated GhostDriver to version 1.0.3 (issue 11146)

    Examples

      * Fixed invalid data URI in the netsniff example (issue 10740)
      * Implemented a new weather example (issue 10794)
      * Fixed rendering issues in render_multi_url (issue 11021)
      * Fixed proper event sequence in page_events example (issue 11028)
      * Miscellanous tweaks (issue 11082)

2013-03-02: Version 1.8.2

    Critical bug fixes:

      * Fixed possible PDF error due to invalid CreationDate field (issue 663)
      * Fixed crash when uploading non existing files (issue 941)
      * Fixed possible crash when accessing inline frames (issue 947)
      * Extended SSL ignore setting to synchronous XHR (issue 985)
      * Fixed incorrect date handling in the cookies (issue 1068)

2013-01-06: Version 1.8.1

    Critical bug fix:

      * Mac OS X: Fix possible crash when using some TrueType fonts (issue 690)

2012-12-21: Version 1.8.0 "Blue Winter Rose"

    New features

      * Integrated GhostDriver as the WebDriver implementation (issue 49)
      * Added an option to specify the SSL protocol (issue 174)
      * Added encoding support for WebServer's response (issue 505)
      * Added process ID (PID) to the System module (issue 769)
      * Added properties to obtain page and frame title (issue 799)
      * Added page navigation methods (issue 808)
      * Added support for modifier keys in keyboard events (issue 835)
      * Added onFilePicker callback for more generic file upload API (issue 843)
      * Added the ability to set the page content and location (issue 909)

    Improvements

      * Fixed date parsing in ISO8601 format (issue 187, 267)
      * Fixed window.location (issue 530, 632)
      * Deregistered multiple callback handler (issue 807)
      * Fixed sending of double-click events (issue 848)
      * Increases maximum number of redirects (issue 849)
      * Fixed keycodes sent for lowercase characters (issue 852)
      * Fixed a regression in table row page break (issue 880)
      * Completed the CoffeeScript version of the examples (issue 907)
      * Updated Qt to version 4.8.4 (issue 918)
      * Fixed potential hang in some example scripts (issue 922)

2012-09-22: Version 1.7.0 "Blazing Star"

    New features

      * Added a module system modelled after CommonJS/Node.js (issue 47)
      * Added support for window pop-up (issue 151)
      * Static build on Linux (issue 413)
      * Added run-time detection of SSL support (issue 484)
      * Added more events support (issue 492, 712)
      * Added support for disabling automatic proxy detection (issue 580)
      * Provided page closing callback (issue 678)
      * Added methods to access URL, frames URL, frame Content (issue 758)
      * Added more cookies-related API (issue 761)

    Improvements

      * Refactored command-line options handling (issue 55)
      * Improved the workflow for producing release builds (issue 599)
      * Improved cookies API and implementation (issue 603, 761)
      * Improved frame switching API (issue 654)
      * Fixed iframe handling regression (issue 683)
      * Fixed OS version number with Windows 8 and Mountain Lion (issue 684, 688)
      * Fixed HAR navigation info in the netsniff example (issue 733)
      * Fixed compile warnings with Visual Studio (issue 744)
      * Removed hacks for static linking on Windows (issue 753)
      * Added ICO image handling on Windows (issue 779)
      * Fixed font antialiasing on Windows (issue 785)
      * Improved Jasmine test runner for Jasmine 1.2 (issue 792)

2012-07-22: Version 1.6.1

    Bug fixes

      * Don't build the deploy in debug mode (issue 599)
      * Fixed building on Windows (issue 424)
      * Fixed remote inspector when building statically (issue 430)

2012-06-20: Version 1.6.0 "Lavender"

    New features

      * Added support for passing arguments to WebPage's evaluate (issue 132)
      * Added callbacks for JavaScript onConfirm and onPrompt (issue 133)
      * Added stack trace when error occurs (issue 166)
      * Added support for local storage path and quota (issue 300)
      * Added initial support for cookies handling (issue 354)
      * Added support for header footer when printing the page (issue 410, 512)
      * Added headers support in the loading request (issue 452)
      * Added support to render the web page as base64-encoded string (issue 547)
      * Added hooks for navigation event (issue 562)
      * Added command-line option to show debug messages (issue 575)
      * Added support for the zoom factor for web page rendering (issue 579)
      * Added crash reporter for Mac OS X and Linux, based on Google Breakpad (issue 576)
      * Added 'os' object to the system module (issue 585)
      * Added support for asynchronous evaluation (issue 593)

    Improvements

      * Fixed remote debugging to work on Mac OS X and Windows (issue 430)
      * Fixed web server getting the dropped connection for empty response (issue 451)
      * Fixed text rendered as boxes (squares) on headless Linux (issue 460)
      * Updated Qt to version 4.8.2 (issue 495)
      * Updated CoffeeScript compiler to version 1.3.3 (issue 496)
      * Fixed the build script to detect and use MAKEFLAGS (issue 503)
      * Fixed the build script to properly pass Qt config flags (issue 507)
      * Changed Info.plist to be embedded in Mac OS X executable (issue 528)
      * Fixed wrong module require in the imagebin example (issue 536)
      * Fixed example scripts to exit with the right exit code (issue 544)
      * Fixed build failure with glib 2.31.0+ (issue 559)
      * Fixed error handler failures in some cases (issue 589)
      * Fixed Twitter-related examples to work with the new site (issue 609)

2012-03-20: Version 1.5.0 "Ghost Flower"

    New features

      * Added interactive mode, also known as REPL (issue 252)
      * Added setting for web security, to allow cross domain XHR (issue 28)
      * Added error handler for WebPage object (issue 166)
      * Added support for custom HTTP header in the network request (issue 77)
      * Added support for read write encoding in the file system module (issue 367)
      * Added remote debugging support on Linux (issue 6)
      * Added support for proxy authentication (issue 105)
      * Added System module, to retrieve environment variables (issue 271) and arguments (issue 276)
      * Added fs.readLink function (issue 329)
      * Added support for reading and writing binary data (issue 400)
      * Added support to retrieve request data in the WebServer? module (issue 340)
      * Added support for individual top/bottom/left/right print margins (issue 388)
      * Added command-line option --help (issue 347)
      * Added short command-line options -v and -h (issue 408)
      * Removed support for Flash and other plugins (issue 418)

    Bug fixes

      * Fixed multiple console.log arguments (issue 36)
      * Fixed file upload (issue 307)
      * Fixed the web server instance to be asynchronous (issue 326) and still support Keep Alive (issue 416)
      * Workaround Qt 4.8.0 crash due to empty URL scheme (issue 365)
      * Fixed a Content-Type problem where POST does not work (issue 337)
      * Fixed reading body request in the web server even without specific Content-Type (issue 439)
      * Fixed Jasmine test runner with Jasmine 1.1 (issue 402)
      * Fixed request URL formatting in the web server (issue 437)
      * Don't display debugging and warning messages (issue 323)

2011-12-31: Version 1.4.1

    Bug fixes

      * Fix setting the proxy type (issue 266)
      * Workaround for file upload regression (issue 307)
      * Fix extraneous messsages in non-debug mode (issue 323)

2011-12-22: Version 1.4.0 "Glory of the Snow"

    New features

      * Added embedded HTTP server (issue 115)
      * Added convenient build script for Linux (issue 197)
      * Added support for SOCKS5 proxy (issue 266)
      * Updated CoffeeScript compiler to version 1.2 (issue 312)

    Bug fixes

      * Fix potential crash in QUrl with Qt 4.8 (issue 304)
      * Fix bug in CookieJar with QSettings and string (PyPhantomJS issue 10)
      * Prevent showing the icon on Mac OS X Dock (issue 281)

    Examples

      * Added a new example to detect browsers sniffing (issue 263)
      * Added HTTP server example (issue 115)

2011-09-23: Version 1.3.0 "Water Lily"

    Bug fixes

      * Fixed open() and POST method, without specifying the finished handler
      * Fixed script execution warning dialog (issue 165)
      * Added WebPage.release() to free the web page from memory (issue 154)
      * Added special handling of about:blank (issue 235)
      * Made a separate network access manager for each page (issue 190)

    New features

      * Introduced file system API based on CommonJS Filesystem proposal (issue 129)
      * Added support for persistent cookies (issue 91)
      * Added event handling, currently only for mouse events (issue 234)
      * Added page scroll position (issue 162)
      * Added HTTP authentication support (issue 45)
      * Added callback for page initialization (issue 143)
      * Added support to specify script and output encoding (issue 186)
      * Added option to allow local content to do cross-domain access (issue 28)
      * Added support to apply configurations from a JSON file (issue 180)
      * Added a convenient WebPage initialization construction (issue 206)
      * Added option to limit the size of disk cache (issue 220)

    Examples

      * Added a new example on using Modernizr to detect features (issue 144)
      * Fixed pizza.js example to use Mobile Yelp (issue 200)
      * Fixed netsniff.coffee example due to wrong indentation (issue 225)
      * Added an example to show live network traffic (issue 227)
      * Added an example demonstrating different output encodings (issue 186)

2011-06-21: Version 1.2.0 "Birds of Paradise"

    Version 1.2.0 is a major update. It introduces a whole set of new API.

    Bug fixes

      * Fixed rendering a very large web page (issue 54)
      * Fixed reporting of CoffeeScript compile error (issue 125)

    New features

      * Added callback for console message (issue 12)
      * Improved security model via WebPage object (issue 41)
      * Added support for POST, HEAD, PUT, and DELETE (issue 88)
      * Scripts filename is now passed as phantom.scriptName
      * Added callback to capture resource requests and responses (issue 2)
      * Added the ability to load external JavaScript (issue 32)

    Examples

      * Ported examples to use WebPage object
      * Added a new example to upload an image to imagebin.org
      * Added a new example to show HTTP POST feature
      * Added a new example to sniff network traffic and save it in HAR format


2011-04-27: Version 1.1.0 "Cherry Blossom"

    Fixed the script loading to use UTF-8 encoding (Yasuhiro Matsumoto).

    Added check for system proxy setting (Yasuhiro Matsumoto).

    Fixed building with Cygwin and Qt 4.5 (John Dalton).

    Added a new example: driver for QUnit tests (Łukasz Korecki).

    Fixed issue #20: problem with JPG transparent color (Alessandro Portale).

    Fixed issue #9: ignore first line starting with #! (Matthias, aka fourplusone).

    Fixed issue #7: support for file upload for form submission (Matthias, aka fourplusone).

    Fixed issue #35: support for disabling images loading (Ariya Hidayat).

    Fixed issue #14: enable or disable plugins (Ariya Hidayat).

    Added a new example: using Canvas to produce the color wheel (Ariya Hidayat).

    Added support for rasterizing as GIF image (Ariya Hidayat).

    Added support for CoffeeScript (Ariya Hidayat).

    Fixed issue #19: option for setting the proxy (Clint Berry, Ariya Hidayat).

    Python implementation using PyQt (James Roe).

    Fixed issue #17: Specify paper size for PDF export (Alessandro Portale).

    Fixed issue #60: Win32 and OS/2 icon files (Salvador Parra Camacho).

    Added clipping rectangle to the render function (Wouter de Bie).

    Added an example on sychronous waiting (Gabor Torok).

    Added command line option to use disk cache (Jon Turner).

    Added text extracting example (Weston Ruter).

    Fixed issue #93: Build with Qt < 4.7 (Ariya Hidayat).

    Ported all examples to CoffeeScript (Robert Gieseke).

2011-01-17: Version 1.0.0

    Initial launch.

    The API is centralized at the 'phantom' object (as child of
    window object) which has the properties: args, content,
    loadStatus, state, userAgent, version, viewportSize, and
    the following functions: exit, open, render, sleep.

    Several examples are included, among others: web page rasterizer,
    weather service, headless test framework driver, and many others.
