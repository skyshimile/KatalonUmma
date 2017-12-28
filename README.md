<__#KATALONUMMA___>

<!DOCTYPE html>
<html lang="en-US" prefix="og: http://ogp.me/ns#" class="no-js">

<details open>
<summary>
	
<blockquote>
<head>
	<body>
	  <span style="font-weight: 400;"> Setup a mobile app testing project for Katalon Studio on macOS.</span></p>
<h2><b>1. Setup Prerequisites</b></h2>
<p><span style="font-weight: 400;">Katalon Studio requires the latest installation of </span><a href="http://appium.io/"><span style="font-weight: 400;">Appium</span></a>
	<span style="font-weight: 400;"> and </span>
	<a href="https://nodejs.org/en/">
		<span style="font-weight: 400;">Node.js</span></a>
	<span style="font-weight: 400;">. Please setup as the following steps:</span></p>

<li style="font-weight: 400;"><span style="font-weight: 400;">Install </span>
<a href="http://brew.sh/"><span style="font-weight: 400;">Homebrew</span></a>
<span style="font-weight: 400;"> from </span>
<b>Terminal</b>
<span style="font-weight: 400;">:</span></li>
<table>
<tbody>
<tr>
<td><code><span style="font-weight: 400;">/usr/bin/ruby -e "$(curl -fsSL </span>
	<span style="font-weight: 400;"><br />
https://raw.githubusercontent.com/Homebrew/install/master/install)"</span></code></td>
</tr>
</tbody>
</table>
<ul>
<li><span style="font-weight: 400;">Install </span>
	<a href="https://github.com/Carthage/Carthage"><span style="font-weight: 400;">Carthage</span></a>
	<span style="font-weight: 400;"> with </span>
	<b>Homebrew</b><span style="font-weight: 400;">:</span></li>
