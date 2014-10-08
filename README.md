# To reproduce NSInternalInconsistencyException 'attempt to delete row 10 from section 0 which only contains 1 rows before the update'

Follow all ios setup and run the project. Also Publish more than 10 photo with your demo. After all of publishing 'load more' button is throwing the exception.

[parse \[PFQueryTableViewController loadNextPage\] bug report link](https://developers.facebook.com/bugs/821437467878353)

# Anypic

Anypic is the easiest way to share photos with your friends. Get the app and share your fun photos with the world. [Anypic](https://anypic.org) is fully powered by [Parse](https://parse.com). 

You can get the [source code](https://github.com/ParsePlatform/Anypic) and create your own Anypic with this [tutorial](https://parse.com/tutorials/anypic).


## iOS Setup

Anypic requires Xcode 5 and iOS 7. The [tutorial](https://parse.com/tutorials/anypic) provides additional setup instructions.

#### Setting up your Xcode project

1. Open the Xcode project at `Anypic-iOS/Anypic.xcodeproj`.

2. Create your Anypic App on [Parse](https://parse.com/apps).

3. Copy your new app's application id and client key into `AppDelegate.m`:

```objective-c
[Parse setApplicationId:@"APPLICATION_ID" clientKey:@"CLIENT_KEY];"
```

#### Configuring Anypic's Facebook integration

1. Set up a Facebook app at http://developers.facebook.com/apps

2. Set up a URL scheme for fbFACEBOOK_APP_ID, where FACEBOOK_APP_ID is your Facebook app's id. 

3. Add your Facebook app id to `Info.plist` in the `FacebookAppID` key.



[Orginal anyPic tutorial](https://parse.com/tutorials/anypic)