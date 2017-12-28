# KatalonUmma
<p>A sample project for Mobile automation</p>
<ul>
 <li> <font size="large"> 1. Setup Prerequisites </font> </li>

Katalon Studio requires the latest installation of Appium and Node.js. Please setup as the following steps:

<li>Install Homebrew from Terminal:</li>

    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

<li>Install Carthage with Homebrew:</li>

    brew install carthage

<li>Install node and npm with Homebrew:</li>

    brew install node

    brew install npm

<li>Note: To make sure Node.js is installed correctly, you run the command which node on Terminal.</li>

<li>Install Appium with npm</li>

    npm install -g appium


<li>2. Set Appium Directory to “/usr/local/lib/node_modules/appium” in Katalon Preferences (from Katalon menu, go to Preferences > Katalon > Mobile)</li>

You will need to install and configure Xcode in case of testing on iOS devices. Please set up Xcode as follows:

    Open Xcode > Preferences > Accounts: Add developer’s Apple ID



     <img src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25103608/Add-acocunt-in-Xcode.png" border="5px #000 solid" align="left" />
     


<li>Open Terminal at WebDriverAgent in Appium directory folder:</li>
    <…>/appium/node_modules/appium-xcuitest-driver/WebDriverAgent and enter following command to initialize WebDriverAgent project:

    mkdir -p Resources/WebDriverAgent.bundle

    sh ./Scripts/bootstrap.sh -d

<li>Open project WebDriverAgent.xcodeproj under WebDriverAgent in Xcode.</li>

  <li><img src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25103716/Open-WebDriverAgent.xcodeproj.png" border="5px #000 solid" align="left" /></li>
   
   <li>Select WebDriverAgentLib, and in the Signing section, check Automatically manage signing and select a team.</li>
   

