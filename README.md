<html lang="en">
<body>
    <!-- JavaScript to load the chatbot asynchronously -->
    <script>
        function loadChatbotScript() {
            var script = document.createElement('script');
            script.src = 'https://cdn.botpress.cloud/webchat/v1/inject.js';
            script.async = true;
            document.body.appendChild(script);

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
                    "stylesheet": "https://webchat-styler-css.botpress.app/prod/code/5ce2b2c8-4482-424a-8e12-ad6bba19692c/v62394/style.css",
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
</body>
</html>
