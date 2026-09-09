# Nathans-IT-Lab
Hands on IT/help desk lab work, AD, Azure, Ticketing practice
## Fixing Misplaced AD Groups

While setting up department-level Security groups (IT, Accounting, HR, Sales, Management) 
for the USA OU, I initially created them under the wrong container — Servers instead of 
Users. Rather than recreating the groups (not possible anyway, since AD group names must 
be unique domain-wide), I selected the affected groups in Active Directory Users and 
Computers and used the Move function to relocate them to the correct Users OU, preserving 
their names, settings, and time.
![OU structure](01-OU-Structure-region.png)
*Regional OU structure (USA, Europe, Asia) *
![Groups misplaced](02-USA-groups-misplaced-under-servers-OU.png)
*Groups mistakenly created under the Servers OU instead of Users*
![Servers department highlight](03-USA-groups-servers-department-higlight.png)
*Identifying the misplaced groups under Servers*
![Selecting and moving](04-USA-groups-users-select-move.png)
*Selecting the groups and using the Move function*
![Final result](05-USA-groups-users-positioned.png)
*Final result — groups correctly positioned under the Users OU*
