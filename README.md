# Grove.io plugin for Jenkins - build-status placeholder

Started with a fork of the Slack plugin:

https://github.com/jenkinsci/slack-plugin

Which was a fork of the HipChat plugin:

https://github.com/jlewallen/jenkins-hipchat-plugin

Which was, in turn, a fork of the Campfire plugin.

# Jenkins Instructions

1. Get a Grove.io account: https://grove.io
2. Get a channel key for each of the channels you want to notify
3. Install this plugin on your Jenkins server
4. Configure it in your Jenkins job and **add it as a Post-build action**.

# Developer instructions

Install Maven and JDK.  This was last built with Maven 3.2.5 and OpenJDK
1.7.0\_75 on KUbuntu 15.04.

Run unit tests

    mvn test

Create an HPI file to install in Jenkins (HPI file will be in `target/slack.hpi`).

    mvn package

