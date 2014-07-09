---
layout: post
title: "Builder pattern"
description: "Testing with the builder pattern"
category: dependency injection
tags: [builder pattern, mockito, unit testing]
---
{% include JB/setup %}

To build clean and expressive unit tests I have been using the Builder pattern lately. I like to keep the tests clean and readable and this is exactly what the Builder pattern allows me to do.

The unit test below has two tests, one with the default values as defined in the builder class and one with (some) values set using the with* methods. 

<script src="https://github.com/wwillems/techlogprojects/blob/master/builder-pattern/src/main/java/org/ts/patterns/Product.java"></script>

<script src="https://github.com/wwillems/techlogprojects/blob/master/builder-pattern/src/main/java/org/ts/patterns/ProductBuilder.java"></script>

<script src="https://github.com/wwillems/techlogprojects/blob/master/builder-pattern/src/test/java/org/ts/patterns/ProductTest.java"></script>

