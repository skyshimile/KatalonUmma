<___#KATALONUMMA__>
   
<!DOCTYPE html>
<html lang="en-US" prefix="og: http://ogp.me/ns#" class="no-js">
<head>
	<body>
                  
</span><span style="font-weight: 400;"><br />
</span><span style="font-weight: 400;">This tutorial explains how to setup a mobile app testing project for Katalon Studio on macOS. It assumes that you are familiar with automated testing.</span></p>
<h2><b>1. Setup Prerequisites</b></h2>
<p><span style="font-weight: 400;">Katalon Studio requires the latest installation of </span><a href="http://appium.io/"><span style="font-weight: 400;">Appium</span></a><span style="font-weight: 400;"> and </span><a href="https://nodejs.org/en/"><span style="font-weight: 400;">Node.js</span></a><span style="font-weight: 400;">. Please setup as the following steps:</span></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Install </span><a href="http://brew.sh/"><span style="font-weight: 400;">Homebrew</span></a><span style="font-weight: 400;"> from </span><b>Terminal</b><span style="font-weight: 400;">:</span></li>
</ul>
<table>
<tbody>
<tr>
<td><code><span style="font-weight: 400;">/usr/bin/ruby -e "$(curl -fsSL </span><span style="font-weight: 400;"><br />
https://raw.githubusercontent.com/Homebrew/install/master/install)"</span></code></td>
</tr>
</tbody>
</table>
<ul>
<li><span style="font-weight: 400;">Install </span><a href="https://github.com/Carthage/Carthage"><span style="font-weight: 400;">Carthage</span></a><span style="font-weight: 400;"> with </span><b>Homebrew</b><span style="font-weight: 400;">:</span></li>
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
<h2></h2>
<h2></h2>
<h2></h2>
<h2></h2>
<h2></h2>
<h2></h2>
<h2></h2>
<h2></h2>
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
<div class="thumbs-rating-container" id="thumbs-rating-1793" data-content-id="1793"><span class="thumbs-rating-up thumbs-rating-vote-up-active thumbs-rating-voted" onclick="thumbs_rating_vote(1793, 1);" title="Yes"><i class="material-icons">thumb_up</i> (8)</span> <span class="thumbs-rating-down thumbs-rating-vote-down-active thumbs-rating-voted" onclick="thumbs_rating_vote(1793, 2);" title="No"><i class="material-icons">thumb_down</i> (2)</span><span class="thumbs-rating-already-voted" data-text="Voted!"></span><div class="a2a_kit a2a_kit_size_32 addtoany_list" data-a2a-url="https://www.katalon.com/resources-center/tutorials/get-started/set-up-mobile-automation-project-macos/" data-a2a-title="Setting up Mobile automation project in macOS"><a class="a2a_button_twitter" href="https://www.addtoany.com/add_to/twitter?linkurl=https%3A%2F%2Fwww.katalon.com%2Fresources-center%2Ftutorials%2Fget-started%2Fset-up-mobile-automation-project-macos%2F&amp;linkname=Setting%20up%20Mobile%20automation%20project%20in%20macOS" title="Twitter" rel="nofollow noopener" target="_blank"></a><a class="a2a_button_linkedin" href="https://www.addtoany.com/add_to/linkedin?linkurl=https%3A%2F%2Fwww.katalon.com%2Fresources-center%2Ftutorials%2Fget-started%2Fset-up-mobile-automation-project-macos%2F&amp;linkname=Setting%20up%20Mobile%20automation%20project%20in%20macOS" title="LinkedIn" rel="nofollow noopener" target="_blank"></a><a class="a2a_button_facebook" href="https://www.addtoany.com/add_to/facebook?linkurl=https%3A%2F%2Fwww.katalon.com%2Fresources-center%2Ftutorials%2Fget-started%2Fset-up-mobile-automation-project-macos%2F&amp;linkname=Setting%20up%20Mobile%20automation%20project%20in%20macOS" title="Facebook" rel="nofollow noopener" target="_blank"></a></div></div>                      <div class="date-tage">
                        <a href class="date">Feb, 25, 2017</a>
                        <a href="https://www.katalon.com/tag/macos/" rel="tag">macOS</a><a href="https://www.katalon.com/tag/mobile-automation/" rel="tag">mobile automation</a>                      </div>
                    </div>
                </div>
              </div>
            </div>
            <div class="col-md-12 relative-posts">
              <div class="col-md-4">
    <div class="post-container">
        <div class="post-meta-thumb">
                                        <img src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/03/09101740/Katalon-Studio-Quick-start-1024x640.jpg"
                     class="img-responsive"/>
                    </div>
        <div class="post-content-container">
            <a href="https://www.katalon.com/resources-center/tutorials/get-started/quick-start/" class="post-title">
                <h2>Quick Start</h2>
            </a>
                        <div class="post-meta-author">
                <span class="post-date">
                  Oct, 01, 2017                </span>
            </div>
            <div class="post-content">
                &nbsp; &nbsp; A quick guide to set up and start your first automation test with Katalon Studio, a complete test&hellip;            </div>
        </div>
    </div>
