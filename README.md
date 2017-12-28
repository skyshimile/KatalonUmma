<___#KATALONUMMA__>
   
<!DOCTYPE html>
<html lang="en-US" prefix="og: http://ogp.me/ns#" class="no-js">
<head>

    <meta charset="UTF-8">
    <!-- <title>Katalon Studio</title> -->
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no"/>
    <!-- <link rel="profile" href="https://gmpg.org/xfn/11"> -->
    <!--     <link rel="pingback" href="https://www.katalon.com/xmlrpc.php">
   -->


    <!-- Favicon -->
    <link rel="shortcut icon" href="https://www.katalon.com/wp-content/themes/katalon/images/katalon_icon_color_normal.png">
    <script>(function(html){html.className = html.className.replace(/\bno-js\b/,'js')})(document.documentElement);</script>
<title>Setting up Mobile automation project in macOS | Katalon Studio</title>

<!-- This site is optimized with the Yoast SEO plugin v4.9 - https://yoast.com/wordpress/plugins/seo/ -->
<meta name="description" content="Using Katalon Studio, mobile automation tester can design automation test for both Android and iOS to run on physical devices, cloud services and emulators."/>
<link rel="canonical" href="https://www.katalon.com/resources-center/tutorials/get-started/set-up-mobile-automation-project-macos/" />
<meta property="og:locale" content="en_US" />
<meta property="og:type" content="article" />
<meta property="og:title" content="Setting up Mobile automation project in macOS" />
<meta property="og:description" content="Using Katalon Studio, mobile automation tester can design automation test for both Android and iOS to run on physical devices, cloud services and emulators." />
<meta property="og:url" content="https://www.katalon.com/resources-center/tutorials/get-started/set-up-mobile-automation-project-macos/" />
<meta property="og:site_name" content="Katalon Studio" />
<meta property="article:publisher" content="https://www.facebook.com/katalonstudio.kms" />
<meta property="article:tag" content="macOS" />
<meta property="article:tag" content="mobile automation" />
<meta property="article:section" content="Get Started" />
<meta property="article:published_time" content="2017-02-25T11:39:12+00:00" />
<meta property="article:modified_time" content="2017-09-01T15:33:23+00:00" />
<meta property="og:updated_time" content="2017-09-01T15:33:23+00:00" />
<meta property="og:image" content="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/03/09132859/Katalon-Studio-iOS-and-Android-setup-on-macOS.jpg" />
<meta name="twitter:card" content="summary" />
<meta name="twitter:description" content="Using Katalon Studio, mobile automation tester can design automation test for both Android and iOS to run on physical devices, cloud services and emulators." />
<meta name="twitter:title" content="Setting up Mobile automation project in macOS" />
<meta name="twitter:site" content="@katalon_studio" />
<meta name="twitter:image" content="https://d1h3p5fzmizjvp.cloudfront.net/wp-content/uploads/2017/03/09132859/Katalon-Studio-iOS-and-Android-setup-on-macOS.jpg" />
<meta name="twitter:creator" content="@katalon_studio" />
<!-- / Yoast SEO plugin. -->

