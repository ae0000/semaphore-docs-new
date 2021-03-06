---
layout: post
title: Building pull requests
category: Getting started
---

Semaphore supports building pull requests from forked repositories for projects
hosted on GitHub. Every time a new pull request is opened, Semaphore creates
a new branch whose name matches the pull request title and number.

<img src="/docs/assets/img/building-pull-requests/pull-requests.png" class="img-responsive">

For each new pull request update, Semaphore checks if the pull request can
be merged. If it can, it runs a new build of the merged version of the code and
pushes the commit status after the build has completed. If the pull request
can't be merged, Semaphore does not initiate a new build.

Since Semaphore automatically builds branches that are created within a
repository, it doesn't support building pull requests that are opened within the
same repository.

Because of technical limitations of its API, Semaphore does not support building
pull requests for projects that are hosted on Bitbucket.
