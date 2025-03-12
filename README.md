#n8n with PostgreSQL locally
Starts n8n with PostgreSQL as database.

Start
To start n8n with PostgreSQL simply start docker-compose by executing the following command in the current folder.
docker-compose up -d

IMPORTANT: But before you do that change the default users and passwords in the .env file!

To stop it execute:
docker-compose stop

Configuration
The default name of the database, user and password for PostgreSQL can be changed in the .env file in the current directory.

Make sure the init-data.sh file has the correct permissions:
chmod +x init-data.sh

# n8n-render

Successfull installation of n8n on Render using Docker.

To make it run just open Render Dashboard and use this git as Blueprint.

Important note if using disk on Render: Keep the mountPath as is, otherwise n8n won't change the data.

The .env file contain examples of lines that can be added manually on Environment Variables on Render after install.

To change the webhook URL from localhost to your domain, for example, just add the var WEBHOOK_URL followed by the full URL.

Version 0.224.1
