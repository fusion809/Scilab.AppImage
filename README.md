# Scilab.AppImage
This repository builds the latest Scilab AppImage. It cannot be uploaded to Bintray any more due to its size exceeding their upload size limit.

Presently the AppImage returns the error:

```bash
libEGL warning: DRI3: xcb_connect failed
libEGL warning: DRI2: xcb_connect failed
libEGL warning: DRI2: xcb_connect failed
libEGL warning: DRI3: xcb_connect failed
libEGL warning: DRI2: xcb_connect failed
libEGL warning: DRI2: xcb_connect failed
libEGL warning: DRI3: xcb_connect failed
libEGL warning: DRI2: xcb_connect failed
libEGL warning: DRI2: xcb_connect failed
Could not create a Scilab main class. Error:
Exception in thread "main" java.lang.NoClassDefFoundError: com/artenum/rosetta/ui/Console
        at org.scilab.modules.gui.console.ScilabConsoleBridge.createConsole(Unknown Source)
        at org.scilab.modules.gui.bridge.ScilabBridge.createConsole(Unknown Source)
        at org.scilab.modules.gui.console.ScilabConsole.<init>(Unknown Source)
        at org.scilab.modules.gui.console.ScilabConsole.getConsole(Unknown Source)
        at org.scilab.modules.core.Scilab.<init>(Unknown Source)
Caused by: java.lang.ClassNotFoundException: com.artenum.rosetta.ui.Console
        at java.net.URLClassLoader.findClass(URLClassLoader.java:381)
        at java.lang.ClassLoader.loadClass(ClassLoader.java:424)
        at sun.misc.Launcher$AppClassLoader.loadClass(Launcher.java:331)
        at java.lang.ClassLoader.loadClass(ClassLoader.java:357)
        ... 5 more

Scilab cannot create Scilab Java Main-Class (we have not been able to find the main Scilab class. Check if the Scilab and thirdparty packages are available).
```
