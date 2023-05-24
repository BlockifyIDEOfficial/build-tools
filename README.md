# Build Tools for [Blockify](https://github.com/BlockifyIDEOfficial/BlockifyIDE).

This repository includes JDK 11, Android SDK and tools for BlockifyIDE. An installation script is also available which you can use to easily install the tools.
```
Blockify build tools installer
This script helps you easily install build tools in BlockifyIDE.

Usage:
idesetup -s 33.0.1 -c -j 17
This will install Android SDK 33.0.1 with command line tools and JDK 17.

Options :
-i   Set the installation directory. Defaults to $HOME.
-s   Android SDK version to download.
-c   Download Android SDK with command line tools.
-j   Choose whether to install JDK 11 or JDK 17. Please note that JDK 17 must be preferred. This option will be removed in future.
-m   Manifest file URL. Defaults to 'manifest.json' in 'build-tools' GitHub repository.

For testing purposes:
-a   CPU architecture. Extracted using 'uname -m' by default.
-p   Package manager. Defaults to 'pkg'.
-l   Name of curl package that will be installed before starting installation process. Defaults to 'libcurl'.

-h   Prints this message.
```

## Installing in BlockifyIDE
- Open the BlockifyIDE terminal.
- Start the installation process by executing : `idesetup -c`
- After you execute the command, it'll show a summary of the configuration. Type `y` to confirm the configuration and start the installation process.

Once the installation is finished, the `ide-environment.properties` file will also be updated. If the file already exists, you'll be asked to confirm if you want to rewrite the properties file.

The default configuration is enough for most users. If you want to configure the installation process (like downloading JDK 11 instead of the default JDK 17), you can do so by using the options provided by the script.

Execute the script with `-h` option to see a list of options that you can use.

## Download
You can manually download and install these tools from [Releases](https://github.com/BlockifyIDEOfficial/build-tools/releases).

## Thanks to
- @Lzhiyong for [sdk-tools](https://github.com/Lzhiyong/sdk-tools).
