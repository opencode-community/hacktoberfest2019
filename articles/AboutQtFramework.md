#Introduction to Qt framework
##overview
**Qt** (pronounced "cute") is a free and open-source widget toolkit for creating graphical user interfaces as well as cross-platform applications that run on various software and hardware platforms such as Linux, Windows, macOS, Android or embedded systems with little or no change in the underlying codebase while still being a native application with native capabilities and speed. 
##Purposes and abilities
Qt is used for developing graphical user interfaces (GUIs) and multi-platform applications that run on all major desktop platforms and most mobile or embedded platforms. Most GUI programs created with Qt have a native-looking interface, in which case Qt is classified as a widget toolkit. Also non-GUI programs can be developed, such as command-line tools and consoles for servers. An example of such a non-GUI program using Qt is the Cutelyst web framework.

Qt supports various compilers, including the **GCC** C++ compiler and the Visual Studio suite and has extensive internationalization support. Qt also provides Qt Quick, that includes a declarative scripting language called QML that allows using JavaScript to provide the logic. With Qt Quick, rapid application development for mobile devices became possible, while logic can still be written with native code as well to achieve the best possible performance.

Other features include **SQL database access**, **XML parsing**, **JSON parsing**, **thread management** and **network support**. 
##Qt Editions and Licenses
There are four editions of Qt available: 
1. Community
2. Indie Mobile
3. Professional 
4. Enterprise.
The **Community** version is under the open source licenses, while the **Indie Mobile**, **Professional** and **Enterprise** versions, which contain additional functionality and libraries, e.g. Enterprise Controls are commercially sold by The Qt Company. 
##Qt software architecture
###Complete abstraction of the GUI
When first released, Qt used its own paint engine and controls, emulating the look of the different platforms it runs on when it drew its widgets. This made the porting work easier because very few classes in Qt depended really on the target platform; however, this occasionally led to slight discrepancies where that emulation was imperfect. Recent versions of Qt use the native style APIs of the different platforms, on platforms that have a native widget set, to query metrics and draw most controls, and do not suffer from such issues as often.On some platforms (such as MeeGo and KDE) Qt is the native API. Some other portable graphical toolkits have made different design decisions; for example, wxWidgets uses the toolkits of the target platform for its implementations.
###Signals and slots
A language construct introduced in Qt for communication between objects[85] which makes it easy to implement the observer pattern while avoiding boilerplate code. The concept is that GUI widgets can send signals containing event information which can be received by other controls using special functions known as slots.
###Metaobject compiler
The metaobject compiler, termed moc, is a tool that is run on the sources of a Qt program. It interprets certain macros from the C++ code as annotations, and uses them to generate added C++ code with meta information about the classes used in the program. This meta information is used by Qt to provide programming features not available natively in C++: signals and slots, introspection and asynchronous function calls.
###Language bindings
Qt can be used in several other programming languages like Python, Javascript, C# or Rust via language bindings

###Qt modules

Starting with Qt 4.0 the framework was split into individual modules.With Qt 5.0 the architecture was modularized even further. Qt is now split into essential and add-on modules. 

####Qt essentials
|Module | Description|
|------|---------|
|Qt Core | The only required Qt module, containing classes used by other modules, including the meta-object system, concurrency and threading, containers, event system, plugins and I/O facilities.
|Qt GUI |The central GUI module. In Qt 5 this module now depends on OpenGL, but no longer contains any widget classes.
|Qt Widgets | Contains classes for classic widget based GUI applications and the QSceneGraph classes. Was split off from QtGui in Qt 5.
|Qt QML | Module for QML and JavaScript languages.
|Qt Quick | The module for GUI application written using QML2.
|Qt Quick Controls |Widget like controls for Qt Quick intended mainly for desktop applications.
|Qt Quick Layouts | Layouts for arranging items in Qt Quick.
|Qt Network |Network abstraction layer. Complete with TCP, UDP, HTTP, SSL and since Qt 5.3 SPDY support.
|Qt Multimedia |Classes for audio, video, radio and camera functionality.
|Qt Multimedia Widgets |The widgets from Qt Multimedia.
|Qt SQL |Contains classes for database integration using SQL.
|Qt WebEngine |A new set of Qt Widget and QML webview APIs based on Chromium.
|Qt Test |Classes for unit testing Qt applications and libraries. 

####Qt add-ons

|Module| Description
|-----|-----|
|Active Qt |Classes for applications which use ActiveX.
|Qt Bluetooth |Classes accessing Bluetooth hardware.
|Qt D-Bus |Classes for IPC using the D-Bus protocol.
|Qt NFC |Classes accessing NFC hardware. Only officially supported on BlackBerry hardware so far (or N9 in the MeeGo port).
|Qt OpenGL |Legacy module containing the OpenGL classes from Qt 4. In Qt 5 the similar functionality in Qt GUI is recommended.
|Qt Location |Classes for accessing GPS and other location services and for mapping and navigation. Split off from the Qt 4 Mobility module of Qt Location. Supported on Android, BlackBerry, iOS, Linux (using GeoClue), Windows and Sailfish OS.
|Qt Script |Legacy module for scripting Qt application using ECMAScript/JavaScript. In Qt 5, using similar classes in Qt QML is recommended.
|Qt Sensors |Classes for accessing various mobile hardware sensors. Used to be part of Qt Mobile in Qt 4. Supported on Android, BlackBerry, iOS, WinRT, Mer and Linux.
|Qt Serial Port |Classes for access to hardware and virtual serial ports. Supported on Windows, Linux and macOS.
|Qt WebChannel |Provides access to Qt objects to HTML/Js over WebSockets.
|Qt WebKit |Qt's WebKit implementation and API.
|Qt WebKit Widgets |The widget API for Qt WebKit
|Qt WebSockets |Provides a WebSocket implementation.
|Qt XML |Legacy module containing classes for SAX and DOM style XML APIs. Replaced with QXmlStreamReader and QXmlStreamWriter classes in Qt Core.
|Qt XML Patterns |Support for XPath, XQuery, XSLT and XML Schema validation. 

Source : [wikipedia](https://en.wikipedia.org/wiki/Qt_(software))

