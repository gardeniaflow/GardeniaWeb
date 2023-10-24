<!DOCTYPE html>
<html>
<head>
    <title>Your Web Chat</title>
    <script src="https://cdn.botpress.cloud/webchat/v1/inject.js"></script>
</head>
<body>
    <!-- Add a container where you want the chat to appear -->
    <div id="botpress-webchat-container"></div>

    <!-- Initialize the Botpress Web Chat -->
    <script>
        window.botpressWebChat.init({
            "composerPlaceholder": "Start typing here",
            "botConversationDescription": "Your Property Partner",
            "botId": "204762d6-ce34-4c89-aec6-f4d659578fc5",
            "hostUrl": "https://cdn.botpress.cloud/webchat/v1",
            "messagingUrl": "https://messaging.botpress.cloud",
            "clientId": "204762d6-ce34-4c89-aec6-f4d659578fc5",
            "lazySocket": true,
            "frontendVersion": "v1",
            "enableConversationDeletion": true,
            "useSessionStorage": true,
            "avatarUrl": "https://i.postimg.cc/NMYxmYRP/image502-1695792437594.jpg",
            "stylesheet": "https://webchat-styler-css.botpress.app/prod/code/fba3b192-98e3-40ef-973e-0a1df8b3700a/v14867/style.css",
            "botName": "Gardenia"
        });
    </script>
</body>
</html>
