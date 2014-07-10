---
layout: post
title: "Builder pattern"
description: "Testing with the builder pattern"
category: dependency injection
tags: [builder pattern, mockito, unit testing]
---
{% include JB/setup %}

To build clean and expressive unit tests I have been using the Builder pattern lately. I like to keep the tests clean and readable and this is exactly what the Builder pattern allows me to do.

The Product class below has a couple of attributes that get set via setters and one calculated value based on the values of the other attributes.

<script src="https://gist.github.com/wwillems/b6e847925bb82d13cfbe.js"></script>

The ProductBuilder class builds products using default values and exposes with* methods to set individual product attributes.

<script src="https://gist.github.com/wwillems/4dd90db4896940fdb0d7.js"></script>

The unit test below has two tests, one with the default values as defined in the builder class and one with (some) values set using the with* methods. 

<script src="https://gist.github.com/wwillems/3058ab7602fc923e5bb2.js"></script>

