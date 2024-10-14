---
title: Simplify Your Workflow with EmEditor's Enhanced Macro Deployment Features
date: 2024-10-07T17:15:34.280Z
updated: 2024-10-14T19:31:35.014Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/227cc128988b516c7d6426572fbbb71529867ec9f293f57740eccc844618f624.jpg
---

## Simplify Your Workflow with EmEditor's Enhanced Macro Deployment Features

April 21, 2008 at 8:39 pm [#5677](https://tools.techidaily.com/emeditor/products/) 

[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")

Keymaster

> owilsky wrote:  
> Hi,
> 
> This one is both a cry for help as well as a feature request:
> 
> I created some kind of IDE out of EmEditor for our company.  
> Therefor I created a lot of macros.  
> Unfortunately because of the way EmEditor stores its configuration it is very difficult to deploy and update the macros on all machines:
> 
> – First I install EmEditor  
> – Then I import a .reg file containing the config that everybody should use  
> – Then the problems begins: Our macros are stored in C:Documents and Settings\[username\]Application DataMy Macros.   
> So you see: Every user has another folder where the macros are saved. So I wrote a tool to change the paths in “HKEY\_CURRENT\_USERSoftwareEmSoftEmEditor v3Macros”.  
> Then I saw that the keyboard shortcuts are saved in a binary field in HKEY\_CURRENT\_USERSoftwareEmSoftEmEditor v3Config\[Config Name\]PIKM and that this binary field contains the absolute path in binary form —> **arghhh!!!**
> 
> Is there an easier way to do this? (User PCs don’t have admin rights for working, so I prefer saving macros in profile folders because they are updated quite often)  
> And please consider an easier way to store the configuration in upcoming versions.
> 
> Thanks for any help,  
> Oliver

 One option is use INI file settings, which use relative path, but if My Macro folder is under user profile (sucn as UsersJohnDocuments…), you will still have to fix each relative path.

 Another option is to use a macro, but this too can take some time. Just in case you want to try this option, I wrote the sample macro to start with:
	  

	bAllConfigs = confirm("Do you want to set keyboard in ALL configurations? Click Cancel if you want to set keyboard only in the current configuration.");  
	  

	if(bAllConfigs){  

		cfgs = new Enumerator(editor.Configs);  

		for(; !cfgs.atEnd(); cfgs.moveNext()){  

		    cfg = cfgs.item();  

		    SetKeys(cfg);  

	else {  

		cfg = document.Config;  

		SetKeys(cfg);  

	alert("Keyboard set successfully!");  
	  

	function SetKeys(cfg)  

		lst = cfg.Keyboard.List;  

		// nKey is a virtual key for the shortcut.  

		// nFlags is a combination of eeVirtualKey, eeShift, eeCtrl, and eeAlt.  See the Macro Reference.  

		// nCmd is the command ID for the macro (9216 through 9216 + 1023).  You can use editor.QueryStringByID method to find the exact command ID.  

		lst.Add(nKey, nFlags, nCmd);  

		cfg.Save();  

	 For the next major version, I will try to find a way to transfer the settings, possibly by adding something like \\%MYMACRO\_PATH\\% environment, which can be included in the macro path, so the shortcut settings will be easily transferred to another PC.

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
<li><a href="https://screen-activity-recording.techidaily.com/new-in-2024-from-raw-footage-to-excellence-the-webcam-edition/"><u>[New] In 2024, From Raw Footage to Excellence The Webcam Edition</u></a></li>
<li><a href="https://article-tips.techidaily.com/updated-one-step-shot-simplify-podcast-streaming-for-2024/"><u>[Updated] One Step Shot Simplify Podcast Streaming for 2024</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-uncovering-your-individual-playlist-sanctuary-on-youtube/"><u>[Updated] Uncovering Your Individual Playlist Sanctuary on Youtube</u></a></li>
<li><a href="https://games-able.techidaily.com/do-mac-systems-hold-the-key-to-next-gen-games/"><u>Do Mac Systems Hold the Key to Next-Gen Games?</u></a></li>
<li><a href="https://win-tricks.techidaily.com/emeditor-professional-v11990-release-candidate-enhanced-text-editing-with-head-start-features/"><u>EmEditor Professional v11.9.90 Release Candidate: Enhanced Text Editing with Head Start Features</u></a></li>
<li><a href="https://win-tricks.techidaily.com/explore-the-world-of-emeditor-your-ultimate-compact-and-powerful-text-editor-solution/"><u>Explore the World of EmEditor, Your Ultimate Compact and Powerful Text Editor Solution</u></a></li>
<li><a href="https://win-tricks.techidaily.com/guide-to-easily-disable-columns-temporarily-in-csv-format-with-emeditor-text-editor/"><u>Guide to Easily Disable Columns Temporarily in CSV Format with EmEditor Text Editor</u></a></li>
<li><a href="https://win-tricks.techidaily.com/how-to-implement-latex-style-mathematical-icons-into-your-custom-toolbars-tips-and-strategies-with-emeditor/"><u>How to Implement LaTeX-Style Mathematical Icons Into Your Custom Toolbars: Tips and Strategies with EmEditor</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-ultimate-guide-to-free-pptp-vpn-for-beginners-on-realme-11-proplus-drfone-by-drfone-virtual-android/"><u>In 2024, Ultimate Guide to Free PPTP VPN For Beginners On Realme 11 Pro+ | Dr.fone</u></a></li>
<li><a href="https://fox-sure.techidaily.com/interactive-feature-selection-popup/"><u>Interactive Feature Selection Popup</u></a></li>
<li><a href="https://smart-video-creator.techidaily.com/new-the-ultimate-guide-to-lip-syncing-5-essential-apps-you-need-for-2024/"><u>New The Ultimate Guide to Lip Syncing 5 Essential Apps You Need for 2024</u></a></li>
<li><a href="https://hardware-help.techidaily.com/update-standard-sata-achi-controller-driver-easily/"><u>Update Standard SATA ACHI Controller Driver Easily</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2151858/7443" target="_top" id="2151858">
  <img src="//a.impactradius-go.com/display-ad/7443-2151858" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2151858/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

