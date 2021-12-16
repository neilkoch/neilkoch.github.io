---
id: 102
title: Another VMware home lab
date: 2013-03-16T03:57:56-04:00
author: Neil Koch
layout: post
guid: http://www.neilkoch.com/blog/?p=102
permalink: /index.php/2013/03/16/another-vmware-home-lab/
categories:
  - Certifications
  - Uncategorized
  - VCP
  - VMware
---
Late last year I set up a VMware home lab to assist with my preparation for the VCP5 certification&#8230; For this set up I borrowed some ideas from [Sammy Bogaert&#8217;s excellent blog](http://boerlowie.wordpress.com/2011/11/30/building-the-ultimate-vsphere-lab-part-1-the-story/). It was a 100% virtualized within VMware Workstation 9. The system I built has the following hardware;

<!--more-->

  
1 x Intel Core i7-3770 BX80637i73770 Processor &#8211; Quad Core, 8MB L3 Cache, 3.40GHz (3.90GHz Max Turbo), Socket H2 (LGA1155), 77W, Fan, Retail  
1 (4x8GB) x Corsair XMS3 CMX32GX3M4A1333C9 32GB Memory Module &#8211; DDR3, 1333MHz, CL9, DIMM  
1 x Crucial CT128M4SSD2 m4 2.5&#8243; Solid State Drive &#8211; 128GB, SATA III 6Gb/s  
1 x Shuttle XPC SH67H3 Barebone PC &#8211; No CPU, Intel H67 chipset, Socket 1155, No RAM, Gigabit LAN, USB 3.0, No OS  
1 x WD Green WD20EARX Hard Drive &#8211; 2TB, 3.5&#8243; SATA, 64MB Cache  
1 x Lite-On IHAS124-04 Internal DVD Writer DVD+R 24X, DVD-R 24X, DVD+RW 8X, DVD-RW 6X, DVD+R DL 8X, SATA (OEM)  
1 x Thermaltake AC0014 Hard Drive Bay Converter &#8211; 3.5&#8243; to SSD/2.5&#8243; Converter  
1 x Wifi card

It&#8217;s FAST (you can&#8217;t go wrong with 32GB!) small, compact and quiet. Why have a server when you can do this?<em id="__mceDel"><br /> <em id="__mceDel"></em></em><figure id="attachment_103" aria-describedby="caption-attachment-103" style="width: 300px" class="wp-caption aligncenter">

[<img loading="lazy" class="size-medium wp-image-103" alt="The Lab!" src="http://104.197.194.174/wp-content/uploads/2013/03/2013-03-15-22.58.10-300x225.jpg" width="300" height="225" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/2013-03-15-22.58.10-300x225.jpg 300w, http://www.neilkoch.com/wp-content/uploads/2013/03/2013-03-15-22.58.10-768x576.jpg 768w, http://www.neilkoch.com/wp-content/uploads/2013/03/2013-03-15-22.58.10-1024x768.jpg 1024w" sizes="(max-width: 300px) 100vw, 300px" />](http://104.197.194.174/wp-content/uploads/2013/03/2013-03-15-22.58.10.jpg)<figcaption id="caption-attachment-103" class="wp-caption-text">The Lab!</figcaption></figure> 

Wonder what an a Domain Controller, SQL, vCenter and two ESXi VM&#8217;s looks like in VMware Workstation along with a few extra VM&#8217;s thrown in&#8230;?

Make sure you take into consideration [nested VM&#8217;s](http://communities.vmware.com/docs/DOC-8970) within ESXi, vCenter, etc. What is this? Well I&#8217;m running VM&#8217;s within VM&#8217;s so naturally this will cause some delays and potential read/write issues.<figure id="attachment_104" aria-describedby="caption-attachment-104" style="width: 300px" class="wp-caption aligncenter">

[<img loading="lazy" class="size-medium wp-image-104" alt="The Lab in VMware Workstation" src="http://104.197.194.174/wp-content/uploads/2013/03/vmworkstationlab-300x222.jpg" width="300" height="222" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/vmworkstationlab-300x222.jpg 300w, http://www.neilkoch.com/wp-content/uploads/2013/03/vmworkstationlab-768x569.jpg 768w, http://www.neilkoch.com/wp-content/uploads/2013/03/vmworkstationlab-1024x759.jpg 1024w, http://www.neilkoch.com/wp-content/uploads/2013/03/vmworkstationlab.jpg 1244w" sizes="(max-width: 300px) 100vw, 300px" />](http://104.197.194.174/wp-content/uploads/2013/03/vmworkstationlab.jpg)<figcaption id="caption-attachment-104" class="wp-caption-text">The Lab in VMware Workstation</figcaption></figure> 

Also with the amount of memory and the SSD drive I encountered virtual memory size issues when the operating system initially booted. You can change this setting via the below method in Windows 7.<figure style="width: 298px" class="wp-caption aligncenter">

[<img loading="lazy" alt="Virtual memory" src="http://104.197.194.174/wp-content/uploads/2013/03/changevirtualmemory-298x300.jpg" width="298" height="300" />](http://104.197.194.174/wp-content/uploads/2013/03/changevirtualmemory.jpg)<figcaption class="wp-caption-text">Virtual memory</figcaption></figure> 

<p style="text-align: center;">
  <a style="font-weight: bold; text-align: left; font-size: 1rem; line-height: 1;" href="http://104.197.194.174/wp-content/uploads/2013/03/screen-shot.jpg"><img loading="lazy" class="size-medium wp-image-108" alt="Virtual memory changed!" src="http://104.197.194.174/wp-content/uploads/2013/03/screen-shot-278x300.jpg" width="278" height="300" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/screen-shot-278x300.jpg 278w, http://www.neilkoch.com/wp-content/uploads/2013/03/screen-shot.jpg 619w" sizes="(max-width: 278px) 100vw, 278px" /></a>
</p>

<dl class="wp-caption aligncenter" id="attachment_108" style="width: 288px;">
  <dd class="wp-caption-dd">
    Virtual memory changed!
  </dd>
</dl>

<span style="line-height: 1.714285714; font-size: 1rem;">Do you have a lab set up at home? If so what do you have?</span>