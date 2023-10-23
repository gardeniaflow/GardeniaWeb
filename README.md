<!DOCTYPE html>
<html>
<head>
    <title>Your Web Chat</title>
    <!-- Include the Botpress Web Chat script -->
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
            "stylesheet": "https://webchat-styler-css.botpress.app/prod/code/193eecba-c426-41aa-bfcf-b81cb9f9131b/v76768/style.css",
            "avatarUrl": "https://i.postimg.cc/NMYxmYRP/image502-1695792437594.jpg",
            "botName": "Gardenia"
        });
    </script>
</body>
</html>
