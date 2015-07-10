---
layout: post
title:  "Broadcast protocol analysis during the 93rd IETF meeting in Prague" 
date:   2015-07-09
categories: projects
---
As [RFC919] notes: “The use of broadcasts, especially on high-speed local area networks, is a good base for many applications”. We would go even further saying that a number of functions are only implementable efficiently using IP broadcasts and an increasing number of application layer protocols make use of IP broadcasts.

This seems all good apart from the fact, that any device in the same broadcast domain will receive all these broadcasts, which means a passive observer will be able to collect the broadcast traffic of all members of the same broadcast domain. The interesting questions are a) what exactly are all these protocols sending out and b) can information from these protocols be combined and correlated to find out interesting things about devices, individuals and groups of individuals?

We have conducted a previous study in a large wireless network installation and found out that indeed there is a lot of interesting information to be gathered just by listening to broadcasts. This includes e.g. the language the owner speaks, his or her name, the users online times and social contacts with other users on the same network. In order to have a second data point, the exact same experiment will be conducted again during the 93rd IETF meeting in Prague.

All gathered data will be aggregated in statistics which will not reveal the identity of the network users. E.g. we will compute the average online time of people etc but not reveal these statistics for individual users. Once all the packet-level data has been analyzed, the traffic traces will be deleted for data privacy reasons.

All results of the study will be made available to the community.

Questions about this experiment? Contact us at <rolf.winter@hs-augsburg.de>. We’ll gladly answer all of your questions.

See you all in Prague!


[RFC919]: https://tools.ietf.org/html/rfc919 

