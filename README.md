Deploy APP

#Start the containers with:
docker-compose up  #if you using compose file for deployment


Navigate to your wiki server's IP address or hostname and complete the installation guide by clicking on the link.

Database Connection Details
The hardest part of the guide is filling in the database connection details. For the host you need to specify:db://localhost

The database user is wikiuser.

You will need to get the password from your docker-compose.yml file as set it to something random using a script above.

LocalSettings File
When you finish, you will automatically download a LocalSettings.php file. Copy the contents of this file. Then open up the editor to where the file needs to be and paste it:

sudo vim $HOME/volumes/mediawiki/LocalSettings.php
sudo chmod 755 $HOME/volumes/mediawiki/LocalSettings.php

Restart The Containers

MEDIAWIKI LIVE