</div>
<div class="col-md-4">
    <div class="post-container">
        <div class="post-meta-thumb">
                                        <img src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/08/10153334/5.-Katalon-Addon.png"
                     class="img-responsive"/>
                    </div>
        <div class="post-content-container">
            <a href="https://www.katalon.com/resources-center/tutorials/configure-katalon-studio-web-automation-test-project/" class="post-title">
                <h2>Configuring Katalon Studio for the Web automation test project</h2>
            </a>
                        <div class="post-meta-author">
                <span class="post-date">
                  Aug, 10, 2017                </span>
            </div>
            <div class="post-content">
                Katalon Studio supports functional testing of web applications on Internet Explorer, Edge, Chrome, Firefox and Safari. This tutorial explains how&hellip;            </div>
        </div>
    </div>
</div>
<div class="col-md-4">
    <div class="post-container">
        <div class="post-meta-thumb">
                                        <img src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/07/17153813/Start-Katalon-Studio.png"
                     class="img-responsive"/>
                    </div>
        <div class="post-content-container">
            <a href="https://www.katalon.com/resources-center/tutorials/get-started/install-setup-katalon-studio/" class="post-title">
                <h2>Installing and Setting up Katalon Studio</h2>
            </a>
                        <div class="post-meta-author">
                <span class="post-date">
                  May, 21, 2017                </span>
            </div>
            <div class="post-content">
                &nbsp; Katalon Studio is a simple and powerful test automation solution for not only web and mobile applications but also&hellip;            </div>
        </div>
    </div>
</div>
                  
            </div>
              </div>
            </div>
          </div>

          <aside class="sticky-sidebar">
              <div class="widget widget_tag_subscribe small">
    <div id="big-modal">
      <span class="modal-close" aria-hidden="true">
        <svg fill="currentColor" width="20" height="20" viewBox="0 0 40 40" size="50" preserveAspectRatio="xMidYMid meet"><g><path d="m31.640000000000004 10.703333333333333l-9.29666666666667 9.296666666666667 9.296666666666667 9.296666666666667-2.3433333333333337 2.3433333333333337-9.296666666666667-9.296666666666667-9.296666666666667 9.296666666666667-2.3433333333333337-2.3433333333333337 9.296666666666667-9.296666666666667-9.296666666666665-9.296666666666667 2.3433333333333337-2.3433333333333337 9.296666666666665 9.296666666666667 9.296666666666667-9.296666666666667z"></path></g></svg>      </span>
      <div class="row">
        <form id="katalon_widget_subscribe_form" class="email-form" role="" method="" action="">  
          <h3 class="widget-title">Subscribe for the latest news and tips</h3>
          <fieldset disabled>
            <!-- <input type="text" class="form-control input-lg" name="email" placeholder=""/>
            <button class="btn btn-subscribe btn-lg">Subscribe</button> -->

            <input type="text" class="email-field col-sm-8" placeholder="Your email address…" name="email" id="email" >
            <input type="submit" id="subscribe-btn" class="email-submit col-sm-4" value="Subscribe">
            <div class="error hide"> <span></span></div>
            <div class="success hide"><span></span></div>
          </fieldset>
        </form>
      </div>
    </div>
    <div id="small-modal">
      <div class="email-icon"></div>
    </div>
  </div>
          </aside>



