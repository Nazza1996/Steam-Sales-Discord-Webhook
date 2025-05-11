# Steam Sales Discord Webhook

This simple Docker Compose setup runs a script that checks for Steam games on sale and sends a message of them to a sepcified Discord webhook.

## Set Up
Before running the script, you will need to create a webhook in your discord server and point it to a channel of your choice. 
Then update the ```docker-compose.yml``` file with the following values:
```
WEBHOOK_URL= # the url of your discord webhook
POLLING_INTERVAL= # how often the script should check for new games in hours
```
Finally, to build and run the container:
```
docker compose up -d
```
This will build and start the Docker container, and start sending messages in discord. There will be alot of messages at first as there are a lot of offers to get through at the start.

