# macos_syncronizer
yet another syncronization tool for macos

Simple shell sync script based on rsync.

Easy for sync Desktop, Thunderbird and Firefox between diferent macs.

Our environment has no NFS, only SMB v.3 and higher. Macos had still problems to automount this sort of shares. Whithout mounting a share, it is no posible to use it for User-Profiles when the user is loged. Because of this, i teach each user to use the share (after a clic there it is mounted without problems) but sometimes, they forget it.

Special problematic for us are: Desktop and Mozilla Apps Thunderbird and Firefox (in local user profile too). The first because is too easy to live something ther, the another both, because there data is in ~/Library.  This Script lose these problems for login in a login-item and for each another times, you can put it in a crontab job, for each 5 or 10 min. or maybe with offset-tool, because it is no more a easy way to put scripts at the logout.

Of course a syncronization for a IMAP folder is not necesary, because of them is out.

The problem is still worse if you want to sync two o more computers by mobile users in diferents workplaces. The macos_syncronizer is directional, also it work in a way other another, but not both. It no delete, if you want this you need to put --delete at the end of rsyc commands. Easy for security reasons, it is not hard to convert it in bidirecctional and/or deleted, but so -i think- you have better control.

And of course: this ist not a good way, if you want to have a good solution for some problems, you need to deploy a NFS Share. Buy maybe, you need -like me- some dirty-scripts for a short time too. I hope it help you!