<!-- Footer -->
<footer>
    <div class="container-fluid">
        <div class="container">
            <div class="row">
                <div class="intro-big col-md-4 col-md-offset-0 col-sm-5 col-sm-offset-1">
                    <ul class="list-unstyled">
                        <li><a href="https://www.katalon.com/features">Features</a></li>
                        <li><a href="https://docs.katalon.com/display/KD" target="">Documentation</a></li>
                        <li><a href="https://forum.katalon.com/entry/jsconnect?client_id=katalon-studio&amp;Target=%2F">Forum</a></li>
                        <li><a href="https://www.kms-technology.com/katalon-services" target="">Services</a></li>
                        <li><a href="https://www.katalon.com/about-us" target="">About Us</a></li>
                    </ul>
                </div>
                <div class="col-md-5 col-sm-5">
                    <h4>Contact Us</h4>
                    <div class="address">
                        <p class="lead"><span>550 Pharr Road NE Suite 525. Atlanta, GA 30305</span><br/>Phone: (678)
                            813-1KMS<br/>Fax: (770) 359-0051<br/>
                            Legal, Partner and General inquiries: <a href="mailto:info@katalon.com">info@katalon.com</a>
                        </p>
                    </div>
                </div>
                <div class="col-md-3 col-sm-12">
                    <p class="social text-right">
                        <a href="https://www.facebook.com/katalonstudio.kms" target="_blank"><i class="fa fa-facebook"
                                                                                                aria-hidden="true"></i></a>&nbsp;&nbsp;&nbsp;
                        <a href="https://twitter.com/katalon_studio" target="_blank"><i class="fa fa-twitter"
                                                                                        aria-hidden="true"></i></a>&nbsp;&nbsp;&nbsp;
                        <a href="https://www.linkedin.com/company/katalon-automation-testing-tool" target="_blank"><i
                                    class="fa fa-linkedin" aria-hidden="true"></i></a>&nbsp;&nbsp;&nbsp;
                        <a href="https://www.youtube.com/channel/UC0g8oLvxnX0i3Ul98uSOrPA" target="_blank"><i
                                    class="fa fa-youtube" aria-hidden="true"></i></a>
                    </p>
                </div>
            </div>
        </div>
    </div>

    <div class="footer">
        <div class="container">
            <a href="https://www.katalon.com/terms-of-use">Terms of uses</a>
            <a href="https://www.katalon.com/privacy-policy">Privacy policy</a>
            <a href="https://www.katalon.com/license-agreement">License Agreement</a>
        </div>
    </div>
</footer>

 <script type="text/javascript">
  analytics.track("Viewed Post", {"title":"Setting up Mobile automation project in macOS","category":"Get Started, Tutorials","noninteraction":true}, {"library":"analytics-wordpress"});
    
