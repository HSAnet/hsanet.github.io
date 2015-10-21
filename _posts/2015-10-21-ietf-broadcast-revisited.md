---
layout: post
title:  "Broadcast/Multicast analysis at the next IETF meeting...likely" 
date:   2015-10-21
categories: projects
---
At the last IETF meeting in Prague, we wanted to do an analysis of broadcast/multicast
traffic. This was unfortunately cancelled, 
but there were valid concerns of meeting
participants and legal uncertainty of whether this would actually be allowed
according to local law. This gave us some time to consult with lawyers and to 
work on our software that performs the analysis and we believe that all previous
concerns have been addressed.

What we plan to do is to passively collect the broadcast and multicast data that
is sent over the meeting Wifi, i.e. the data that every device on the network
receives. The primary concern that was raised was the potential handling of personally identifiable
information. And indeed some protocols include the hostname of devices and as it turns
out, a lot of hostnames contain information such as the device owner's name, the language
he or she speaks and other information device owners might make part of their devices' names.
In order to address this problem, we will use a piece of software that securely
hashes MAC addresses and IP addresses before we start our analysis.
In addition, it will tokenize protocol fields that might
contain hostnames and hash the resulting tokens securely as well. This make
analysis more difficult, a lot of information is lost, but the experiment is still
interesting enough to go ahead with it. 

We also wrote an [Internet draft] which expresses our concern with current use
of broadcast and multicast messages which is why we do this experiment in the
first place.

Questions about this experiment? Contact us at <rolf.winter@hs-augsburg.de>. We’ll gladly answer all of your questions.

See you all in Yokohama!

[Internet draft]: https://tools.ietf.org/html/draft-winfaa-broadcast-consider-01

