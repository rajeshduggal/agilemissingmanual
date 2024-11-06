---
weight: 1
title: "Don't Get to Attached"
draft: true
---

# Don't Get to Attached

(show diagram of scooter to car... and point out that when it's time to build the peddles.. there are two routes that can be taken.

 One is to build a fancier and fancier bike.. with more and more improved pedals..
and the other is to remove the pedals completely and build a motorcycles.

So the key is to do the least possible. Don't spend time engineering super fancy pedals. Instead make basic high quality strong peddles. Maybe acquire peddles from a third party and put them in.. even if they aren't that great.  Just get something that works for now.  If the customer complains about them. Don't ignore them. Capture the complaints. And we can use that feedback.


Take all the complaints from the pedals. and then ask the customer...
Not that you've spent some time using the pedals.  Should we make the improved pedals...? This would be the ROI.  Or should we make a motorized scooter instead?


When building the pedals.. to do agile, its still important to build them in apartocular way.
you need to be aiming towards these things..
* Make it modular, so it can be removed.
* Make sure it's high quality. 
* Make sure other devs know what's going on with the code in case they are the ones that need to remove this feature.
* Try to keep as much of the code contained within a particular area as possible. Don't have bits and pieces of this code in some other external system, or some other application expecting it to be there.
* Make them so they can be added/removed easily.. i.e. modular. And 
* Keep it small and very high quality.
* Keep building unit tests, so that if this feature is removed or replaces with something else, another dev will still have "courage" that they aren't going to break the system.


And resisting doing these things..
* Making it feature rich and fancy.
* Trying to make everything super configurable. It's okay to hard code things sometimes, for the first iteration, and in a future iteration we can add some configuraiton. YAGNI
* Building what ever implementation the stakeholder has put in the user story. e.g. Understand what the user the is trying to trying to accomplish and even if the user story says to make pedals... think if something even smaller can be used instead.  And bring it to the attentoin of the BA/Product owner. Have a discussion and see, if there might something even simpler that will do for now.. and maybe once this is in production, pedals might work for the next iteration.
* Don't try and be hero with getting more code and elaborate feature intos in the system. Be a hero by spending your time and energy efficiently to provide the most ROI work (for the project as a whole) as possible, and also by finding ways to deliver smaller incremental pieces. So the product owner can try it out and quickly give feedback. Before delivering the next increment.



