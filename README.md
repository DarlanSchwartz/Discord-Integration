<img src="https://pbs.twimg.com/profile_images/1609033758497202176/7QBpkbA5_400x400.jpg" width="60px" heigth="60px" align="right"/> 

# Github Discord Integration 

If you want to integrate Discord with your GitHub repository, you can use Discord Webhook through your own server to send messages to a text channel in your Discord server. This is useful when you want to send messages to a Discord channel from your own server/website.

If you need to send your messages from your server/website to a Discord channel , checkout this [README_API.md](./README_API.md) for more.

## Steps

1. Create a text channel in your discord server.
2. Right click on the channel and go to `Edit Channel`.
3. Go to `Integrations` and click on `Create Webhook`.
4. Click on `Copy Webhook URL` and save it somewhere.

<img width="100%" align="center" src="./images/create_channel_and_webhook.gif"/>

5. Go to the repository where you want to integrate discord.
6. Go to `Settings` -> `Webhooks` -> `Add Webhook`.
7. Paste the copied webhook URL in the `Payload URL` field and add `/github` at the end of the URL.
8. Set the `Content type` to `application/json`.
9. In the `Which events would you like to trigger this webhook?` section, select the events you want to trigger the webhook.
10. Click on `Add Webhook`.
11. If everything is set up correctly, you will see a green ✔️ tick mark next to the webhook URL.

<img width="100%" align="center" src="./images/add_github_webhook.gif"/>


### Now, whenever the selected events occur in the repository, a message will be sent to the discord channel.

<div align="center">
    <img width="100%" src="./images/discord_message.gif"/>
    <img width="100%" src="./images/discord_message_2.gif"/>
    <img width="100%" src="./images/discord_messages_print.png"/>
</div>

