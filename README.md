# KatalonUmma
<p>A sample project for Mobile automation</p>
<ul>
  <font size="24px"><li>1. Setup Prerequisites</li></font>
          Configuration

Katalon Studio requires the latest installation of Appium and Node.js. Please setup as the following steps:

    Install Homebrew from Terminal:

/usr/bin/ruby -e "$(curl -fsSL
https://raw.githubusercontent.com/Homebrew/install/master/install)"

    Install Carthage with Homebrew:

brew install carthage

    Install node and npm with Homebrew:

brew install node

brew install npm

Note: To make sure Node.js is installed correctly, you run the command which node on Terminal.

    Install Appium with npm

npm install -g appium

    Set Appium Directory to “/usr/local/lib/node_modules/appium” in Katalon Preferences (from Katalon menu, go to Preferences > Katalon > Mobile)

You will need to install and configure Xcode in case of testing on iOS devices. Please set up Xcode as follows:

    Open Xcode > Preferences > Accounts: Add developer’s Apple ID



<img src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25103608/Add-acocunt-in-Xcode.png" border="5px #000 solid" align="right" />


    Open Terminal at WebDriverAgent in Appium directory folder:
    <…>/appium/node_modules/appium-xcuitest-driver/WebDriverAgent and enter following command to initialize WebDriverAgent project:

mkdir -p Resources/WebDriverAgent.bundle

sh ./Scripts/bootstrap.sh -d

    Open project WebDriverAgent.xcodeproj under WebDriverAgent in Xcode.
</ul>
