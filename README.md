# learner-project
An umbrella project that's used for learning and management of other projets in this organization.

## What are we trying to accomplish?

As stated in the projects description, the main goal is to have a project on which we can learn and demonstrate modern development principles.

Because coming up with examples over and over again is hard, these projects will be a good platform on which to demonstrate your knowledge, your examples, or just work on a product that might benefit you.
Given that CocoaHeads Slovenia holds regular meet-ups (and our members also give talks at other events), these projects will also be an easy platform to add example code to, further adding to the talks topics.

## What will it do?

We needed a fairly easy idea as a starting point, while having enough potential to expand on it, so we thought of time tracking / management.
Yes, it's been done before, yes, there are many projects that do this very well, we know all that.

That's the reason why this was such a good project to start with. We can borrow ideas from elsewhere, we know what we need / want from a project like this, and maybe most important: we can actually make use of a project like this, which will make adding to it that much more fun.

### Server side

The server side code is named [theClocker](https://github.com/cocoaheads-slovenija/theClocker) and is a [Vapor](https://vapor.codes) based project that allows users to register themselves, and provides a [RESTful](https://en.wikipedia.org/wiki/Representational_state_transfer) API to data stored on the server.

### Clients

[theClocker](https://github.com/cocoaheads-slovenija/theClocker) provides an API that may be consumed by various clients. We will start off with an iOS client and see from there.

* iOS client - [charge-oclock](https://github.com/cocoaheads-slovenija/charge-oclock)
* macOS Client - coming soon
* Web Client - maybe?

#### Other clients?

Sure, why not, contact us and we'll discuss it and if appropriate, create a new repo for it.

##### Even Android?

Of course!

## Functionality

The basic premise of the project is storing time spent on tasks. We'd like the tasks to be grouped by projects, with all data being linked to the user that created it.
Tasks should also be able to exist without being linked to a particular project.

It would be nice to have the option of adding tags to items, as well as charge information (charge per project, task type, ...)

Good examples of projects that already do this will are:

* [Toggl](https://toggl.com)
* [Hours](https://itunes.apple.com/app/hours-time-tracking/id895933956)

## Deployment

The server side code will be deployed to a server, and we may start charging for use of said server. The rate will be determined at a later time, but it should be noted that this is not intended to be a money making endeavour.
Any funds gained through this will go towards covering the cost of running the server, whatever is left goes towards funding the meet-ups we host.

This of course also means that the clients might be distributed through official channels (e.g. the app store for the iOS client).

The projects themselves will remain open source, of course, so if you do not wish to subscribe to a payed project, you don't have to, we will not hold this against anyone.