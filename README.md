<___#KATALONUMMA__>
   
<!DOCTYPE html>
<html lang="en-US" prefix="og: http://ogp.me/ns#" class="no-js">
<head>
	<body>
        <div class="collapse navbar-collapse" id="bs-navbar-main-collapse">
            <ul class="nav navbar-nav navbar-right">
                <li>
                    <a href="https://www.katalon.com/features">Features</a>
                </li>
                <li class="kat-dropdown dropdown">
                                        <a href="https://www.katalon.com/resources-center/" class="dropdown-toggle"
                       data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">Resources</a>
                    <ul class="dropdown-menu">
                        <li><a href="https://www.katalon.com/resources-center/tutorials/">Tutorials</a></li>
                        <li><a href="https://www.katalon.com/resources-center/blog/">Blog</a></li>
                        <li><a href="https://www.katalon.com/videos/">Videos</a></li>
                        <li>
                            <a href="https://www.katalon.com/case-studies">Case Studies</a>
                        </li>
                        <li>
                            <a href="https://docs.katalon.com/display/KD" target="_blank">Documentation</a>
                        </li>
                        <li>
                            <a href="http://api-docs.katalon.com/studio/v5.2.0.1/api/index.html" target="_blank">API Reference</a>
                        </li>
                        <li><a href="https://www.katalon.com/faqs">FAQs</a></li>
                    </ul>
                </li>
                <!-- <li class="kat-dropdown dropdown">
                    <a href="javascript:void(0);" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true"
                       aria-expanded="false">Support</a>
                    <ul class="dropdown-menu">
                        
                        <li><a href="#submit-ticket">Submit Ticket</a></li>
                        <li><a href="https://forum.katalon.com/entry/jsconnect?client_id=katalon-studio&amp;Target=%2F" target="_blank">Forum</a></li>
                    </ul>
                </li> -->
                <li><a href="https://forum.katalon.com/entry/jsconnect?client_id=katalon-studio&amp;Target=%2F" target="_blank">Forum</a></li>
                <li>
                    <a href="https://www.kms-technology.com/katalon-services" target="">Services</a>
                </li>
                <li class="btn-join-beta">
                    <a id="download-btn-header" href="#katalon-download" class="btn btn-download btn-top"
                       onclick="kat.clickDownloadBtn('Navigation Bar')">Download</a>
                </li>
                <!-- <li>
                  <a href="#" class="active">Sign in</a>
                </li> -->
                <li><a class="page-scroll" href="#katalon-login" title="Sign in">Sign in</a></li>            </ul>
        </div>
        <!-- /.navbar-collapse -->
    </div>
    <!-- /.container -->
</nav>

<section id="category-header">
    <div class="container">
        <div class="row cat-header">
            <h3 class="brand-heading">Tutorials</h3>        </div>

                    <div class="row">
                <div class="sub-cats">
                    <a class="card page-scroll active" href="https://www.katalon.com/resources-center/tutorials/#get-started"><span class=""></span>Get Started</a><a class="card page-scroll" href="https://www.katalon.com/resources-center/tutorials/#test-design"><span class="two"></span>Test Design</a><a class="card page-scroll" href="https://www.katalon.com/resources-center/tutorials/#test-execution"><span class="three"></span>Test Execution</a><a class="card page-scroll" href="https://www.katalon.com/resources-center/tutorials/#advanced"><span class="five"></span>Advanced</a><a class="card page-scroll" href="https://www.katalon.com/resources-center/tutorials/#configurations"><span class="six"></span>Configurations</a>                </div>
            </div>
            </div>
</section>

<!-- We will have the same content for all type of post, so using this one directly -->

          <div class="main-content blog-detail">
            <div class="container">
              <div class="row">
                

              <div class="col-md-12">
                <div class="post-container detail" id="blog-view">
                  <div class="post-meta-author big">
                  </div>
                  <!-- <div class="post-meta-thumb">
                                          <img src="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/03/09132859/Katalon-Studio-iOS-and-Android-setup-on-macOS.jpg" class="img-responsive" />
                                      </div> -->

                  <div class="post-content-container">
                    <a href="#" class="post-title" ><h1>Setting up Mobile automation project in macOS</h1></a>                    <div class="post-content">
                      <p><span style="font-weight: 400;">Using Katalon Studio, a tester can design mobile app automation tests for both Android and iOS to run on physical devices, cloud services or emulators.</span><span style="font-weight: 400;"><br />
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
