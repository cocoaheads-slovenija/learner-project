# How to contribute

Third party contributions are essential for keeping these projects great. We can't handle all the changes required to keep up with the iOS SDK development over time. We want to keep it as easy as possible to contribute changes that make the projects better suited for both your needs as well as current development principles.
There are a few guidelines that we need contributors to follow so that we may have a chance of keeping on top of things.

## Licence

Please note that if you contribute work to any of these project, you agree that your contributions will fall under the projects licence. The licence may be found in the `LICENCE` file.

## External frameworks

Since these projects are meant as learning projects, we tend not to use third party frameworks. Apples SDKs are feature complete and provide all that is needed for development.
That said, in an production environment it might make sense to use third party code, but in these projects that will not be allowed.

## Dependency managers

Since we don't use third party frameworks, no dependency managers will be used.

The only exception to this is [theClocker](https://github.com/cocoaheads-slovenija/theClocker), which is a Vapor based server side project. It used the Swift Package Manager, so we're sticking with that. Additional third-party frameworks are frowned upon in that project as well, though.

## I still want to contribute

That's great, we're glad and thankful. A few steps to get you started (you've taken care of most of these? even better):

* Make sure you have a [Github account](https://github.com)
* [Fork](https://help.github.com/articles/fork-a-repo/) the repo you wish to work on
  Alternatively you can also work on the main repo if you're a member of our Team. This is managed through our [slack team](https://github.com/cocoaheads-slovenija/learner-project/issues/1)
* Submit a ticket (on the repo, not your fork) for your issue, assuming one does not already exist.
  * Clearly describe the issue including steps to reproduce when it is a bug.
  * Make sure you fill in the earliest version that you know has the issue.
  * If it's a feature / enhancement / ..., clearly describe what you plan to do and how. 

## Making changes

* Create a topic branch from where you want to base your work.
  * This is usually the master branch.
  * Only target release branches if you're certain your fix must be on that branch.
  * Please avoid working directly on the `master` branch. (you will not be able to push changes to the repo)
* Make commits of logical units
* Check for unnecessary whitespace with `git diff --check` before committing.
* Make sure your commit messages are in the proper format.
  First line should be a short description, including a link back to the issue it addresses. (github allows for a shorthand using a hash character and the issue number. e.g. #42 )
* Make sure you have added the necessary tests for your changes. (where appropriate)
* Run *all* the tests to assure nothing else was accidentally broken.

## Making trivial changes

### Documentation

For changes of a trivial nature to comments and documentation, it is not always necessary to create a new issue. In this case it's appropriate to leave out a link to an issue in the commit message.

## Submitting changes

* Make sure your contributions may be distributed under the projects licence.
* Push your changes to a topic branch in your fork of the repository.
  Alternatively, use a topic branch on the main repository.
* Submit a pull request to the repository in the [CocoaHeads Slovenija](https://github.com/cocoaheads-slovenija) organization. Include a request for review with the PR.
* After the core team approves the PR (which might include required changes), your contribution will be merged into the repository and the issue closed.

## Revert policy

By running tests in advance and by engaging with peer review for prospective changes, your contributions have a high probability of becoming long lived parts of the project. Should your code change results in a test failure, however, we will make our best effort to correct the error. If a fix cannot be determined and committed within 24 hours of its discovery, the commit(s) responsible *may* be reverted, at the discretion of the committer and/or maintainers.

### **Summary**

Changes resulting in test failures will be reverted if they cannot be resolved within one business day.

## Releases / branch flow

All development is done on the `master` branch. When we decide to do a release, a release branch is created, the release stabilised on it (work on `master` may continue without interference), when the release is ready, the branch is tagged, merged back to `master` and deleted.

This means that the only long-lived branch is `master`.

### Bug fixes

Should a bug fix be needed for a particular release, a bug fix branch is created from the appropriate release tag, fixes applied, the branch is tagged (before releasing the bug fixes) and merged to master, after which it is deleted.