</ul>
<table>
<tbody>
<tr>
<td><span style="font-weight: 400;"><code>brew install carthage</code></span></td>
</tr>
</tbody>
</table>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Install </span><b>node</b><span style="font-weight: 400;"> and </span><b>npm</b><span style="font-weight: 400;"> with </span><b>Homebrew</b><span style="font-weight: 400;">:</span></li>
</ul>
<table style="height: 98px;" width="230">
<tbody>
<tr style="height: 7px;">
<td style="width: 220px; height: 7px;"><span style="font-weight: 400;"><code>brew install node</code></span></p>
<p><span style="font-weight: 400;"><code>brew install npm</code></span></td>
</tr>
</tbody>
</table>
<p><span style="font-weight: 400;">Note: To make sure </span><b>Node.js</b><span style="font-weight: 400;"> is installed correctly, you run the command </span><b>which node</b><span style="font-weight: 400;"> on Terminal. </span></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Install </span><b>Appium</b><span style="font-weight: 400;"> with </span><b>npm</b></li>
</ul>
<table>
<tbody>
<tr>
<td><span style="font-weight: 400;"><code>npm install -g appium</code></span></td>
</tr>
</tbody>
</table>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Set Appium Directory to </span><b>&#8220;/usr/local/lib/node_modules/appium&#8221; </b><span style="font-weight: 400;">in Katalon Preferences (from Katalon menu, go to </span><b>Preferences &gt; Katalon &gt; Mobile)</b></li>
</ul>
<p><span style="font-weight: 400;">You will need to install and configure </span><a href="https://developer.apple.com/xcode/"><span style="font-weight: 400;">Xcode</span></a><span style="font-weight: 400;"> in case of testing on iOS devices. Please set up Xcode as follows:</span></p>
<ul>
<li><span style="font-weight: 400;">Open </span><b>Xcode &gt; Preferences &gt; Accounts</b><span style="font-weight: 400;">: Add developer’s Apple ID</span></li>
</ul>
<p><img class="init-size alignnone wp-image-1807 size-full" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25103608/Add-acocunt-in-Xcode.png" alt="Add-acocunt-in-Xcode" width="624" height="493" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25103608/Add-acocunt-in-Xcode.png 624w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25103608/Add-acocunt-in-Xcode-300x237.png 300w" sizes="(max-width: 624px) 100vw, 624px" /></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Open Terminal at </span><b>WebDriverAgent</b><span style="font-weight: 400;"> in Appium directory folder:<br />
</span><i><span style="font-weight: 400;">&lt;…&gt;/appium/node_modules/appium-xcuitest-driver/WebDriverAgent</span></i><span style="font-weight: 400;"> and enter following command to initialize </span><b>WebDriverAgent</b><span style="font-weight: 400;"> project:</span></li>
</ul>
<table>
<tbody>
<tr>
<td><span style="font-weight: 400;"><code>mkdir -p Resources/WebDriverAgent.bundle</code></span></p>
<p><span style="font-weight: 400;"><code>sh ./Scripts/bootstrap.sh -d</code></span></td>
</tr>
</tbody>
</table>
<ul>
<li><span style="font-weight: 400;">Open project </span><b>WebDriverAgent.xcodeproj</b><span style="font-weight: 400;"> under </span><b>WebDriverAgent</b><span style="font-weight: 400;"> in Xcode.</span></li>
</ul>
<p><img class="init-size alignnone wp-image-1808 size-full" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25103716/Open-WebDriverAgent.xcodeproj.png" alt="Open-WebDriverAgent.xcodeproj" width="624" height="382" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25103716/Open-WebDriverAgent.xcodeproj.png 624w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25103716/Open-WebDriverAgent.xcodeproj-300x184.png 300w" sizes="(max-width: 624px) 100vw, 624px" /></p>
<ul>
<li><span style="font-weight: 400;">Select </span><b>WebDriverAgentLib</b><span style="font-weight: 400;">, and in the Signing section, check </span><b>Automatically manage signing</b><span style="font-weight: 400;"> and select a team.</span></li>
</ul>
<p><img class="init-size alignnone wp-image-1809 size-full" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104007/Select-target-WebDriverAgentLib.png" alt="Select-target-WebDriverAgentLib" width="624" height="403" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104007/Select-target-WebDriverAgentLib.png 624w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104007/Select-target-WebDriverAgentLib-300x194.png 300w" sizes="(max-width: 624px) 100vw, 624px" /></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Then on Xcode’s menu bar, select </span><b>Product &gt; Build</b></li>
</ul>
<p><img class="init-size alignnone wp-image-1810 size-full" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104038/Select-Build.png" alt="Select-Build" width="624" height="414" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104038/Select-Build.png 624w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104038/Select-Build-300x199.png 300w" sizes="(max-width: 624px) 100vw, 624px" /></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Repeat the last two steps for </span><b>WebDriverAgentRunner</b></li>
</ul>
<p>&nbsp;</p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Build </span><b>WebDriverAgent</b><span style="font-weight: 400;"> to verify whether the steps above work</span></li>
</ul>
<table>
<tbody>
<tr>
<td><span style="font-weight: 400;"><code>xcodebuild -project WebDriverAgent.xcodeproj -scheme WebDriverAgentRunner -destination 'id=&lt;udid&gt;' test</code></span></p>
<p><span style="font-weight: 400;">Note: &lt;udid&gt; is the device UDID of your mobile device. </span></td>
</tr>
</tbody>
</table>
<ul style="list-style-type: disc;">
<li><span style="font-weight: 400;">If the following dialog is shown, select </span><b>Always Allow</b></li>
</ul>
<p><img class="init-size alignnone wp-image-1812 size-full" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104200/Always-allow.png" alt="Always-allow" width="432" height="196" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104200/Always-allow.png 432w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104200/Always-allow-300x136.png 300w" sizes="(max-width: 432px) 100vw, 432px" /></p>
<ul>
<li><span style="font-weight: 400;">You should be able to see </span><i><span style="font-weight: 400;">Listening on USB </span></i><span style="font-weight: 400;">in the build output as below</span></li>
</ul>
<p><img class="init-size alignnone wp-image-1813 size-full" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104232/Build-Output.png" alt="Build-Output" width="585" height="366" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104232/Build-Output.png 585w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104232/Build-Output-300x188.png 300w" sizes="(max-width: 585px) 100vw, 585px" /></p>

<h2><b>2. Setup Devices</b></h2>
<p><span style="font-weight: 400;">For Android devices:</span></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Turn on your Android device’s developer mode (go to </span><b>Settings </b><span style="font-weight: 400;">&gt; </span><b>Developer options</b><span style="font-weight: 400;">).</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Connect the device to your computer via a USB cable. Just confirm if prompted for accepting/trusting the device.</span></li>
</ul>
<p><span style="font-weight: 400;">For iOS devices:</span></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Connect your iOS Devices to your computer via a USB cable. Just confirm if prompted for accepting/trusting the phone.</span></li>
<li style="font-weight: 400;"><b>For iOS 8 and higher</b><span style="font-weight: 400;">, you must enable the service UI automation on the device (connect the iOS device to Xcode) as follows:</span>
<ol>
<li style="font-weight: 400;"><span style="font-weight: 400;">plug in the iOS device </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">open Xcode on Mac </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">go to </span><b>Settings</b><span style="font-weight: 400;"> on the device &gt; </span><b>Developer</b><span style="font-weight: 400;"> &gt; turn ON </span><b>UIAutomation</b></li>
</ol>
</li>
<li style="font-weight: 400;"><b>For iOS 6 and higher</b><span style="font-weight: 400;">, on your iOS device, go to </span><b>Settings &gt; Safari &gt; Advanced</b><span style="font-weight: 400;"> and enable </span><b>Web Inspector</b></li>
</ul>
<p><span style="font-weight: 400;">To test an iOS native application file (</span><b>.ipa</b><span style="font-weight: 400;"> or </span><b>.app</b><span style="font-weight: 400;"> file), make sure the file is already built and signed properly to deploy on the device. Follow these steps to check if an application file is already built and signed correctly:<br />
</span><span style="font-weight: 400;">1. Open </span><b>Xcode</b><span style="font-weight: 400;"> and navigate to </span><b>Window/Devices<br />
</b><span style="font-weight: 400;">2. Choose your device from the Devices list<br />
3. Press the “+” button and choose your application file<br />
</span><br />
<img class="init-size wp-image-1815 alignleft" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104436/Choose-your-application-file.png" alt="Choose-your-application-file" width="548" height="408" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104436/Choose-your-application-file.png 624w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25104436/Choose-your-application-file-300x224.png 300w" sizes="(max-width: 548px) 100vw, 548px" /></p>
<p>4. If installed successfully, the application will appear in the Installed Apps section as shown below</p>
<p><img class="init-size wp-image-1828 alignleft" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25105538/Installed-successfully.png" alt="Installed-successfully" width="549" height="408" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25105538/Installed-successfully.png 624w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25105538/Installed-successfully-300x223.png 300w" sizes="(max-width: 549px) 100vw, 549px" /></p>







