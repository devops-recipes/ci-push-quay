# Docker Build, Push and Continuous Integration for a Node JS application

[![Run Status](https://api.shippable.com/projects/5900754c614d120700088a0d/badge?branch=master)](https://app.shippable.com/github/himanshu0503/ci-push-quay) [![Coverage Badge](https://api.shippable.com/projects/5900754c614d120700088a0d/coverageBadge?branch=master)](https://app.shippable.com/github/himanshu0503/ci-push-quay)

![AyeAye](https://github.com/devops-recipes/ci-push-quay/blob/master/public/resources/images/captain.png)

A simple Node JS application with unit tests and coverage reports using mocha
and istanbul. It also does a docker build once CI posses and then pushes the image
to Quay

## Run CI for this repo on Shippable
* Fork this repo into your local repo
* Login into the [Continuous Integration Service](https://app.shippable.com)
* Create a Quay [integration](http://docs.shippable.com/integrations/imageRegistries/quay/) on shippable to connect your Quay.io account
* All CI configuration is in `shippable.yml`
* Follow these [CI Setup Instructions](http://docs.shippable.com/ci/runFirstBuild/) if you have never used Shippable CI Service
* Update the integrationName in the integration.hub section if you used something other than `quay-integration`
* Change the IMAGE_REPO and QUAY_ORGANIZATION to point to your repo and Quay organization
* You should be able to run a manual build or webhook build on commit

## CI Reports on Shippable

### CI Integration View
![CI Integration View](https://github.com/devops-recipes/ci-push-quay/blob/master/public/resources/images/integration.png)

### CI Console Output
![CI Console Output](https://github.com/devops-recipes/ci-push-quay/blob/master/public/resources/images/console.png)
