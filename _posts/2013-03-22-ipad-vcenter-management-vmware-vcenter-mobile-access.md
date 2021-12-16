---
id: 143
title: Want to use your iPad to manage vCenter?
date: 2013-03-22T02:25:46-04:00
author: Neil Koch
layout: post
guid: http://www.neilkoch.com/blog/?p=143
permalink: /index.php/2013/03/22/ipad-vcenter-management-vmware-vcenter-mobile-access/
categories:
  - Cloud Management Tools
  - iPad
  - Uncategorized
  - VMware
  - vSphere
---
The VMware vCenter Mobile Access tool allows you to use your iPad to manage and monitor your vCenter environment. This handy tool I deployed the other day in my lab environment in around 20 minutes or less.<figure id="attachment_159" aria-describedby="caption-attachment-159" style="width: 300px" class="wp-caption aligncenter">

[<img loading="lazy" class="size-medium wp-image-159" alt="VMware vSphere iPad App" src="http://104.197.194.174/wp-content/uploads/2013/03/13-vcma-300x225.jpg" width="300" height="225" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/13-vcma-300x225.jpg 300w, http://www.neilkoch.com/wp-content/uploads/2013/03/13-vcma-768x576.jpg 768w, http://www.neilkoch.com/wp-content/uploads/2013/03/13-vcma.jpg 1024w" sizes="(max-width: 300px) 100vw, 300px" />](http://104.197.194.174/wp-content/uploads/2013/03/13-vcma.jpg)<figcaption id="caption-attachment-159" class="wp-caption-text">VMware vSphere iPad App</figcaption></figure> 

The process is really simple<!--more-->. Here&#8217;s how&#8230;

<strong style="line-height: 1.714285714; font-size: 1rem;">Installation process<br /> </strong><span style="line-height: 1.714285714; font-size: 1rem;">Visit the </span><a style="line-height: 1.714285714; font-size: 1rem;" href="http://labs.vmware.com/flings/vcma" target="_blank">vCMA | VMware Labs</a> <span style="line-height: 1.714285714; font-size: 1rem;">site and download the zip or OVF. Once this is completed copy it across to your vCenter server and locate where you will be installing it from. Copy and paste this location to so that you install insert when you go through the OVF wizard in vCenter.</span><figure id="attachment_145" aria-describedby="caption-attachment-145" style="width: 300px" class="wp-caption aligncenter">

[<img loading="lazy" class="size-medium wp-image-145" alt="Download the OFV or Zip" src="http://104.197.194.174/wp-content/uploads/2013/03/01-vcma-300x236.jpg" width="300" height="236" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/01-vcma-300x236.jpg 300w, http://www.neilkoch.com/wp-content/uploads/2013/03/01-vcma.jpg 762w" sizes="(max-width: 300px) 100vw, 300px" />](http://104.197.194.174/wp-content/uploads/2013/03/01-vcma.jpg)<figcaption id="caption-attachment-145" class="wp-caption-text">Download the OFV or Zip</figcaption></figure> <figure id="attachment_146" aria-describedby="caption-attachment-146" style="width: 300px" class="wp-caption aligncenter">[<img loading="lazy" class="size-medium wp-image-146" alt="02-vcma" src="http://104.197.194.174/wp-content/uploads/2013/03/02-vcma-300x165.jpg" width="300" height="165" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/02-vcma-300x165.jpg 300w, http://www.neilkoch.com/wp-content/uploads/2013/03/02-vcma.jpg 688w" sizes="(max-width: 300px) 100vw, 300px" />](http://104.197.194.174/wp-content/uploads/2013/03/02-vcma.jpg)<figcaption id="caption-attachment-146" class="wp-caption-text">Copy and paste the location</figcaption></figure> 

Open up vCenter and click **File** then **Deploy OVF Template**. Paste in the location of your OVF you previously downloaded from the vCMA site.<figure id="attachment_147" aria-describedby="caption-attachment-147" style="width: 300px" class="wp-caption aligncenter">

[<img loading="lazy" class="size-medium wp-image-147" alt="Deploy OVF template" src="http://104.197.194.174/wp-content/uploads/2013/03/03-vcma-300x141.jpg" width="300" height="141" />](http://104.197.194.174/wp-content/uploads/2013/03/03-vcma.jpg)<figcaption id="caption-attachment-147" class="wp-caption-text">Deploy OVF template</figcaption></figure> 

Follow the prompts, etc.<figure id="attachment_149" aria-describedby="caption-attachment-149" style="width: 300px" class="wp-caption aligncenter">

[<img loading="lazy" class="size-medium wp-image-149" alt="Select your Host and Cluster" src="http://104.197.194.174/wp-content/uploads/2013/03/05-vcma-300x282.jpg" width="300" height="282" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/05-vcma-300x282.jpg 300w, http://www.neilkoch.com/wp-content/uploads/2013/03/05-vcma.jpg 719w" sizes="(max-width: 300px) 100vw, 300px" />](http://104.197.194.174/wp-content/uploads/2013/03/05-vcma.jpg)<figcaption id="caption-attachment-149" class="wp-caption-text">Select your Host and Cluster</figcaption></figure> 

After you have installed the OVF template in vCenter make note of the VM&#8217;s IP address. Next you will then need to download and install the iPad application. Search &#8216;vsphere&#8217; in the search box and select the &#8216;VMware vSphere Client for iPad&#8217; application. Click FREE, then INSTALL.<figure id="attachment_166" aria-describedby="caption-attachment-166" style="width: 400px" class="wp-caption aligncenter">

[<img loading="lazy" class=" wp-image-166   " alt="Download from the iTunes AppStore" src="http://104.197.194.174/wp-content/uploads/2013/03/12-01-vcma-300x225.png" width="400" height="325" />](http://104.197.194.174/wp-content/uploads/2013/03/12-01-vcma.png)<figcaption id="caption-attachment-166" class="wp-caption-text">Download from the iTunes AppStore</figcaption></figure> 

Upon opening the application you&#8217;ll then be asked for the vCMA application DNS name or IP address. You can get this from the vCMA VM that you previously created.<figure id="attachment_167" aria-describedby="caption-attachment-167" style="width: 300px" class="wp-caption aligncenter">

[<img loading="lazy" class="size-medium wp-image-167" alt="vCMA Server Setup" src="http://104.197.194.174/wp-content/uploads/2013/03/12-02-vcma-300x225.png" width="300" height="225" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/12-02-vcma-300x225.png 300w, http://www.neilkoch.com/wp-content/uploads/2013/03/12-02-vcma-768x576.png 768w, http://www.neilkoch.com/wp-content/uploads/2013/03/12-02-vcma.png 1024w" sizes="(max-width: 300px) 100vw, 300px" />](http://104.197.194.174/wp-content/uploads/2013/03/12-02-vcma.png)<figcaption id="caption-attachment-167" class="wp-caption-text">vCMA Server Setup</figcaption></figure> 

After you entering these details you can then enter your vCenter credentials.<figure id="attachment_162" aria-describedby="caption-attachment-162" style="width: 300px" class="wp-caption aligncenter">

[<img loading="lazy" class="size-medium wp-image-162" alt="12-vcma" src="http://104.197.194.174/wp-content/uploads/2013/03/12-vcma-300x225.png" width="300" height="225" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/12-vcma-300x225.png 300w, http://www.neilkoch.com/wp-content/uploads/2013/03/12-vcma-768x576.png 768w, http://www.neilkoch.com/wp-content/uploads/2013/03/12-vcma.png 1024w" sizes="(max-width: 300px) 100vw, 300px" />](http://104.197.194.174/wp-content/uploads/2013/03/12-vcma.png)<figcaption id="caption-attachment-162" class="wp-caption-text">Login screen</figcaption></figure> 

Once you have logged in you&#8217;ll be able to view your ESXi hosts and then further review specific details about the VMs. This also includes the capability to monitor, manage, start, shutdown, restart VMS and also ping and trace route.<figure id="attachment_159" aria-describedby="caption-attachment-159" style="width: 300px" class="wp-caption aligncenter">

[<img loading="lazy" class="size-medium wp-image-159" alt="VMware vSphere iPad App" src="http://104.197.194.174/wp-content/uploads/2013/03/13-vcma-300x225.jpg" width="300" height="225" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/13-vcma-300x225.jpg 300w, http://www.neilkoch.com/wp-content/uploads/2013/03/13-vcma-768x576.jpg 768w, http://www.neilkoch.com/wp-content/uploads/2013/03/13-vcma.jpg 1024w" sizes="(max-width: 300px) 100vw, 300px" />](http://104.197.194.174/wp-content/uploads/2013/03/13-vcma.jpg)<figcaption id="caption-attachment-159" class="wp-caption-text">VMware vSphere iPad App</figcaption></figure> <figure id="attachment_165" aria-describedby="caption-attachment-165" style="width: 225px" class="wp-caption aligncenter">[<img loading="lazy" class="size-medium wp-image-165" alt="Host view" src="http://104.197.194.174/wp-content/uploads/2013/03/15-vcma-225x300.jpg" width="225" height="300" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/15-vcma-225x300.jpg 225w, http://www.neilkoch.com/wp-content/uploads/2013/03/15-vcma.jpg 768w" sizes="(max-width: 225px) 100vw, 225px" />](http://104.197.194.174/wp-content/uploads/2013/03/15-vcma.jpg)<figcaption id="caption-attachment-165" class="wp-caption-text">Host view</figcaption></figure> <figure id="attachment_164" aria-describedby="caption-attachment-164" style="width: 225px" class="wp-caption aligncenter">[<img loading="lazy" class="size-medium wp-image-164" alt="14-vcma" src="http://104.197.194.174/wp-content/uploads/2013/03/14-vcma-225x300.jpg" width="225" height="300" srcset="http://www.neilkoch.com/wp-content/uploads/2013/03/14-vcma-225x300.jpg 225w, http://www.neilkoch.com/wp-content/uploads/2013/03/14-vcma.jpg 768w" sizes="(max-width: 225px) 100vw, 225px" />](http://104.197.194.174/wp-content/uploads/2013/03/14-vcma.jpg)<figcaption id="caption-attachment-164" class="wp-caption-text">Performance monitoring</figcaption></figure> 

&nbsp;