# macos_syncronizer
yet another syncronization tools for macos

Simple shell sync script based on rsync. 

Our environment has no NFS only SMB v.3 and higher. Macos had still problems to automount this sort of shares. Whithout mounting a share, it is no posible to use it for User-Profiles. Because of them, i teach each user to use the share (after clic is mounted) but sometimes, they forget it.

Special problematic are: Desktop and Mozilla Apps (in local user profile too). This Script lose the problem for login, and for each time, you can put it in a crontab job, for each 5 or 10 min. because it is no more easy posible to put al logout.

The problem is still worse if you want to sync two o more computers by mobile users in diferents workplaces. The my macos_syncronizer is directional, also it work in a way other another, but not both. It no delete, if you want this you need to put --delete at the end of rsyc commands.

And of course: this ist not a good way, if you want to have a good solution for some problems, you need to deploy a NFS Share. Buy maybe, you need some dirty-scripst for a short time too. I hope it help you!
