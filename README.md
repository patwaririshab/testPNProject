# testPNProject

This project was created to find out the required JSON Payload to be sent through Apple Push Notifications as well as the
required implementation in code.

In order to use this project you will need:
- Xcode 11.4 beta 2

Reference:
- https://www.raywenderlich.com/8164-push-notifications-tutorial-getting-started

Setting up local push notifications in Xcode 11.4 beta 2:
- https://medium.com/swlh/simulating-push-notifications-in-ios-simulator-9e5198bed4a4

This is the sample payload that worked
```
{
    "Simulator Target Bundle": "com.razeware.WenderCast",
    "aps": {
      "alert": "New Posts!",
      "sound": "default",
      "link_url": "https://raywenderlich.com",
      "category": "VIEW_IDENTIFIER"
    }
}
```

## How to test
1. Build and run project in Xcode 11.4 beta 2
2. In an editor, copy and paste the sample JSON Payload above, then save as `.apns` file
3. Drag and drop the sample JSON Payload into your simulator when app is NOT in the foreground


