# ACBuildConfig
[![License](https://img.shields.io/badge/license-Apache%202.0-cb0010.svg)](https://raw.githubusercontent.com/appcron/acinteractor/master/LICENSE)
[![Xcode Version](https://img.shields.io/badge/Xcode-8.3.3-blue.svg)]

Xcode Build Settings for Swift and Objective-C projects.  
Contains the recommended settings we use at AppCron.
- Disables Bitcode.
- Enables recommended warnings.
- Enables recommended Analyzer hints.

## Installation
1. Add the **ACBuildConfig.xcconfig** file to your Xcode project.
   * Make sure it is not added to any of your Build Targets.
2. Select your project in the **Project navigator**.
3. Open the **Info** Tab of your project.
4. Expand **Debug** on the **Configurations** Section.
5. Select **ACBuildConfig** on project level.
   * Do not set it on target level, otherwise it might override your project specific build settings.
6. Do the same for **Release**.

You should now see a new column titled **Config.File (ACBuildConfig.xcconfig)** in your Target's Build Settings.  
Make sure to have selected the **Levels** display option, otherwise you won't see the columns.  
Sometimes Xcode doesn't show the new column. In this case restarting Xcode might help.

You can still override the settings of the config file with target or project specific settings in the *Build Settings* tab.

Happy Coding 🐳