<h2><b>3. Desired Capabilities</b></h2>
<p><span style="font-weight: 400;">You can modify extra </span><b>Desired Capabilities</b><span style="font-weight: 400;"> when executing automation test in Katalon Studio. </span></p>
<p><span style="font-weight: 400;">To define Desired Capabilities for local execution using Chrome, Firefox, IE, Safari or Edge, please access </span><b>Project &gt; Settings &gt; Execution &gt; Default &gt; Mobile &gt; iOS</b><span style="font-weight: 400;"> (or Android).</span></p>
<p><span style="font-weight: 400;">The example below shows Desired Capabilities settings for Android to enable Unicode inputs. </span></p>
<p><img class="init-size alignnone wp-image-1830 size-large" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25110650/Desired-capabilities-setting-1024x673.png" alt="Desired-capabilities-setting" width="840" height="552" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25110650/Desired-capabilities-setting-1024x673.png 1024w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25110650/Desired-capabilities-setting-300x197.png 300w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25110650/Desired-capabilities-setting-768x505.png 768w" sizes="(max-width: 840px) 100vw, 840px" /></p>
<p><span style="font-weight: 400;">Refer to </span><a href="https://github.com/SeleniumHQ/selenium/wiki/DesiredCapabilities"><span style="font-weight: 400;">Desired Capabilities</span></a><span style="font-weight: 400;"> for which properties of each web browser are supported by Selenium. For Desired Capabilities to be used with Appium, refer to </span><a href="http://appium.io/slate/en/master/?ruby#appium-server-capabilities"><span style="font-weight: 400;">Appium server capabilities</span></a><span style="font-weight: 400;">.</span></p>
<h2><b>4. External Library</b></h2>
<p><span style="font-weight: 400;">You may use external libraries in your test project. Go to </span><b>Project &gt; Settings &gt; External Libraries</b><span style="font-weight: 400;"> to add new or remove existing libraries for Katalon Studio. External libraries are stored in the Katalon Studio project’s </span><b>Drivers</b><span style="font-weight: 400;"> folder. </span></p>
<p><img class="init-size alignnone wp-image-1831 size-full" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25111218/external-Library-Katalon-Studio.png" alt="external-Library-Katalon-Studio" width="804" height="528" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25111218/external-Library-Katalon-Studio.png 804w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25111218/external-Library-Katalon-Studio-300x197.png 300w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25111218/external-Library-Katalon-Studio-768x504.png 768w" sizes="(max-width: 804px) 100vw, 804px" /></p>
<ul style="list-style-type: disc;">
<li><b>Add</b><span style="font-weight: 400;">: Click to add your external libraries. The selected libraries will be copied to the Katalon project’s </span><b>Drivers</b><span style="font-weight: 400;"> folder.</span></li>
<li><b>Remove:</b><span style="font-weight: 400;"> Click to remove existing libraries. They will be removed from the Katalon project’s </span><b>Drivers</b><span style="font-weight: 400;"> folder.</span></li>
</ul>
<p><span style="font-weight: 400;">The added libraries can be imported and referenced in the </span><a href="https://docs.katalon.com/display/KD/Test+Case+Script+View"><span style="font-weight: 400;">Script View</span></a><span style="font-weight: 400;"> of Katalon Studio:</span></p>
<p><img class="init-size alignnone wp-image-1832 size-full" src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25111249/Script-view-Katalon-Studio1.png" alt="Script-view-Katalon-Studio1" width="758" height="364" srcset="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25111249/Script-view-Katalon-Studio1.png 758w, https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/25111249/Script-view-Katalon-Studio1-300x144.png 300w" sizes="(max-width: 758px) 100vw, 758px" /></p>
   		 </div>
  		</div>
		</div>
  	</div>
</html>
	</blockquote>

