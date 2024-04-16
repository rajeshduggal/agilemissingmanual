---
weight: 1
title: "Gradual Migration"
draft: true
---

# Gradual Migration

Some projects require changing to a different technology stack or to move an application to some new infrastructure 

Since doing agile is about gradual change over time it would be beneficial to be able to do it would be beneficial to see if there is a potential to do this to do this migration gradually 

I remember one project many years ago that was coded in classic asp and they were plans to migrate to asp.net technology

(Classic ASP to asp.net content management system CMS.)

so rather rather than creating a project plan to migrate each page and functionality of the application to Asp.net. instead we created this new story to only convert the about us page to asp.net. 

In this case these story was describing modernizing the application essentially to keep it up and running so although there wasn't any new functionality for the end user this project was still needed to keep the application afloat. Meaning if we didn't do this migration the application would be shut down within the organization so it was necessary so the first thing we did is just to convert the about us page only to asp.net while keeping the remainder of the application and classic asp so we have to figure out how can we run both asp.net and classic ASP at the same time.

We were able to convert the about us page to use the new to use the new asp.net CMS system. And we had the content staff login and change the about this text so they could experience it and confirm that they that they we're able to confirm that the new CMS is installed we celebrated the fact that the new CMS is in place the installation of the new CMS is complete. We informed leadership that we have the new CMS in production. Another remainder of the work was just to migrate the all of the existing content in the class KSP system into the new asp.net CMS 

We also there was another project where we were migrating a hosted perl web application  running on Windows that needed to be migrated to a Java cloud Unix infrastructure. And so we found a way to proxy the requests so that they would come from so that we could point the URL to the new cloud infrastructure and every request that came in would be proxied and sent to the window the existing system running on Windows and so the user wouldn't know that on the back end they were still using the window system because each of the request was coming through the Unix cloud infructure again we were able to we were quickly able to tell leadership that the application was now being accessed through the cloud infrastructure and the remainder of the project was to migrate each piece of the Windows pro application into the cloud application and continuously adjusting the proxy rules so that it would point to the correct server eventually we were able to drop eventually when all of the features were built we moved over to the new cloud infrastructure we were able to remove turn off the Pearl application.


