# hubot-rocketchat
hubot-rocketchat for docker


Utilisation :

docker run -it -e ROCKETCHAT_URL=<your rocketchat instance>:<port> \
    -e ROCKETCHAT_ROOM='' \
    -e LISTEN_ON_ALL_PUBLIC=true \
    -e ROCKETCHAT_USER=bot \
    -e ROCKETCHAT_PASSWORD=bot \
    -e ROCKETCHAT_AUTH=password \
    -e BOT_NAME=bot \
    -e EXTERNAL_SCRIPTS=hubot-pugme,hubot-help \
    -v $PWD:/home/hubot/node_modules/hubot-rocketchat hihouhou/hubot-rocketchat

docker run --link rocketchat:rocketchat -e ROCKETCHAT_URL=rocketchat:3000 \
    -e ROCKETCHAT_ROOM='' \
    -e LISTEN_ON_ALL_PUBLIC=true \
    -e ROCKETCHAT_USER=bot \
    -e ROCKETCHAT_PASSWORD=bot \
    -e ROCKETCHAT_AUTH=password \
    -e BOT_NAME=bot \
    -e EXTERNAL_SCRIPTS=hubot-pugme,hubot-help \
    -v $PWD:/home/hubot/node_modules/hubot-rocketchat hihouhou/hubot-rocketchat