</script>
    <div id="katalon-account">
        <div id="katalon-user-modal" data-active-form="">
          <div class="signup-modal">
            <div class="modal fade">
              <div class="modal-dialog katalon-login">
  <div class="modal-content">
    <span class="modal-close" data-dismiss="modal" aria-hidden="true">
      <svg fill="currentColor" width="20" height="20" viewBox="0 0 40 40" size="50" preserveAspectRatio="xMidYMid meet"><g><path d="m31.640000000000004 10.703333333333333l-9.29666666666667 9.296666666666667 9.296666666666667 9.296666666666667-2.3433333333333337 2.3433333333333337-9.296666666666667-9.296666666666667-9.296666666666667 9.296666666666667-2.3433333333333337-2.3433333333333337 9.296666666666667-9.296666666666667-9.296666666666665-9.296666666666667 2.3433333333333337-2.3433333333333337 9.296666666666665 9.296666666666667 9.296666666666667-9.296666666666667z"></path></g></svg>    </span>
    <div class="form">
      <div class="text-center ">
          <h3>Sign in
          <span>
          Please sign in to download Katalon Studio or to access the support forum</span></h3>
      </div>

              <form id="katalon_login_form" method="post" action="https://www.katalon.com/">
                    <div>
            <input type="email" name="user_email" id="user_email" value="" placeholder="Email" required autofocus>
            <span class="error hidden"></span> 
          </div>
          <div>
            <input type="password" name="user_pass" id="user_pass" value="" placeholder="Password" data-errormsg="Please choose a password with a minimum of 6 characters" required>
            <span class="error hidden"></span>
          </div> 
          <div class="checkbox-btn">
              <input type="checkbox" id="remember" name="remember" checked >
              <label for="remember" onclick="">Remember me</label>
          </div>
          <input type="hidden" name="action" value="katalon_login">
          <input type="submit" id="login-btn" data-loading-text="Loading..." value="SIGN IN">
          <span class="error hidden error-general"></span>
          <input type="hidden" id="login-security" name="login-security" value="5a0b9c1d79" /><input type="hidden" name="_wp_http_referer" value="/resources-center/tutorials/get-started/set-up-mobile-automation-project-macos/" />        </form>
          </div>
  </div><!-- /.modal-dialog -->
  <div class="function">
      <!-- <p class="pull-left"><a href="#katalon-reset-password" >Forgot your password?</a></p> -->
      <p class="pull-left"><a href="#katalon-reset-password" class="no-cl">Forgot your password?</a></p>
      <p class="pull-right">Don't have an account yet? <a href="#katalon-register">Sign up</a></p>
      <!-- <p class="text-center">Don't have an account yet? <a href="#katalon-register">Sign up</a></p> -->
  </div>
</div>
<div class="modal-dialog katalon-register">
  <div class="modal-content">
    <span class="modal-close" data-dismiss="modal" aria-hidden="true">
      <svg fill="currentColor" width="20" height="20" viewBox="0 0 40 40" size="50" preserveAspectRatio="xMidYMid meet"><g><path d="m31.640000000000004 10.703333333333333l-9.29666666666667 9.296666666666667 9.296666666666667 9.296666666666667-2.3433333333333337 2.3433333333333337-9.296666666666667-9.296666666666667-9.296666666666667 9.296666666666667-2.3433333333333337-2.3433333333333337 9.296666666666667-9.296666666666667-9.296666666666665-9.296666666666667 2.3433333333333337-2.3433333333333337 9.296666666666665 9.296666666666667 9.296666666666667-9.296666666666667z"></path></g></svg>    </span>
    <div class="form">
      <div class="text-center">
          <h3 id="sign-up-then-download-title">Sign up to download</h3>
          <h3 id="sign-up-only-title">Sign up</h3>
          <h3><span>A <span style="color:#6BC550; font-weight: 700; display: inline;"> valid email </span> is required to activate Katalon Studio installation and to access the support forum</span></h3>
      </div>

      <form id="katalon_registration_form" method="post" action="https://www.katalon.com/">
        <div>
          <input type="text" name="user_login" id="user_login" value="" placeholder="Full name" required autofocus>
        </div>
        <div>
          <input type="email" name="user_email" id="user_email" value="" placeholder="Email@email.com" required>
          <span class="error hidden"></span> 
        </div>
        <div>
          <input type="password" name="user_pass" id="user_pass" value="" placeholder="Password, 6 characters minimum" required  min="6">
          <span class="error hidden"></span> 
        </div>
        <div class="checkbox-btn" onclick="toggleDisableAttr('#user_agreement', '#katalon_registration_form #signup-btn')">
            <input type="checkbox" id="user_agreement" name="user_agreement" required >
            <label for="user_agreement" >I agree with Katalon.com <a href="https://katalon.com/privacy-policy" target="_blank">Privacy Policy</a> and <a href="https://katalon.com/terms-of-use" target="_blank">Terms of Use</a></label>
        </div>      
        <input type="hidden" name="action" value="katalon_register"/>
        <input type="submit" id="signup-btn" value="Download" data-loading-text="Loading..." disabled>
        <input type="submit" id="signup-btn" value="Sign up" class="hidden" data-loading-text="Loading..." disabled>
        <span class="error hidden error-general"></span>
        <input type="hidden" id="register-security" name="register-security" value="5a0b9c1d79" /><input type="hidden" name="_wp_http_referer" value="/resources-center/tutorials/get-started/set-up-mobile-automation-project-macos/" />      </form>
    </div>
  </div><!-- /.modal-dialog -->
  <div class="function">
      <p class="text-center">Already have an account? <a href="#katalon-login">Sign in</a></p>
  </div>
