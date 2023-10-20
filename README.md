<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gardenia</title>
    <style>
        /* Set the maximum width and height for the chatbot container */
        .chatbot-container {
            max-width: 400px; /* Adjust the maximum width as needed */
            max-height: 200px; /* Adjust the maximum height as needed */
            margin: 0 auto; /* Center the container horizontally */
            overflow: auto; /* Add scrollbar when content overflows */
        }
    </style>
</head>
<body>
    <!-- Add a container div for the chatbot with a unique ID -->
    <div id="chatbot-container" class="chatbot-container">
        <!-- JavaScript to load the chatbot asynchronously -->
        <script>
            function loadChatbotScript() {
                var script = document.createElement('script');
                script.src = 'https://cdn.botpress.cloud/webchat/v0/inject.js';
                script.async = true;
                document.getElementById('chatbot-container').appendChild(script);

                script.onload = function () {
                    window.botpressWebChat.init({
                        "botId": "204762d6-ce34-4c89-aec6-f4d659578fc5",
                        "clientId": "204762d6-ce34-4c89-aec6-f4d659578fc5",
                        "hostUrl": "https://cdn.botpress.cloud/webchat/v0",
                        "messagingUrl": "https://messaging.botpress.cloud",
                        "botName": "Gardenia",
                        "avatarUrl": "https://i.postimg.cc/NMYxmYRP/image502-1695792437594.jpg",
                        "composerPlaceholder": "Start typing here",
                        "botConversationDescription": "Your Property Partner",
                        "hideWidget": true,
                        "stylesheet": "https://webchat-styler-css.botpress.app/prod/code/193eecba-c426-41aa-bfcf-b81cb9f9131b/v53044/style.css",
                        "disableAnimations": true,
                        "lazySocket": false,
                        "useSessionStorage": true,
                        "frontendVersion": "v1",
                        "enableConversationDeletion": true
                    });
                    window.botpressWebChat.onEvent(function () {
                        window.botpressWebChat.sendEvent({ type: 'show' });
                    }, ['LIFECYCLE.LOADED']);
                };
            }

            // Call the function to load the chatbot script
            loadChatbotScript();
        </script>
    </div>
</body>
</html>

