---
id: 392
title: AWS Amazon WorkSpaces review
date: 2017-03-03T23:22:36-05:00
author: admin
layout: revision
guid: http://www.neilkoch.com/index.php/2017/03/03/340-autosave-v1/
permalink: /?p=392
---
<p style="text-align: justify;">
  AWS or Amazon Web Services in March this year released their new product called Amazon WorkSpaces. I thought I would give it a whirl to see how it goes. Amazon WorkSpaces is a fully managed Virtual Desktop Infrastructure (VDI) service which runs in Amazon&#8217;s cloud infrastructure. You don&#8217;t need any back-end components to have this running as you would with VMware Horizon View for example. In addition there are major cost advantages according to AWS compared to traditional VDI systems. You simply set it up on the fly and a basic desktop is ready to go in about 20 minutes.<br /> <!--more-->
</p>

<p style="text-align: justify;">
  <strong>Signup<br /> </strong>To signup to the service you simply need to go the AWS Management Console and click the Amazon WorkSpaces link under Applications.
</p>

<p style="text-align: justify;">
  <a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-14_52_06-AWS-Management-Console.png"><img loading="lazy" class="aligncenter wp-image-341 size-full" src="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-14_52_06-AWS-Management-Console.png" alt="AWS Management Console" width="283" height="102" /></a><a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-14_52_06-AWS-Management-Console.png"><br /> </a>After you have completed this step click the Launch WorkSpaces option.
</p><figure id="attachment_352" aria-describedby="caption-attachment-352" style="width: 300px" class="wp-caption aligncenter">

