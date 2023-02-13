# MMDVM_groupsrewrite
Pistar-Update pulls in and generates a groups.txt file from BrandMeister only
this adds other DMR networks to the groups.txt file and prepends 
the network name so that the group name will show up for all the 
networks you're connected to in a multi-network system

Just put the .service file in /etc/systemd/system/ and enable it and start it, 
and GroupsRewrite will happily sleep in the background, checking
the groupts.txt file every 10 minutes to see if its modified timestamp has changed 
indicating the file was modified by an update, in which case GroupsRewrite
will awaken and complete the rewrite of the file, and then go back to sleep

This was developed for my own use, so I only utilized the 5 networks
I connect to.   Feel free to change it to suit your needs.  
the code is pretty self explanatory, but if you have questions
I can be reached at john at wa1okb.radio
