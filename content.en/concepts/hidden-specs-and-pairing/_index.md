---
weight: 1
title: "Hidden Specs and Pairing"
draft: true
---

# Hidden Specs and Pairing

I remember working on software development projects before user stories existed. The team would work on writing up verbose "use cases" and some would take up a 2 or 3 pages.
Detailing all the alternative and extension flows.  And even then the use cases wouldnt be complete. Even though we tried to complete them all before starting the "development phase". We would need them so we could estimate them and put them into the schedule. So we would track if we're in-front of, or behind schedule to get the final software deployed into production.

Sometimes an external vendor would be hired to spec out and write all the use cases, and design/architect the entire system.  And once they delivered this spec bookelet. We weren't suppose to change any of it.  Or if we did, it had to go through a change control process. To cost it out and do an impact analysis.

The reality is that as we're thinking about or working on the feature, we're realizing things that need to be accounted for and built to make the feature work. The list of things needed can keep growing and growing with more and more details for some time, while we're in the middle of the implementation.

There are many things which the implementors already know need to happen for the feature to work: e.g.
* What to do if the database is down.
* What to do if the user's name is very long and doesn't fit in the small window on the user's cell phone screen.
* What to do if the network connectivity to the external API is down.
* What to do if the user's uploaded image is too large.
etc, etc.  And they may document 


When I started to see User Stories first introduced into projects that had always been doing detailed use cases, it was difficult for many people to grasp. It felt like a step backwards for many of them. It didn't seem right to forego capturing all these important details. and instead to just write a few sentences as a user story.

