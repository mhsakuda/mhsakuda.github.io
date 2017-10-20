---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-10-19
labels:
  - Software Engineering
  - Meteor
  - Windows 10
  - Troubleshooting
---

<img class="ui large centered image" src="../images/meteor.png">

Using Meteor has been an interesting experience so far for developing our Digits application. The first major issue that I encountered was the initial set-up and installation of Meteor on Windows 10. There were times where -meteor run would not work, the localhost site would not refresh properly when changes were made to files on IntelliJ and the site would crash, and issues where Meteor would take too long to startup. I read through the Meteor tips and tricks in the Meteor module and discovered that Windows Defender could be the source of my problems with Meteor runtime, as it scans all the files when building the application. Sure enough, after disabling Windows Defender, I had no issues with the initial startup or while running Meteor. For future applications, disabling Windows Defender is a must. Second, I did a clean re-installation of Meteor and MongoDB to make sure there weren't any corrupt files that were causing issues. After performing these two actions, I can say that Meteor hasn't been giving me any issues starting up or building the application.

Another issue I encountered was during the actual development of the Digits application. My contact list was not showing up on the home page despite creating a contacts list in the database and linking it with the html files. I watched though the WOD video again and then double checked to make sure that I created and formatted all of the pages correctly. It turns out that I had capitalized a contact list variable in one of the files, and the variable that I was trying to call did not exist, and therefore a blank list was being displayed. The lesson learned was to make sure to double check all variable names and make sure that they are being called properly when needed.