<link rel='dns-prefetch' href='//cdnjs.cloudflare.com' />
<link rel='dns-prefetch' href='//fonts.googleapis.com' />
<link rel='dns-prefetch' href='//maxcdn.bootstrapcdn.com' />
<link rel='dns-prefetch' href='//s.w.org' />
<link rel="alternate" type="application/rss+xml" title="Katalon Studio &raquo; Setting up Mobile automation project in macOS Comments Feed" href="https://www.katalon.com/resources-center/tutorials/get-started/set-up-mobile-automation-project-macos/feed/" />
		<script type="text/javascript">
			window._wpemojiSettings = {"baseUrl":"https:\/\/s.w.org\/images\/core\/emoji\/2.2.1\/72x72\/","ext":".png","svgUrl":"https:\/\/s.w.org\/images\/core\/emoji\/2.2.1\/svg\/","svgExt":".svg","source":{"concatemoji":"https:\/\/www.katalon.com\/wp-includes\/js\/wp-emoji-release.min.js?ver=4.7.5"}};
			!function(a,b,c){function d(a){var b,c,d,e,f=String.fromCharCode;if(!k||!k.fillText)return!1;switch(k.clearRect(0,0,j.width,j.height),k.textBaseline="top",k.font="600 32px Arial",a){case"flag":return k.fillText(f(55356,56826,55356,56819),0,0),!(j.toDataURL().length<3e3)&&(k.clearRect(0,0,j.width,j.height),k.fillText(f(55356,57331,65039,8205,55356,57096),0,0),b=j.toDataURL(),k.clearRect(0,0,j.width,j.height),k.fillText(f(55356,57331,55356,57096),0,0),c=j.toDataURL(),b!==c);case"emoji4":return k.fillText(f(55357,56425,55356,57341,8205,55357,56507),0,0),d=j.toDataURL(),k.clearRect(0,0,j.width,j.height),k.fillText(f(55357,56425,55356,57341,55357,56507),0,0),e=j.toDataURL(),d!==e}return!1}function e(a){var c=b.createElement("script");c.src=a,c.defer=c.type="text/javascript",b.getElementsByTagName("head")[0].appendChild(c)}var f,g,h,i,j=b.createElement("canvas"),k=j.getContext&&j.getContext("2d");for(i=Array("flag","emoji4"),c.supports={everything:!0,everythingExceptFlag:!0},h=0;h<i.length;h++)c.supports[i[h]]=d(i[h]),c.supports.everything=c.supports.everything&&c.supports[i[h]],"flag"!==i[h]&&(c.supports.everythingExceptFlag=c.supports.everythingExceptFlag&&c.supports[i[h]]);c.supports.everythingExceptFlag=c.supports.everythingExceptFlag&&!c.supports.flag,c.DOMReady=!1,c.readyCallback=function(){c.DOMReady=!0},c.supports.everything||(g=function(){c.readyCallback()},b.addEventListener?(b.addEventListener("DOMContentLoaded",g,!1),a.addEventListener("load",g,!1)):(a.attachEvent("onload",g),b.attachEvent("onreadystatechange",function(){"complete"===b.readyState&&c.readyCallback()})),f=c.source||{},f.concatemoji?e(f.concatemoji):f.wpemoji&&f.twemoji&&(e(f.twemoji),e(f.wpemoji)))}(window,document,window._wpemojiSettings);
		</script>
		<style type="text/css">
img.wp-smiley,
img.emoji {
	display: inline !important;
	border: none !important;
	box-shadow: none !important;
	height: 1em !important;
	width: 1em !important;
	margin: 0 .07em !important;
	vertical-align: -0.1em !important;
	background: none !important;
	padding: 0 !important;
}
</style>
<link rel='stylesheet' id='ajax-load-more-css'  href='https://www.katalon.com/wp-content/plugins/ajax-load-more/core/css/ajax-load-more.min.css?ver=4.7.5' type='text/css' media='all' />
<link rel='stylesheet' id='bootstrap-select-style-css'  href='//cdnjs.cloudflare.com/ajax/libs/bootstrap-select/1.12.1/css/bootstrap-select.min.css?ver=1.12.1' type='text/css' media='all' />
<link rel='stylesheet' id='katalon-account-css'  href='https://www.katalon.com/wp-content/plugins/katalon-account/public/css/katalon-account-public.css?ver=17.02.17' type='text/css' media='all' />
<link rel='stylesheet' id='thumbs_rating_styles-css'  href='https://www.katalon.com/wp-content/plugins/thumbs-rating/css/style.css?ver=1.0.0' type='text/css' media='all' />
<link rel='stylesheet' id='wpfront-scroll-top-css'  href='https://www.katalon.com/wp-content/plugins/wpfront-scroll-top/css/wpfront-scroll-top.min.css?ver=1.5' type='text/css' media='all' />
<link rel='stylesheet' id='katalontheme-fonts-css'  href='https://fonts.googleapis.com/css?family=Open+Sans:300,300i,400,400i,600,600i,700,700i' type='text/css' media='all' />
<link rel='stylesheet' id='font-awesome-css'  href='//maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css?ver=4.7.0' type='text/css' media='all' />
<link rel='stylesheet' id='bootstrap-css'  href='//maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css?ver=3.3.7' type='text/css' media='all' />
<link rel='stylesheet' id='material-icons-css'  href='//fonts.googleapis.com/icon?family=Material+Icons&#038;ver=1.0.0' type='text/css' media='all' />
<link rel='stylesheet' id='katalontheme-style-css'  href='https://www.katalon.com/wp-content/themes/katalon/style.css?ver=17.11.27.1' type='text/css' media='all' />
<link rel='stylesheet' id='A2A_SHARE_SAVE-css'  href='https://www.katalon.com/wp-content/plugins/add-to-any/addtoany.min.css?ver=1.14' type='text/css' media='all' />
      <script>
      if (document.location.protocol != "https:") {
          document.location = document.URL.replace(/^http:/i, "https:");
      }
      </script>
      <script type='text/javascript' src='https://www.katalon.com/wp-includes/js/jquery/jquery.js?ver=1.12.4'></script>