</div>

<style type="text/css">
  .katalon-register #sign-up-only-title {
    display: none;
  }

  .katalon-register input#signup-btn.hidden {
    display: none !important;
  }
</style><div class="modal-dialog katalon-reset-password">
    <div class="modal-content">
        <span class="modal-close" data-dismiss="modal" aria-hidden="true">
          <svg fill="currentColor" width="20" height="20" viewBox="0 0 40 40" size="50" preserveAspectRatio="xMidYMid meet"><g><path d="m31.640000000000004 10.703333333333333l-9.29666666666667 9.296666666666667 9.296666666666667 9.296666666666667-2.3433333333333337 2.3433333333333337-9.296666666666667-9.296666666666667-9.296666666666667 9.296666666666667-2.3433333333333337-2.3433333333333337 9.296666666666667-9.296666666666667-9.296666666666665-9.296666666666667 2.3433333333333337-2.3433333333333337 9.296666666666665 9.296666666666667 9.296666666666667-9.296666666666667z"></path></g></svg>        </span>
        <div class="form">
            <div class="text-center">
                <!-- <img src="images/logo-popup.png" alt="Katalon" /> -->
                <h3>Reset password
                    <span>Please enter the registered email<br/>We will send you a link to reset the password</span>
                </h3>
            </div>
            <form method="post" action="" id="katalon_reset_password_form" >
                <div>
                    <input type="email" name="email" id="email" value="" data-errormsg="Enter your email address" placeholder="Email address" required autofocus>
                    <span class="error hidden"></span> 
                </div>
                <input type="submit" id="reset-pass-btn" value="Reset Password">
            </form>
        </div>
    </div>
    <!-- /.modal-dialog -->
    <div class="function">
        <p class="pull-left">Back to <a href="#katalon-login">Sign In</a></p>
        <p class="pull-right">Don't have an account yet? <a href="#katalon-register">Sign Up</a></p>
    </div>
</div><div class="modal-dialog katalon-resend-password">
    <div class="modal-content">
        <span class="modal-close" data-dismiss="modal" aria-hidden="true">
          <svg fill="currentColor" width="20" height="20" viewBox="0 0 40 40" size="50" preserveAspectRatio="xMidYMid meet"><g><path d="m31.640000000000004 10.703333333333333l-9.29666666666667 9.296666666666667 9.296666666666667 9.296666666666667-2.3433333333333337 2.3433333333333337-9.296666666666667-9.296666666666667-9.296666666666667 9.296666666666667-2.3433333333333337-2.3433333333333337 9.296666666666667-9.296666666666667-9.296666666666665-9.296666666666667 2.3433333333333337-2.3433333333333337 9.296666666666665 9.296666666666667 9.296666666666667-9.296666666666667z"></path></g></svg>        </span>
        <div class="form" >
            <div class="text-center">
                <!-- <img src="images/logo-popup.png" alt="Katalon" /> -->
                <h3><span>An email has been sent to your email address that includes a password reset link</span></h3>
            </div>
            <form id="katalon_resend_password_form">
                <p class="text-center only-test">Still don't get the email</p>
                <input type="submit" value="Resend Email" id="resend-btn" data-loading-text="Loading..." >
            </form>
        </div>
    </div>
    <!-- /.modal-dialog -->
    <div class="function">
        <p class="pull-left">Back to <a href="#katalon-login">Sign in</a></p>
        <p class="pull-right">Don't have an account yet? <a href="#katalon-register">Sign up</a></p>
    </div>
