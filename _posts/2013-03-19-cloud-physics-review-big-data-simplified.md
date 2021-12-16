---
id: 116
title: 'CloudPhysics review &#8211; Big Data simplified'
date: 2013-03-19T20:59:02-04:00
author: Neil Koch
layout: post
guid: http://www.neilkoch.com/blog/?p=116
permalink: /index.php/2013/03/19/cloud-physics-review-big-data-simplified/
categories:
  - Cloud
  - Cloud Management Tools
  - CloudPhysics
  - Uncategorized
---
CloudPhysics is an online tool for monitoring your VMware environment available from <a href="http://www.cloudphysics.com" target="_blank">CloudPhysics.com</a>. The tool allows you to see a graphical representation of your VMware environment. <span style="line-height: 1.714285714; font-size: 1rem;">The functionality of the reporting is based on setting up a CloudPhysics Observer Server (through an <a href="http://www.vmware.com/technical-resources/virtualization-topics/virtual-appliances/ovf.html" target="_blank">OVF template</a>) and</span><figure id="attachment_119" aria-describedby="caption-attachment-119" style="width: 350px" class="wp-caption aligncenter">

[<img loading="lazy" class=" wp-image-119 " alt="The main monitoring page" src="http://104.197.194.174/wp-content/uploads/2013/03/cp-01-300x201.jpg" width="350" height="251" />](http://104.197.194.174/wp-content/uploads/2013/03/cp-01.jpg)<figcaption id="caption-attachment-119" class="wp-caption-text">The main monitoring page displaying the &#8216;Observer Cards&#8217;</figcaption></figure> 

<!--more--> then providing your credentials back to CloudPhysics. The  service uses vCenter data to report directly back to CloudPhysics and then graphically displays a representation of what your virtual infrastructure looks like.

This comes in handy if you spend your day reviewing logs, reports, triggers, alarms, etc as a VMware Sys Admin. This type of data easily available in a graphical representation can save your a hours off your regular working week! (sorry I have no data to back up this statement! 🙂 )

Below is the installation process I went through and an overview of what the environment looks like on the back-end. The installation took about 10-15 minutes if that. The longer you have the CloudPhysics Observer server running the more data it can send back to CloudPhysics for review via your account. Overall a great system and definitely a company worth following as they further develop their product offerings.

<div id='gallery-1' class='gallery galleryid-116 gallery-columns-1 gallery-size-thumbnail'>
  <figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/03/19/cloud-physics-review-big-data-simplified/cp-001/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-001-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-1-118" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-001-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/03/cp-001-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-118'> You can download the OVA or directly install via an OVF </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/03/19/cloud-physics-review-big-data-simplified/cp-00/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-00-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-1-117" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-00-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/03/cp-00-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-117'> The finished VM running </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon portrait'>
    <a href='http://www.neilkoch.com/index.php/2013/03/19/cloud-physics-review-big-data-simplified/cp-02-uptime-bench-mark/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-02-uptime-bench-mark-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-1-121" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-02-uptime-bench-mark-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/03/cp-02-uptime-bench-mark-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-121'> Uptime Bench Mark full view </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/03/19/cloud-physics-review-big-data-simplified/cp-02-a-uptime-bench-mark/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-02-a-uptime-bench-mark-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-1-120" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-02-a-uptime-bench-mark-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/03/cp-02-a-uptime-bench-mark-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-120'> Uptime Bench Mark VM rating. Gold, Silver, Bronze rated VM&#8217;s </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/03/19/cloud-physics-review-big-data-simplified/cp-03-host-resource-commitment/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-03-host-resource-commitment-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-1-122" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-03-host-resource-commitment-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/03/cp-03-host-resource-commitment-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-122'> Host Resources Commitment </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/03/19/cloud-physics-review-big-data-simplified/cp-04-snapshots-gone-wild/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-04-snapshots-gone-wild-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-1-123" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-04-snapshots-gone-wild-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/03/cp-04-snapshots-gone-wild-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-123'> Snapshots Gone Wild </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/03/19/cloud-physics-review-big-data-simplified/cp-05-vm-reservations-and-limits/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-05-vm-reservations-and-limits-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-1-124" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-05-vm-reservations-and-limits-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/03/cp-05-vm-reservations-and-limits-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-124'> VM Reservations and Limits </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/03/19/cloud-physics-review-big-data-simplified/cp-06-cloud-physics-labs-community-labs/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-06-cloud-physics-labs-community-labs-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-1-125" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-06-cloud-physics-labs-community-labs-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/03/cp-06-cloud-physics-labs-community-labs-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-125'> Community Lab cards </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://www.neilkoch.com/index.php/2013/03/19/cloud-physics-review-big-data-simplified/cp-07-inventory/'><img width="150" height="150" src="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-07-inventory-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="" loading="lazy" aria-describedby="gallery-1-126" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/cp-07-inventory-150x150.jpg 150w, http://www.neilkoch.com/wp-content/uploads/2013/03/cp-07-inventory-100x100.jpg 100w" sizes="100vw" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-126'> Inventory overview </figcaption></figure>
</div>