[<img loading="lazy" class="wp-image-352 size-medium" src="http://www.neilkoch.com/wp-content/uploads/2014/10/qs_welcome-300x179.png" alt="WorkSpaces Welcome Message" width="300" height="179" srcset="http://www.neilkoch.com/wp-content/uploads/2014/10/qs_welcome-300x179.png 300w, http://www.neilkoch.com/wp-content/uploads/2014/10/qs_welcome-768x457.png 768w, http://www.neilkoch.com/wp-content/uploads/2014/10/qs_welcome.png 821w" sizes="(max-width: 300px) 100vw, 300px" />](http://104.197.194.174/wp-content/uploads/2014/10/qs_welcome.png)<figcaption id="caption-attachment-352" class="wp-caption-text">Picture source: http://docs.aws.amazon.com/workspaces/latest/adminguide/what_is.html</figcaption></figure> 

<p style="text-align: justify;">
  You&#8217;ll be asked to choose a package. Currently the costs are based on Regions as are many AWS products. For North America the Standard Bundle starts at $35 per month as of October 2014 for 1 vCPU, 3.75 GiB Memory, 50 GB User Storage. The highest bundle option is the Performance Plus Bundle which goes for $75 per month and includes the following specs, 2 vCPU&#8217;s, 7.5 GiB Memory, 100 GB User Storage. If you&#8217;re located in other AWS Regions Sydney, Tokyo, or the EU the price rises slightly. These can be viewed <a href="https://aws.amazon.com/workspaces/pricing/">here</a>.
</p><figure id="attachment_345" aria-describedby="caption-attachment-345" style="width: 477px" class="wp-caption aligncenter">

[<img loading="lazy" class="wp-image-345" src="http://104.197.194.174/wp-content/uploads/2014/10/qs_get_started-300x243.png" alt="qs_get_started" width="477" height="386" srcset="http://www.neilkoch.com/wp-content/uploads/2014/10/qs_get_started-300x243.png 300w, http://www.neilkoch.com/wp-content/uploads/2014/10/qs_get_started-768x623.png 768w, http://www.neilkoch.com/wp-content/uploads/2014/10/qs_get_started.png 794w" sizes="(max-width: 477px) 100vw, 477px" />](http://104.197.194.174/wp-content/uploads/2014/10/qs_get_started.png)<figcaption id="caption-attachment-345" class="wp-caption-text">Picture source http://docs.aws.amazon.com/workspaces/latest/adminguide/what_is.html</figcaption></figure> 

<p style="text-align: justify;">
  After you have setup your new WorkSpace the following summary is displayed.
</p>

<p style="text-align: justify;">
  <a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-12_28_04-WorkSpaces-Management-Console.png"><img loading="lazy" class="aligncenter wp-image-343 size-medium" src="http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_28_04-WorkSpaces-Management-Console-300x142.png" alt="WorkSpaces Management Console" width="300" height="142" srcset="http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_28_04-WorkSpaces-Management-Console-300x142.png 300w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_28_04-WorkSpaces-Management-Console-768x363.png 768w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_28_04-WorkSpaces-Management-Console-1024x485.png 1024w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_28_04-WorkSpaces-Management-Console.png 1044w" sizes="(max-width: 300px) 100vw, 300px" /></a>
</p>

<p style="text-align: justify;">
  This process takes up to 20 minutes according to AWS. Go and grab a coffee if you&#8217;re testing this yourself with your own AWS account. After this completes you will receive an email from AWS which includes the registration code and links to download the client application you will need for the first time you sign in. You&#8217;ll need to visit <a href="https://clients.amazonworkspaces.com/">https://clients.amazonworkspaces.com/</a> to get the latest client depending on how you will be connecting.
</p>

<p style="text-align: justify;">
  For this demo I used the Windows client.
</p>

<p style="text-align: justify;">
  <a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-12_20_20-Amazon-WorkSpaces-Client-Download.png"><img loading="lazy" class="aligncenter size-medium wp-image-346" src="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-12_20_20-Amazon-WorkSpaces-Client-Download-300x172.png" alt="Amazon WorkSpaces Client Download" width="300" height="172" srcset="http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_20_20-Amazon-WorkSpaces-Client-Download-300x172.png 300w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_20_20-Amazon-WorkSpaces-Client-Download.png 534w" sizes="(max-width: 300px) 100vw, 300px" /></a>
</p>

<p style="text-align: justify;">
  Here you will need to enter your registration code you would have received in the email through the signup process.
</p>

<p style="text-align: justify;">
  <a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-12_23_08-Amazon-WorkSpaces.png"><img loading="lazy" class="aligncenter wp-image-347 size-medium" src="http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_23_08-Amazon-WorkSpaces-172x300.png" alt="2014-10-24 12_23_08-Amazon WorkSpaces" width="172" height="300" srcset="http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_23_08-Amazon-WorkSpaces-172x300.png 172w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_23_08-Amazon-WorkSpaces.png 353w" sizes="(max-width: 172px) 100vw, 172px" /></a>
</p>

<p style="text-align: justify;">
  After you enter you credentials you will then log into your new WorkSpace. The log in process takes around 5 to 10 seconds max.
</p>

<p style="text-align: justify;">
  <a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-12_55_03-Amazon-WorkSpaces.png"><img loading="lazy" class="aligncenter wp-image-348 size-medium" src="http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_55_03-Amazon-WorkSpaces-172x300.png" alt="Amazon WorkSpaces" width="172" height="300" srcset="http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_55_03-Amazon-WorkSpaces-172x300.png 172w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-12_55_03-Amazon-WorkSpaces.png 353w" sizes="(max-width: 172px) 100vw, 172px" /></a>
</p>

<p style="text-align: justify;">
  Now that you have logged in you will have your new Amazon WorkSpace up and running.
</p>

<p style="text-align: justify;">
  <a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-12_57_10-Amazon-WorkSpaces.png"><img loading="lazy" class="aligncenter wp-image-349" src="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-12_57_10-Amazon-WorkSpaces-300x247.png" alt="Amazon WorkSpaces" width="472" height="389" /></a>
</p>

<p style="text-align: justify;">
  After you have logged in you will be presented with a Windows 7 desktop experience which is provided through Windows 2008 R2 behind the scenes through AWS.
</p>

<p style="text-align: justify;">
  One thing to note, all users will have Local Administrative rights to the desktop so if you are an Administrator for your company looking after this it&#8217;s important to be aware of this. Further details are the <a href="https://aws.amazon.com/workspaces/faqs/">FAQ</a>;
</p>

> &#8220;Q: Can users install applications on their WorkSpace?
> 
> By default, users are configured as local administrators of their WorkSpaces. Administrators can change this setting and can restrict users’ ability to install applications with a technology such as Group Policy.&#8221;

<p style="text-align: justify;">
  If you&#8217;re an IT Administrative you should note Windows Update will require updates and is enabled by default.
</p>

<p style="text-align: justify;">
  <a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-13_16_25-Amazon-WorkSpaces.png"><img loading="lazy" class="aligncenter wp-image-354" src="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-13_16_25-Amazon-WorkSpaces-300x246.png" alt="Amazon WorkSpaces" width="629" height="516" srcset="http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-13_16_25-Amazon-WorkSpaces-300x246.png 300w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-13_16_25-Amazon-WorkSpaces-768x630.png 768w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-13_16_25-Amazon-WorkSpaces-1024x840.png 1024w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-13_16_25-Amazon-WorkSpaces.png 1097w" sizes="(max-width: 629px) 100vw, 629px" /></a>
</p>

<p style="text-align: justify;">
  AWS recommends that you have a 100ms ping to the region you are connecting to. So if you are outside the recommended ping times you&#8217;ll experience minor delays in using the cursor or typing. However the plus side to this is the type of connection speeds you will experience within the AWS WorkSpace. I ran a quick SpeedTest and the results speak for themselves. On a quick test I did the upload speed was higher than the download&#8230;
</p>

<p style="text-align: justify;">
  <a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-13_22_55-Amazon-WorkSpaces.png"><img loading="lazy" class="aligncenter wp-image-355 size-medium" src="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-13_22_55-Amazon-WorkSpaces-300x188.png" alt="Amazon WorkSpaces SpeedTest" width="300" height="188" srcset="http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-13_22_55-Amazon-WorkSpaces-300x188.png 300w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-13_22_55-Amazon-WorkSpaces.png 730w" sizes="(max-width: 300px) 100vw, 300px" /></a>
</p>

<p style="text-align: justify;">
  Seeing how AWS WorkSpaces handles streaming videos from YouTube and Netflix is another great test to see how good a VDI type solution is.
</p>

<p style="text-align: justify;">
  <a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-13_12_16-Amazon-WorkSpaces.png"><img loading="lazy" class="aligncenter size-medium wp-image-356" src="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-13_12_16-Amazon-WorkSpaces-300x225.png" alt="YouTubeAmazon WorkSpaces" width="300" height="225" srcset="http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-13_12_16-Amazon-WorkSpaces-300x225.png 300w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-13_12_16-Amazon-WorkSpaces-768x577.png 768w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-13_12_16-Amazon-WorkSpaces-1024x769.png 1024w, http://www.neilkoch.com/wp-content/uploads/2014/10/2014-10-24-13_12_16-Amazon-WorkSpaces.png 1188w" sizes="(max-width: 300px) 100vw, 300px" /></a>
</p>

<p style="text-align: justify;">
  There was noticeable delays playing videos displayed in 480p on YouTube, reducing this to 240p resolved this, however it was still rather choppy. Interestingly enough the sound was OK and came across without setbacks. Playing a video on Netflix is probably something I wouldn&#8217;t recommend unless you have a very fast connection and there would be no real advantage to doing this as you could easily enough complete this through the device you are using. Overall from a speed perspective, the faster the connection the better results with these types of tests.
</p>

<p style="text-align: justify;">
  <a href="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-13_39_53-Amazon-WorkSpaces.png"><img loading="lazy" class="aligncenter size-medium wp-image-357" src="http://104.197.194.174/wp-content/uploads/2014/10/2014-10-24-13_39_53-Amazon-WorkSpaces-300x247.png" alt="Amazon WorkSpaces" width="300" height="247" /></a>
</p>

<p style="text-align: justify;">
  <strong>Conclusion<br /> </strong>The setup was very impressive! Considering there is no physical or even virtual servers required to be setup. If you&#8217;re an end user and business owner and don&#8217;t want to dish out money for new hardware there are obvious reasons to choose this solution. From a billing point of view the price to setup this up was pretty impressive also. The total cost for the 4-5 hours of the testing I did was divided between the monthly rate of $35 and the minutes used so overall this cost for the time was about $8.00
</p>

**Document sources:  
** https://aws.amazon.com/  
https://aws.amazon.com/workspaces/  
http://docs.aws.amazon.com/workspaces/latest/adminguide/what_is.html  
**  
**