</div><div class="modal-dialog katalon-reset-password-change">
  <div class="modal-content">
    <span class="modal-close" data-dismiss="modal" aria-hidden="true">
      <svg fill="currentColor" width="20" height="20" viewBox="0 0 40 40" size="50" preserveAspectRatio="xMidYMid meet"><g><path d="m31.640000000000004 10.703333333333333l-9.29666666666667 9.296666666666667 9.296666666666667 9.296666666666667-2.3433333333333337 2.3433333333333337-9.296666666666667-9.296666666666667-9.296666666666667 9.296666666666667-2.3433333333333337-2.3433333333333337 9.296666666666667-9.296666666666667-9.296666666666665-9.296666666666667 2.3433333333333337-2.3433333333333337 9.296666666666665 9.296666666666667 9.296666666666667-9.296666666666667z"></path></g></svg>    </span>
    <div class="form">
      <div class="text-center">
        <!-- <img src="images/logo-popup.png" alt="Katalon" /> -->
        <h3>Reset password</h3>
      </div>

      <form method="post" action="" id="katalon_reset_password_change_form">
        <div>
          <input type="password" name="pass_new" id="pass_new" value="" placeholder="New password, 6 characters minimum" required autofocus>
          <span class="error hidden"></span> 
        </div> 
        <div>
          <input type="password" name="pass_confirm" id="pass_confirm" value="" placeholder="Confirm password" required>
          <span class="error hidden"></span> 
        </div> 
        <input type="submit" value="Reset" id="reset-btn" data-loading-text="Loading..." disabled>
        <span class="error hidden error-general"></span>
        <input type="hidden" id="login-security" name="login-security" value="5a0b9c1d79" /><input type="hidden" name="_wp_http_referer" value="/resources-center/tutorials/get-started/set-up-mobile-automation-project-macos/" />      </form>
    </div>
  </div><!-- /.modal-content -->
    <div class="function">
      <p class="pull-left">Back to <a href="#katalon-login">Sign in</a></p>
      <p class="pull-right">Don't have an account yet? <a href="#katalon-register">Sign up</a></p>
    </div>
</div><!-- /.modal-dialog --><div class="modal-dialog katalon-change-password-after">
  <div class="modal-content">
    <span class="modal-close" data-dismiss="modal" aria-hidden="true">
      <svg fill="currentColor" width="20" height="20" viewBox="0 0 40 40" size="50" preserveAspectRatio="xMidYMid meet"><g><path d="m31.640000000000004 10.703333333333333l-9.29666666666667 9.296666666666667 9.296666666666667 9.296666666666667-2.3433333333333337 2.3433333333333337-9.296666666666667-9.296666666666667-9.296666666666667 9.296666666666667-2.3433333333333337-2.3433333333333337 9.296666666666667-9.296666666666667-9.296666666666665-9.296666666666667 2.3433333333333337-2.3433333333333337 9.296666666666665 9.296666666666667 9.296666666666667-9.296666666666667z"></path></g></svg>    </span>
    <div class="form">
      <div class="text-center success">
        <img src="https://www.katalon.com/wp-content/themes/katalon/images/success.png" alt="Katalon" />
        <h3>
          <span>Your password has been changed successfully</span>
        </h3>
      </div>            
      <form method="post" action="" id="katalon_change_password_after_form">        
        <input type="submit" value="OK">
      </form>
    </div>
  </div>
