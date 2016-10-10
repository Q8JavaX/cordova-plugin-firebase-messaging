# cordova-plugin-firebase-messaging
> Cordova plugin for [Firebase Messaging](https://firebase.google.com/docs/cloud-messaging/)

## Installation

    cordova plugin add cordova-plugin-firebase-messaging --save

## Supported Platforms

- iOS
- Android

## Methods

### registerMessageReceiver(_callback_)
Called when a message is received.
```js
window.cordova.plugins.firebase.messaging.registerMessageReceiver(function(message) {
    console.log("Got a new message: ", message);
    });
```

### registerTokenReceiver(_callback_)
Logs an instance id token received.
```js
window.cordova.plugins.firebase.messaging.registerTokenReceiver(function(token) {
    console.log("Got device token: ", token);
    });
```

### subscribe(_topic_)
Subscribe to topic in background.
```js
window.cordova.plugins.firebase.messaging.subscribe("New Topic");
```

### unsubscribe(_topic_)
Unsubscribe from topic in background.
```js
window.cordova.plugins.firebase.messaging.unsubscribe("New Topic");
```
