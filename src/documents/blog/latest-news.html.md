---
layout: posts
kind: blogpost
title: Latest news
blogExcerpt: "In this post I'll briefly describe what has been done since September."
menuItem: "blog"
blogDate: 2013-12-12 19:24
---
It was a while since I've written something about SolidBuild. Don't worry we worked really hard to bring a new changes. In this post I'll briefly describe each of them.

##Build parameters

Basically, build parameters allow you to control builds with a more granularity. I've added 3 types of build parameters: Users, Systems and Environment parameters.

![Parameters tab](parameters-tab.gif "Parameters tab")

Here is an example of copy script step with a build parameter {BuildVersion}.

![Script builder](script-builder.gif "Script builder")

##Requirements

You can find a new tab in build editor - Requirements. Here you can specify which build clients can build this script.

![Requirements tab](requirements-tab.gif "Requirements tab")

##Builds listing

I've changed builds listing page. I believe now it looks better. On this page you can find your comments from VCS.

![New builds listing](new-builds-listing.gif "New builds listing")
<%-@partial('post-image.html.eco', { url: "latest-news/new-builds-listing.gif", title: "New builds listing" })%>

##Script re-run

On the previous screenshot you can find "re-run" button. Now you can re-run your script at particular revision in VCS. It might be usefull for scripts which deploy your application.  
Now you can re-deploy previous successful version.

##Users

Now you can add your own users to the system. There are only 2 roles available at the moment: Developer and AccountOwner. I'm sure in the future we'll add more.

![Users page](users-page.gif "Users page")

##Email notifications

Before, notifications didn't contain the root cause of the problem. It was annoying. I've changed it :). Now email notifications contain failed tests and errors from log.

![Email notification](email-notification.gif "Email notification")

##Real-time script execution info

From now you can see in real-time information about script execution. Next to each running script we show the name of step which is currently executing.

![Overview page](overview-page.gif "Overview page")

Wow! A lot of new cool stuff I hope you'll enjoy all these.

Cheers,  
Siarhei