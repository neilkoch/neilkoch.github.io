---
id: 191
title: CloudPhysics New Card Builder Launched!
date: 2013-06-25T09:00:24-04:00
author: Neil Koch
layout: post
guid: http://www.neilkoch.com/blog/?p=191
permalink: /index.php/2013/06/25/cloudphysics-new-card-builder-launched/
image: /wp-content/uploads/2013/06/cp09.jpg
categories:
  - Cloud
  - Cloud Management Tools
  - CloudPhysics
  - Uncategorized
  - VMware
---
CloudPhysics who I have blogged about in the <a href="http://www.neilkoch.com/blog/?p=116" target="_blank">past</a> announced today their much awaited new feature, Card Builder. Recently I had the privilege to try out CloudPhysics new Card Builder. Picture a dynamic interface reporting tool that is intuitive and extremely flexible! All the features you need when putting together reports for vSphere Analytics! <!--more-->

<span style="font-size: 1rem; line-height: 1.714285714;">The card building process allows you to create fully customized vSphere Analytics. The information is extracted directly from the CloudPhysics Observer VM&#8217;s running in your environment. </span><span style="line-height: 1.714285714; font-size: 1rem;">I&#8217;ve been really impressed by how simple it is to create reports that otherwise take a fare while to put together. According to CloudPhysics you can:<br /> </span>

  * _<span style="line-height: 1.714285714; font-size: 1rem;">Create easy, visual reports for your vSphere environment</span>_
  * _<span style="line-height: 1.714285714; font-size: 1rem;">Run mashups across VMs, hosts, datastores, networks, resource pools, VDS, even vCenters</span>_
  * _<span style="line-height: 1.714285714; font-size: 1rem;">Automatically filter out results</span>_
  * _<span style="line-height: 1.714285714; font-size: 1rem;">Report on multiple vCenters from one view</span>_
  * _<span style="line-height: 1.714285714; font-size: 1rem;">Fastest configuration troubleshooting in the world</span>_

<span style="font-size: 1rem; line-height: 1.714285714;">When you&#8217;re a VMware administrator you spend a lot of time on creating reports. <a href="https://www.vmware.com/support/developer/PowerCLI/">vSphere PowerCLI</a> is probably the most common scripting tool you can use to create reports with. It&#8217;s pretty easy to see why you could use the new Card Builder. Here is a script to create a <a href="https://www.vmware.com/technical-resources/script-automation/power-cli.html">&#8216;tabular report of your Virtual Machines&#8217;</a>. This gives you an idea of the operations of pre-defined scripting that occurs behind the scenes with the Card Builder. </span>

<pre>New-VIProperty -Name MemReservation -ObjectType VirtualMachine ` 
 -Value { 
 param($vm) 
 $vm.ExtensionData.Summary.Config.memoryReservation 
 } -Force 
New-VIProperty -Name NumVirtualDisks -ObjectType VirtualMachine ` 
 -Value { 
 param($vm) 
 $vm.ExtensionData.Summary.Config.NumVirtualDisks 
 } -Force 
Get-VM | Select-Object Name, MemoryMB , NumCpu, MemReservation, NumVirtualDisks | Format-Table</pre>

<span style="font-size: 1rem; line-height: 1.714285714;">It&#8217;s pretty easy to see why you would want to use this type of tool&#8230;</span>

<span style="font-size: 1rem; line-height: 1.714285714;">Below are some screen shots from a basic report creation using the Card Builder.</span>

<div id='gallery-2' class='gallery galleryid-191 gallery-columns-3 gallery-size-thumbnail'>
  <figure class='gallery-item'> 
  
  <div class='gallery-icon portrait'>
    <a href='http://www.neilkoch.com/index.php/2013/06/25/cloudphysics-new-card-builder-launched/cp01/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/06/cp01-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-2-240" srcset="http://www.neilkoch.com/wp-content/uploads/2013/06/cp01-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/06/cp01-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-2-240'> The Card Builder card </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/06/25/cloudphysics-new-card-builder-launched/cp02/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/06/cp02-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-2-239" srcset="http://www.neilkoch.com/wp-content/uploads/2013/06/cp02-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/06/cp02-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-2-239'> Create Card page </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/06/25/cloudphysics-new-card-builder-launched/cp04/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/06/cp04-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-2-237" srcset="http://www.neilkoch.com/wp-content/uploads/2013/06/cp04-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/06/cp04-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-2-237'> Available properties to select </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/06/25/cloudphysics-new-card-builder-launched/cp03/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/06/cp03-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-2-238" srcset="http://www.neilkoch.com/wp-content/uploads/2013/06/cp03-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/06/cp03-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-2-238'> Cluster filter options </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon portrait'>
    <a href='http://www.neilkoch.com/index.php/2013/06/25/cloudphysics-new-card-builder-launched/cp05/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/06/cp05-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-2-236" srcset="http://www.neilkoch.com/wp-content/uploads/2013/06/cp05-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/06/cp05-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-2-236'> Datastore filters </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon portrait'>
    <a href='http://www.neilkoch.com/index.php/2013/06/25/cloudphysics-new-card-builder-launched/cp06/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/06/cp06-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-2-235" srcset="http://www.neilkoch.com/wp-content/uploads/2013/06/cp06-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/06/cp06-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-2-235'> Host filters </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/06/25/cloudphysics-new-card-builder-launched/cp10/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/06/cp10-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-2-233" srcset="http://www.neilkoch.com/wp-content/uploads/2013/06/cp10-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/06/cp10-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-2-233'> When you &#8216;drag and drop &#8216;a &#8216;Filter&#8217; a fancy graphic is displayed which guides you through the process on where to drop the item. </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/06/25/cloudphysics-new-card-builder-launched/cp09/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/06/cp09-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-2-231" srcset="http://www.neilkoch.com/wp-content/uploads/2013/06/cp09-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/06/cp09-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-2-231'> Drag and Drop with &#8216;Associated Virtual Machines&#8217; </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/06/25/cloudphysics-new-card-builder-launched/cp11/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/06/cp11-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-2-232" srcset="http://www.neilkoch.com/wp-content/uploads/2013/06/cp11-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/06/cp11-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-2-232'> The finished report </figcaption></figure>
</div>

[Update] Also check out the recent video on from CloudPhysics below.



&nbsp;