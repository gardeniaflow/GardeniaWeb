<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gardenia</title>
</head>
<body>
    <!-- JavaScript to load the chatbot asynchronously -->
    <script>
        function loadChatbotScript() {
            var script = document.createElement('script');
            script.src = 'https://cdn.botpress.cloud/webchat/v1/inject.js'; // Using v1
            script.async = true;
            document.body.appendChild(script);

            script.onload = function () {
                window.botpressWebChat.init({
                    "botId": "0e30855c-6873-4f87-9de6-b3352a0622b3", // Bot ID from the first script
                    "clientId": "0e30855c-6873-4f87-9de6-b3352a0622b3", // Client ID from the first script
                    "hostUrl": "https://cdn.botpress.cloud/webchat/v1",
                    "messagingUrl": "https://messaging.botpress.cloud",
                    "composerPlaceholder": "Start typing here",
                    "botConversationDescription": "Your Property Partner",
                    "hideWidget": true,
                    "disableAnimations": true,
                    "enableConversationDeletion": true,
                    "botName": "Gardenia", // Add botName
                    "avatarUrl": "https://i.postimg.cc/YC8DyGW1/Screenshot-2023-09-13-213012.jpg", // Add avatarUrl
                    "containerWidth": "100%25", // Add containerWidth
                    "layoutWidth": "100%25", // Add layoutWidth
                });

                window.botpressWebChat.onEvent(function () {
                    window.botpressWebChat.sendEvent({ type: 'show' });
                }, ['LIFECYCLE.LOADED']);
            };
        }

        // Call the function to load the chatbot script
        loadChatbotScript();
    </script>
</body>
</html>
