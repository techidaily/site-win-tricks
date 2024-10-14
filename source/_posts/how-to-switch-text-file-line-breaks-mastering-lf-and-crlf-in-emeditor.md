---
title: "How to Switch Text File Line Breaks: Mastering LF and CRLF in EmEditor"
date: 2024-10-12T18:50:06.496Z
updated: 2024-10-14T19:20:43.064Z
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
<li><a href="https://extra-tips.techidaily.com/new-cloud-marketplace-dissecting-cost-structures/"><u>[New] Cloud Marketplace Dissecting Cost Structures</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-get-your-stream-on-point-with-these-top-webcams-for-youtube/"><u>[Updated] Get Your Stream on Point with These Top Webcams for YouTube</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/updated-in-depth-guide-to-extracting-vimeo-media/"><u>[Updated] In-Depth Guide to Extracting Vimeo Media</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-the-instagram-follower-dilemrancy-guide/"><u>[Updated] The Instagram Follower Dilemrancy Guide</u></a></li>
<li><a href="https://youtube-zero.techidaily.com/approved-acceleratedecelerate-your-youtube-videos-a-step-by-step-guide/"><u>2024 Approved Accelerate/Decelerate Your YouTube Videos A Step-by-Step Guide</u></a></li>
<li><a href="https://extra-support.techidaily.com/2024-approved-integrating-slug-lines-into-your-writing-process/"><u>2024 Approved Integrating Slug Lines Into Your Writing Process</u></a></li>
<li><a href="https://win-tricks.techidaily.com/advanced-features-of-emeditor-professional-v7002-beta-text-editing-software/"><u>Advanced Features of EmEditor Professional v7.00.2 Beta - Text Editing Software</u></a></li>
<li><a href="https://win-tricks.techidaily.com/advanced-text-editing-with-emeditor-the-ultimate-free-software/"><u>Advanced Text Editing with EmEditor: The Ultimate Free Software</u></a></li>
<li><a href="https://win-tricks.techidaily.com/emeditor-professional-v11990-release-candidate-enhanced-text-editing-with-head-start-features/"><u>EmEditor Professional v11.9.90 Release Candidate: Enhanced Text Editing with Head Start Features</u></a></li>
<li><a href="https://win-tricks.techidaily.com/emeditor-text-editor-reviewed-in-depth-analysis-of-its-spell-check-feature/"><u>EmEditor Text Editor Reviewed: In-Depth Analysis of Its Spell Check Feature</u></a></li>
<li><a href="https://win-tricks.techidaily.com/explore-the-world-of-emeditor-your-ultimate-compact-and-powerful-text-editor-solution/"><u>Explore the World of EmEditor, Your Ultimate Compact and Powerful Text Editor Solution</u></a></li>
<li><a href="https://win-tricks.techidaily.com/guide-to-easily-disable-columns-temporarily-in-csv-format-with-emeditor-text-editor/"><u>Guide to Easily Disable Columns Temporarily in CSV Format with EmEditor Text Editor</u></a></li>
<li><a href="https://win-tricks.techidaily.com/how-to-implement-latex-style-mathematical-icons-into-your-custom-toolbars-tips-and-strategies-with-emeditor/"><u>How to Implement LaTeX-Style Mathematical Icons Into Your Custom Toolbars: Tips and Strategies with EmEditor</u></a></li>
<li><a href="https://activate-lock.techidaily.com/in-2024-a-how-to-guide-on-bypassing-the-apple-iphone-8-icloud-lock-by-drfone-ios/"><u>In 2024, A How-To Guide on Bypassing the Apple iPhone 8 iCloud Lock</u></a></li>
<li><a href="https://activate-lock.techidaily.com/in-2024-bypass-icloud-activation-lock-with-imei-code-from-apple-iphone-xr-by-drfone-ios/"><u>In 2024, Bypass iCloud Activation Lock with IMEI Code From Apple iPhone XR</u></a></li>
<li><a href="https://facebook.techidaily.com/lock-your-likes-making-photo-sharing-on-facebook-private/"><u>Lock Your Likes: Making Photo Sharing on Facebook Private</u></a></li>
<li><a href="https://win-tricks.techidaily.com/simplify-your-workflow-with-emeditors-enhanced-macro-deployment-features/"><u>Simplify Your Workflow with EmEditor's Enhanced Macro Deployment Features</u></a></li>
<li><a href="https://win11-tips.techidaily.com/stop-windows-from-starting-spotify-by-default/"><u>Stop Windows From Starting Spotify by Default</u></a></li>
<li><a href="https://win-tricks.techidaily.com/troubleshooting-character-set-challenges-for-list-boxes-in-emeditor-text-editor/"><u>Troubleshooting Character Set Challenges for List Boxes in EmEditor Text Editor</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://homestyler.sjv.io/c/5597632/1943647/22993" target="_top" id="1943647">
  <img src="//a.impactradius-go.com/display-ad/22993-1943647" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://homestyler.sjv.io/i/5597632/1943647/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

