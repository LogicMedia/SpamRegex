# SpamRegex
Regular Expression set to help identify web contact form spam

This is a collection of regular expressions to help identify spam that is submitted on web forms. Each regular expression has an optional "weight" at the end, after a "#". This is an integer that is added to the total spam score. After a certain threshold, you may want to consider the message spam and automatically discard it. Default weight is +1 if no weight is specified.

Negative weights are to help reduce this effect. Local phone numbers, for example, have a negative weight in my instance. 

Strings of capital and lowercase letters (e.g. xjDsXrFzF) match a spam pattern, but some surnames, such as McAdams, do as well, so there is a negative weighted pattern for that.

My use case is specifically english-only, so the entire cyrillic alphabet is included in a pattern, as are many other non-english letters. The patterns in this file are from actual spam. This is all extremely specific to my use case. This may not be your use case, so modify accordingly.

