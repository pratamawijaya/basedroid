Basedroid: A Base Template for Android Apps
======================

Basedroid is a starting framework for new Android apps that serves to eliminate the boilerplate you find yourself writing in apps.

It comes packed with several frameworks and features that make Android development much simpler:

   * roboguice, a dependency injection library, comes configured.  Examples include automatic injection of 
     state management classes, HTTP classes, UI elements, and more.

   * Action Bar Sherlock, an extension of the Android action bar
     pattern which gives your app a consistent look and feel.

   * A singleton HTTP client with GET / POST requests of JSON. 

   * A singleton StateManager that uses Gson to serialize and deserialize data.

   * Several examples of unit testing with roboguice.  The HTTP client and state manager are tested and the tests are integrated into the Maven build process.

Configuring Basedroid
------------

  You must have a PATH variable $ANDROID_HOME set to your Android SDK directory.  
  Basedroid is built on API 16 but is compatible with as low as Android 2.2.

        export ANDROID_HOME=/my/sdk/path
        git clone git://github.com/achuinard/basedroid.git

Building from source
--------------------

  On a Unix-like system you can build Basedroid from source using the following
  command:

        mvn clean package

  To build Basedroid you will need:

  * [Android SDK](http://developer.android.com/sdk/index.html)
  * [Maven 3.0.4](http://maven.apache.org/download.html)


More info
---------

  * Tony Chuinard:

    <http://chuinard.com>
