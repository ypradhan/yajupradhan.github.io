---
layout: post
title:  "Keyword Based Acceptance Test Framework"
date:   2015-08-29 23:56:45
description: Just a sample post to show some of the typography elements supported from harmony theme.
categories:
- blog
permalink: first-post
---
__Hello there. There are more than dozens of tools that I have been looking into that support automation by selenium webdriver. Each language has its own test tools and a plethora of frameworks that help to write these test. A look at the automation pyramid help us see that the best way to move forward is have a minimal amount of these tests and closely interacting how user would interact. The choice to make when choosing the tools is still a hard one to make. 
_

A blockquote:

> A year from now you may wish you had started today. 
> - By Karen Lamb


Hello there. There are more than dozens of tools that I have been looking into that support automation by selenium webdriver. Each language has its own test tools and a plethora of frameworks that help to write these test. A look at the automation pyramid help us see that the best way to move forward is have a minimal amount of these tests and closely interacting how user would interact. The choice to make when choosing the tools is still a hard one to make. 

The first and the easiest one to start off with is the IDE itself. It is pretty basic and anyone with knack for working with web application can learn it in hours, the tool that is. But, today I will be talking about selenium webdriver and a tools I have looked into. Robotframework is an acceptance test framework. It has the easy of the IDE for any non technical user, who can start off quickly. It is written in python and is a simple keyowork based frameowork with an IDE that supports help for each keywork they supports. There is even a tool called [FireRobot](https://github.com/joao-carloto/FireRobot) that make creating the test scripts as easy as Selenium IDE.

Example code:
 {% highlight robotframework%}

*** Settings ***
Documentation  Generic Selenium2Library resources keywords
Library        Selenium2Library

*** Test Cases ***
Test Home Page Open
    Open browser
    Home Page Should Be Open  Grasshopper

*** Keywords ***
Open browser   ${URL}    ${BROWSER}    


Home Page Should Be Open
    [Arguments]  ${_title}
    Title Should Be    ${_title}
{% endhighlight %}



