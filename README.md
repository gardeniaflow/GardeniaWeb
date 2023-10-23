<!DOCTYPE html>
<html>
<head>
    <title>Your Web Chat</title>
    <!-- Include the Botpress Web Chat script -->
    <script src="https://cdn.botpress.cloud/webchat/v1/inject.js"></script>

    <!-- Add custom CSS for your chat container -->
    <style>
        #botpress-webchat-container {
            margin: 10px;
            background: #66ba69;
            border-radius: 10px;
            position: relative;
            overflow: hidden;
            border: 1px solid #66ba69;
            color: #ffffff;
        }

        /* Styling for the chat bubble content when it's from the user */
        .bpw-from-user .bpw-chat-bubble .bpw-chat-bubble-content {
            background-color: #66ba69;
            color: #ffffff;
        }
    </style>
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
            "botName": "Gardenia"
        });
    </script>
</body>
</html>
