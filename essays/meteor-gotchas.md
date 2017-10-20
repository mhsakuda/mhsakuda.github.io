---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-10-19
labels:
  - Software Engineering
  - Meteor
---

<img class="ui medium left floated image" src="../images/meteor.png">

Using Meteor has been an interesting experience so far for developing our Digits application. The first major issue that I encountered was the initial set-up and installation of Meteor. There was times where -meteor run would not work, the localhost site would not refresh properly and would therefore crash, and issues where Meteor would take too long to startup. I read through the Meteor tips and tricks and discovered that Windows Defender was the problem with Meteor runtime, as it scans all the files when building the application. For future applications, disabling Windows Defender is a must. Second, I did a clean re-installation of Meteor and MongoDB to make sure there weren't any corrupt files that were causing issues. After performing these two actions, I can say that Meteor hasn't been giving me any issues starting up or building the application.

Another issue I encountered was during the actual development of the Digits application. My contact list was not showing up on the home page despite creating a contacts list in the database and linking up with the html files. It turns out that I had capitalized a variable in one of the files, and that's why it was displaying nothing on the main page. A lesson learned was to make sure to double check all variable names and make sure that they are being called properly when needed.
