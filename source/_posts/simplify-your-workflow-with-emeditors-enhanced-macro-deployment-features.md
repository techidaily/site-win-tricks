---
title: Simplify Your Workflow with EmEditor's Enhanced Macro Deployment Features
date: 2024-10-04T16:39:22.443Z
updated: 2024-10-08T17:54:21.634Z
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
<li><a href="https://fox-direct.techidaily.com/new-essential-websites-how-to-get-the-right-youtube-ringtones-in-2024/"><u>[New] Essential Websites How to Get the Right YouTube Ringtones, In 2024</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/updated-in-2024-top-cycling-sims-worth-your-time/"><u>[Updated] In 2024, Top Cycling Sims Worth Your Time</u></a></li>
<li><a href="https://some-approaches.techidaily.com/updated-top-20-unencumbered-public-domain-pubg-artifacts/"><u>[Updated] Top 20 Unencumbered, Public Domain PUBG Artifacts</u></a></li>
<li><a href="https://win-tricks.techidaily.com/convertir-des-gif-vers-des-fichiers-swf-gratuitement-avec-la-solution-web-de-movavi-guide-detaille/"><u>Convertir Des GIF Vers Des Fichiers SWF Gratuitement Avec La Solution Web De Movavi - Guide Détaillé</u></a></li>
<li><a href="https://win-tricks.techidaily.com/flv-webm-movavi/"><u>FLV 파일을 WebM로 원격적으로 변환하는 편리한 Movavi 도구</u></a></li>
<li><a href="https://win-tricks.techidaily.com/free-online-converter-change-your-gifs-into-mp4-videos-use-movavi/"><u>Free Online Converter: Change Your GIFs Into MP4 Videos - Use Movavi</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-mirror-huawei-nova-y71-to-mac-drfone-by-drfone-android/"><u>In 2024, How to Mirror Huawei Nova Y71 to Mac? | Dr.fone</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-top-7-phone-number-locators-to-track-motorola-g24-power-location-drfone-by-drfone-virtual-android/"><u>In 2024, Top 7 Phone Number Locators To Track Motorola G24 Power Location | Dr.fone</u></a></li>
<li><a href="https://win-answers.techidaily.com/madden-nfl-19-pc-version-resolved-game-crash-issues/"><u>Madden NFL 19 PC Version - Resolved Game-Crash Issues</u></a></li>
<li><a href="https://win-tricks.techidaily.com/mov-conversion-from-tod-quick-and-easy-online-upgrade-with-movavi/"><u>MOV Conversion From TOD - Quick & Easy Online Upgrade with Movavi</u></a></li>
<li><a href="https://article-helps.techidaily.com/srt-production-via-xml-ssa-and-ttml-conversions-for-2024/"><u>SRT Production via XML, SSA & TTML Conversions for 2024</u></a></li>
<li><a href="https://win11.techidaily.com/triumph-in-speed-mastering-double-click-on-windows-pc/"><u>Triumph in Speed: Mastering Double-Click on Windows PC</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2151854/7443" target="_top" id="2151854">
  <img src="//a.impactradius-go.com/display-ad/7443-2151854" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2151854/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

