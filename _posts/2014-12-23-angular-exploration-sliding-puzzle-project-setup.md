

---
layout: post
title: "Sliding puzzle project setup"
description: "Frontend project setup"
category: angular
tags: [angular,phonegap,yeoman]
---
{% include JB/setup %}

To start the project I created a Phonegap project and used the mobileangularui yeoman generator. To create a Phonegap project based on Mobile Angular UI I followed the steps as outlined in the excellent post <href a="http://mobileangularui.com/blog/your-first-phonegap-app-with-mobile-angular-ui/">Your first Phonegap App with Mobile Angular Ui</a>

Install the required tools:
npm install -g bower 
npm install -g yo 
npm install -g gulp 
npm install -g generator-mobileangularui 
npm install -g phonegap

To scaffold the project a yeoman (http://yeoman.io/) generator can be used. A yeoman generator is just a plugin that can be run with the `yo` command to scaffold the project.

Create Phonegap project:
phonegap create swiped
cd swiped

Scaffold the project: yo mobileangularui

Build the project: gulp build

Run the Android version of the app: phonegap run android

Test in a web browser: gulp
