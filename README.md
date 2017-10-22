# slackoncrash
Small Android library to send crash notificaiton of your app to slack channel

## Download Lib
https://www.dropbox.com/s/c3mlmsq11j35srp/slackoncrash-0.0.1.aar?dl=0

## How to use
Add following code to your application class
```
SlackOnCrash.install(getApplicationContext(),"Your Slack App Web hook");
SlackOnCrash.addProperty("AppName",getString(R.string.app_name),true);
SlackOnCrash.addProperty("AppId",BuildConfig.APPLICATION_ID,false);
//Here you can add properties to display in slack channel
SlackOnCrash.start();
//start can be called in application or in your main activity onresume
        
```

## What you will see in your channel
