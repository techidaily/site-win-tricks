---
title: "How to Switch Text File Line Breaks: Mastering LF and CRLF in EmEditor"
date: 2024-10-04T17:37:26.831Z
updated: 2024-10-08T18:05:13.466Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/28460332c706ced456fd18767c0466a64d105614a00c30d76ebc074f7652f887.jpg
---

## How to Switch Text File Line Breaks: Mastering LF and CRLF in EmEditor

Viewing 2 posts - 1 through 2 (of 2 total)

* Author  
Posts
* July 17, 2009 at 8:00 pm [#7479](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/8018308e3403eaa02d050e84a9e58378?s=80&d=identicon&r=g)mak](https://www.emeditor.com/forums/users/mak/ "View mak's profile")  
Member  
I want to convert UTF-16 Le (LF unix) to UTF-16 (CR+LF to windows) and UTF-8 LE to UTF-8 CR+LF can I use command line if yes what is command line i should use ?  
 Or can I batch process this file in emeditor ?  
 .java files – from UTF-16 Le (LF unix) to UTF-16 (CR+LF to windows)  
 .rc files – from UTF-16 Le (LF unix) to UTF-16 (CR+LF to windows)  
 .XML files —UTF-8 LE to UTF-8 CR+LF  
 I tried many utilities and Sed commands they all are corrupting the files.  
 I can do this by opeing each file in emditor and save as to windows format but this solution is not logical for 200+ files.  
 thanks in advance.  
July 17, 2009 at 9:52 pm [#7480](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
> mak wrote:  
> I want to convert UTF-16 Le (LF unix) to UTF-16 (CR+LF to windows) and UTF-8 LE to UTF-8 CR+LF can I use command line if yes what is command line i should use ?  
> Or can I batch process this file in emeditor ?  
> .java files – from UTF-16 Le (LF unix) to UTF-16 (CR+LF to windows)  
> .rc files – from UTF-16 Le (LF unix) to UTF-16 (CR+LF to windows)  
> .XML files —UTF-8 LE to UTF-8 CR+LF  
> I tried many utilities and Sed commands they all are corrupting the files.  
> I can do this by opeing each file in emditor and save as to windows format but this solution is not logical for 200+ files.  
> thanks in advance.  
 Not on version 8, but on version 9, you will see new command line options /scr /scrlf /slf available. So if you want to convert from UTF-16 (LF unix) to UTF-8 (CR+LF windows), you would use,  
 emeditor.exe “org\_name” /cp 65537 /cps 65001 /ss- /scrlf /sa “new\_name”  
 v9 alpha is available in our beta forum. I hope this will help.
* Author  
Posts

Viewing 2 posts - 1 through 2 (of 2 total)

* You must be logged in to reply to this topic.

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>

<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://fox-http.techidaily.com/new-the-comprehensive-guide-to-crafting-effective-reddit-posts/"><u>[New] The Comprehensive Guide to Crafting Effective Reddit Posts</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/ed-elevating-your-yt-content-with-the-top-thumbnail-hacks-for-2024/"><u>[Updated] Elevating Your YT Content with the Top Thumbnail Hacks for 2024</u></a></li>
<li><a href="https://screen-recording.techidaily.com/updated-in-2024-broadcast-your-games-with-professional-skill/"><u>[Updated] In 2024, Broadcast Your Games with Professional Skill</u></a></li>
<li><a href="https://blog-min.techidaily.com/1-live-streaming-mastery-high-quality-video-with-manycam-and-virtual-camera-solutions/"><u>1. Live Streaming Mastery: High-Quality Video with ManyCam and Virtual Camera Solutions</u></a></li>
<li><a href="https://games-able.techidaily.com/boosting-performance-in-shooter-games-through-sensitivity-tweaks/"><u>Boosting Performance in Shooter Games Through Sensitivity Tweaks</u></a></li>
<li><a href="https://some-approaches.techidaily.com/conversione-libera-per-internet-dei-formati-ogg-e-mp4-con-macrox-video-converter/"><u>Conversione Libera per Internet Dei Formati Ogg E MP4 Con MacroX Video Converter</u></a></li>
<li><a href="https://win-tricks.techidaily.com/hassle-free-system-improvements-mastering-the-art-of-smoother-windows-updates/"><u>Hassle-Free System Improvements: Mastering the Art of Smoother Windows Updates.</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-best-3-vivo-v27-pro-emulator-for-mac-to-run-your-wanted-android-apps-drfone-by-drfone-android/"><u>In 2024, Best 3 Vivo V27 Pro Emulator for Mac to Run Your Wanted Android Apps | Dr.fone</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/instas-tunes-ownership-and-legalities/"><u>Insta's Tunes Ownership & Legalities</u></a></li>
<li><a href="https://win-tricks.techidaily.com/is-integrating-android-with-windows-11-beneficial-explore-insights-from-zdnet/"><u>Is Integrating Android with Windows 11 Beneficial? Explore Insights From ZDNet</u></a></li>
<li><a href="https://win-tricks.techidaily.com/navigating-microsofts-future-plans-transformative-strategies-for-enhanced-cloud-computing-targeted-ad-campaigns-and-cross-device-connectivity-itinnovators.m243/"><u>Navigating Microsoft's Future Plans: Transformative Strategies for Enhanced Cloud Computing, Targeted Ad Campaigns, and Cross-Device Connectivity | ITInnovators</u></a></li>
<li><a href="https://win-tricks.techidaily.com/revolutionizing-tech-with-microsofts-new-approach-to-cloud-services-and-devices-a-deep-dive-by-zdnet/"><u>Revolutionizing Tech with Microsoft's New Approach to Cloud Services & Devices – A Deep Dive by ZDNet</u></a></li>
<li><a href="https://win-tricks.techidaily.com/seamless-file-sharing-from-windows-to-android-with-microsofts-new-feature-tech-news/"><u>Seamless File Sharing From Windows to Android with Microsoft’s New Feature | Tech News</u></a></li>
<li><a href="https://win-tricks.techidaily.com/supercharge-microsoft-edge-must-have-addons-and-plugins-for-a-better-browsing-journey/"><u>Supercharge Microsoft Edge: Must-Have Addons and Plugins for a Better Browsing Journey</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/the-secret-to-stylish-borders-in-instagram-visuals-for-2024/"><u>The Secret to Stylish Borders in Instagram Visuals for 2024</u></a></li>
<li><a href="https://win-tricks.techidaily.com/top-methods-for-capturing-your-screen-on-windows-11-not-just-with-game-bar/"><u>Top Methods for Capturing Your Screen on Windows 11, Not Just with Game Bar</u></a></li>
<li><a href="https://win-tricks.techidaily.com/understanding-the-role-of-a-tpm-in-windows-11-a-comprehensive-guide/"><u>Understanding the Role of a TPM in Windows 11: A Comprehensive Guide</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137213/26400" target="_top" id="2137213">
  <img src="//a.impactradius-go.com/display-ad/26400-2137213" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137213/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

