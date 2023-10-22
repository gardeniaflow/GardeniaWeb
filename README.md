<!DOCTYPE html>
<html>
</style></head>
<body>
  <div id="botpress-webchat-container"></div>
  <script src="https://cdn.botpress.cloud/webchat/v0/inject.js"></script>
  <script>
    window.botpressWebChat.init({
      "botId": "204762d6-ce34-4c89-aec6-f4d659578fc5",
      "clientId": "204762d6-ce34-4c89-aec6-f4d659578fc5",
      "hostUrl": "https://cdn.botpress.cloud/webchat/v0",
      "messagingUrl": "https://messaging.botpress.cloud",
      "botName": "Gardenia",
      "avatarUrl": "https://i.postimg.cc/NMYxmYRP/image502-1695792437594.jpg",
      "containerWidth": "100%25",
      "layoutWidth": "100%25",
      "composerPlaceholder": "Start typing here",
      "botConversationDescription": "Your Property Partner",
      "hideWidget": true,
      "disableAnimations": true,
      "stylesheet": "https://webchat-styler-css.botpress.app/prod/code/5ce2b2c8-4482-424a-8e12-ad6bba19692c/v62394/style.css",
      "enableConversationDeletion": true
    });

    window.botpressWebChat.onEvent(function () {
      window.botpressWebChat.sendEvent({ type: "show" });
    }, ["LIFECYCLE.LOADED"]);
  </script>
</body>
</html>
