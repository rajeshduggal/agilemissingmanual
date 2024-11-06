---
weight: 1
title: "Quality is a Variable"
draft: true
---

# Quality is a Variable (The elephant in the room)

No one seems to be talking about how quality is a variable.

It's a taboo topic. Management seem to just assume that the implementation team knows they need to do everything at high quality.

And the development team use the quality variable as a way to give themselves a bit of emergency buffer to squeeze work that ends up taking them more than they thought. If they get stuck along the way, and they only have a day or two left to finish the work, and they know they won't get it all done, then they just reduce the quality a little bit and usually no notices. (Sometimes other devs notice, when they're doing code review. But they also know that this code needs to go into the next production release in a few days time. So they let is slide. "It's good enough").  Maybe it is, or maybe it isn't.  But the thing is that this is all just under the radar.. and slowly over time it can make the software more kludgy and difficult to keep building on (refactoring is always postponed again and again, and so the software becomes harder and harder to maintain and update). They just keep adding one more "if" statement to the code, or one more attribute to the class. Instead of refactoring and re-organizing the code in a way that makes it easier to work with.

It's interesting to ask developers, if you had a week to refactoring the code, what do you think would give the most ROI, so that the code would be easier for others to understand, and work with. Or what would reduce the chance of bugs leaking through the system.

The more pressure that has been put on the devs to reach tight time lines the more things the dev will be able to point out.  And so it's interesting. Because the devs are smart, they know what the code should look like.  But because of timeline pressures they haven't been able to refactor the code and keep the quality high.

Sometimes I've seen teams add user stories to "refactor the code" or "Fix on technical debt", so that the devs have an opportunity to do some clean up.  But of course this doesn't make sense, because the user stories should be owned by the product owners, and they should be something that the product owners understands and are asking for themselves. And should be scheduling and prioritizing against the other stories in the backlog.

----

Ask the developers in your team how common they think this scenerio is.

The developer has to write some code to make a http call to an external service to retrieve some information and present it to the user and save it to the database. As they're thinking through the work. They realize that there are many alternate and extension flows that can happen, and should be accounted for in the code.
* The network is down, and so the server code should queue the request and try to get it later, so it can be stored in the db.
* The http request takes a long time, and the user hit stop their browser, and made the request again. And now multiple, long-running requests for the same data are being executed at the same time.
* There was a response from the API saying that the data isn't availabe right now, try again later.
* There was a response from the API saying that the data isn't availabe and never will be. So we shouldn't try the same request again.
* There API server said there was an error with the request.
* The data was retrieved from the server, but it wasn't within the expected format.  Perhaps we were expecting a number but got a blank. Or perhaps some text was returned.
* The local database was down.
* The local database is running, but there was an error in saving the data.  And it should be tried again later.
* The local database is running, but there was an error in saving the data because the data was in the wrong format. Perhaps the database field stores a number, but we're trying to save text. Or perhaps the text is too long and needs to be truncated before it can be saved.
* There are many other possible scenarios that aren't the happy path.

The developer may be aware of all of these different scenarios, and was planning on coding for them.  However, the schedule says that this is due tomorrow.  And so instead of handling these various scenarios, developer just writes an error to the log file. And just has and error page appear the end user's browser.  This can be tested by QA and they see the correct data in the browser, because the network, database and API are all currently up and running, and the request we're making for the test is a simple straight forward typical request that is very very likely to just work.  And the stakeholders see this code working too and gives a thumbs up.  Meanwhile, the developer secretely knows that they didn't handle all of the other flows properly and just keeps quiet about it. No one else is the wiser!

What's happened here? Simple... The developer lowered the quality of the code to be able to get the work completed in time for tomorrow's due date. It all seems to be  working fine.