<script type='text/javascript' src='https://www.katalon.com/wp-includes/js/jquery/jquery-migrate.min.js?ver=1.4.1'></script>
<script type='text/javascript' src='https://www.katalon.com/wp-content/plugins/add-to-any/addtoany.min.js?ver=1.0'></script>
<script type='text/javascript'>
/* <![CDATA[ */
var thumbs_rating_ajax = {"ajax_url":"https:\/\/www.katalon.com\/wp-admin\/admin-ajax.php","nonce":"dc9b548b52"};
/* ]]> */
</script>
<script type='text/javascript' src='https://www.katalon.com/wp-content/plugins/thumbs-rating/js/general.js?ver=4.0.1'></script>
<script type="text/javascript" src="https://www.katalon.com/wp-content/plugins/wpfront-scroll-top/js/wpfront-scroll-top.min.js?ver=1.5" async="true"></script>
<script type="text/javascript">
	!function(){var analytics=window.analytics=window.analytics||[];if(analytics.invoked)window.console&&console.error&&console.error("Segment snippet included twice.");else{analytics.invoked=!0;analytics.methods=["trackSubmit","trackClick","trackLink","trackForm","pageview","identify","group","track","ready","alias","page","once","off","on"];analytics.factory=function(t){return function(){var e=Array.prototype.slice.call(arguments);e.unshift(t);analytics.push(e);return analytics}};for(var t=0;t<analytics.methods.length;t++){var e=analytics.methods[t];analytics[e]=analytics.factory(e)}analytics.load=function(t){var e=document.createElement("script");e.type="text/javascript";e.async=!0;e.src=("https:"===document.location.protocol?"https://":"http://")+"cdn.segment.com/analytics.js/v1/"+t+"/analytics.js";var n=document.getElementsByTagName("script")[0];n.parentNode.insertBefore(e,n)};analytics.SNIPPET_VERSION="3.0.0";
		window.analytics.load("CKtkuhHutrLD5L4bAWNj16wwaCmP2Oxw");
	window.analytics.page();
	  }}();
</script>
<link rel='https://api.w.org/' href='https://www.katalon.com/wp-json/' />
<link rel="EditURI" type="application/rsd+xml" title="RSD" href="https://www.katalon.com/xmlrpc.php?rsd" />
<link rel="wlwmanifest" type="application/wlwmanifest+xml" href="https://www.katalon.com/wp-includes/wlwmanifest.xml" /> 
<meta name="generator" content="WordPress 4.7.5" />
<link rel='shortlink' href='https://www.katalon.com/?p=1793' />
<link rel="alternate" type="application/json+oembed" href="https://www.katalon.com/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fwww.katalon.com%2Fresources-center%2Ftutorials%2Fget-started%2Fset-up-mobile-automation-project-macos%2F" />
<link rel="alternate" type="text/xml+oembed" href="https://www.katalon.com/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fwww.katalon.com%2Fresources-center%2Ftutorials%2Fget-started%2Fset-up-mobile-automation-project-macos%2F&#038;format=xml" />

<script type="text/javascript">
var a2a_config=a2a_config||{};a2a_config.callbacks=a2a_config.callbacks||[];a2a_config.templates=a2a_config.templates||{};
</script>
<script type="text/javascript" src="https://static.addtoany.com/menu/page.js" async="async"></script>
    </head>
<body data-rsssl=1 id="page-top" data-spy="scroll" data-target=".navbar-fixed-top">
<!-- Navigation -->
<nav class="navbar navbar-default navbar-fixed-top topnav" role="navigation">
    <div class="container topnav menu">
        <div class="navbar-header">
            <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#bs-navbar-main-collapse">
                <span class="sr-only">Toggle navigation</span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
            </button>
            <a class="navbar-brand page-scroll" href="https://www.katalon.com">
                <img class="katalon-logo"
                     src="https://www.katalon.com/wp-content/themes/katalon/images/katalon-studio-logo-notag.svg"
                     alt="Katalon Studio Logo"/>
            </a>
        </div>

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