</div><div class="modal-dialog katalon-contact-us">
  <div class="modal-content">
      <span class="modal-close" data-dismiss="modal" aria-hidden="true">
        <svg fill="currentColor" width="20" height="20" viewBox="0 0 40 40" size="50" preserveAspectRatio="xMidYMid meet"><g><path d="m31.640000000000004 10.703333333333333l-9.29666666666667 9.296666666666667 9.296666666666667 9.296666666666667-2.3433333333333337 2.3433333333333337-9.296666666666667-9.296666666666667-9.296666666666667 9.296666666666667-2.3433333333333337-2.3433333333333337 9.296666666666667-9.296666666666667-9.296666666666665-9.296666666666667 2.3433333333333337-2.3433333333333337 9.296666666666665 9.296666666666667 9.296666666666667-9.296666666666667z"></path></g></svg>      </span>
      <div class="form contact-us ">
          <div class="caption">
            <h3>Sales Inquiry Contact
            <span class="captionn-text">
              We'll do our best to get back to you <br> as soon as possible.
            </span>
            </h3>
          </div>
          <form method="post" action="" id="katalon_contact_us_form">
              <div>
                  <input type="text" name="user_name" id="user_name" value="" placeholder="Full name (*)" required>
                  <span class="error hidden"></span>
              </div>
              <div>
                  <input type="email" name="user_email" id="user_email" value="" placeholder="Email address (*)" required>
                  <span class="error hidden"></span>
              </div>
              <div>
                  <input type="tel" name="user_phone" id="user_phone" value="" placeholder="Phone number">
                  <span class="error hidden"></span>
              </div>
              <div>
                  <input type="text" name="user_subject" id="user_subject" value="" placeholder="Subject (*)" required>
                  <span class="error hidden"></span>
              </div>

              <div>
                  <textarea placeholder="Message (*)" name="user_message" id="user_message" rows="3"  style="resize:none" required></textarea>
                  <span class="error hidden"></span>
              </div>

              <div class="caption">
                <h3>
                <span class="caption-text">
                  For technical support inquiry, please join our <a href="https://forum.katalon.com/entry/jsconnect?client_id=katalon-studio&amp;Target=%2F" target="">Forum</a>.
                </span>
                </h3>
              </div>

              <input type="hidden" name="action" value="katalon_contact_us"/>
              <input type="submit" id="contact-us-btn" value="Send" data-loading-text="Loading...">
              <span class="error hidden error-general"></span>
              <input type="hidden" id="register-security" name="register-security" value="5a0b9c1d79" /><input type="hidden" name="_wp_http_referer" value="/resources-center/tutorials/get-started/set-up-mobile-automation-project-macos/" />          </form>
      </div>
  </div>
</div>
<div class="modal-dialog katalon-contact-us-after">
  <div class="modal-content">
    <span class="modal-close" data-dismiss="modal" aria-hidden="true">
      <svg fill="currentColor" width="20" height="20" viewBox="0 0 40 40" size="50" preserveAspectRatio="xMidYMid meet"><g><path d="m31.640000000000004 10.703333333333333l-9.29666666666667 9.296666666666667 9.296666666666667 9.296666666666667-2.3433333333333337 2.3433333333333337-9.296666666666667-9.296666666666667-9.296666666666667 9.296666666666667-2.3433333333333337-2.3433333333333337 9.296666666666667-9.296666666666667-9.296666666666665-9.296666666666667 2.3433333333333337-2.3433333333333337 9.296666666666665 9.296666666666667 9.296666666666667-9.296666666666667z"></path></g></svg>    </span>
    <div class="form">
      <div class="text-center success">
        <img src="https://www.katalon.com/wp-content/themes/katalon/images/success.png" alt="Katalon" />
        <h3>
          Thanks for getting in touch!
          <span>We'll try our best to respond as soon as possible.</span>
          <!-- <span>Have a great day ahead!</span> -->
        </h3>
      </div>            
      <form method="post" action="" id="katalon_contact_us_after">        
        <input type="submit" value="OK">
      </form>
    </div>
  </div>
</div>            </div>
          </div>
        </div>
    </div>


</body>
</html>
