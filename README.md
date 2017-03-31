## Checklist

Make sure you've done the following before trying to submit to test flight or the app store:

* Your app works and doesn't crash.
* Your app has all of it's icons. You can use a service like <https://makeappicon.com> to generate all the different sizes.

## Create Certificate

If you've already created an Ad Hoc Production certificate, continue on to the next section.

* Select `All` under the `Certificates` menu on the left.
* Click on the plus button at the top right corner.
* Select `App Store and Ad Hoc` under `Production` and click `Continue`.
* Follow Apple's instructions on how to create a Certificate Signing Request.
* Upload your signing request to create a new certificate.
* Download the certificate and double click it to open it in Keychain.

## Create App ID

If you've already created an App ID for your app, continue on to the next section.

* Go to your [apple developer account](https://developer.apple.com/account/ios/identifier/bundle) and select `App Id's` on the left menu under `Identifiers`.
* Click on the plus button at the top right corner and enter the following details:
  - App ID Description: The name of your app.
  - App ID Prefix: Leave as default, should be Team ID.
  - App ID Suffix: Explicit App ID. Enter the bundle id of your app. This should be something like `com.your-name.app-name`
  - App Services: Check any services that your app uses.

![New App](http://i.imgur.com/fuKJye9.png)

* Click `Continue` at the bottom of the page.
* Confirm the information and click the `Register` button.

## Create Provisioning Profile

* select `distribution` on the left menu under `Provisioning Profiles`.
* Click on the plus button at the top right corner.
* Select `Ad Hoc` under `Distribution` and click `Continue`.
* Select the `App ID` you just created from the dropdown menu and click `Continue`.
* Select the ad hoc certificate that you made in the first step and click `Continue`.
* `Select All` for the devices and click `Continue`.
* Enter a name for this provisioning profile and click `Continue`. This is the name that will show up in Xcode.

![Profile Name](http://i.imgur.com/mEqUHUK.png)

* Click `Download` to download the new profile, and double click it to open it in Xcode.

## Create new app in iTunes connect

If you've already created your app in iTunes Connect, continue on to the next section.

* Login to [iTunes Connect](https://itunesconnect.apple.com/).
* Click on `My Apps`.

![My Apps](http://i.imgur.com/7cZqMkz.png)

* Click the plus button in the top right corner, and select `New App` from the drop down.

![New App](http://i.imgur.com/4Mla6CZ.png)

* Enter the following information in the pop up windows:
  - Platform: iOS
  - Name: The name of your app as it will appear on the app store.
  - Primary Language: Probably English.
  - Bundle ID: The App ID you created earlier.
  - SKU: A unique ID for your app that is not visible on the App Store.
* Click the `Create` button.
  
![New App](http://i.imgur.com/IJtpg0v.png)

* Click on Testflight

## Upload app

* Open your app settings in Xcode, and make sure the bundle ID matches the ID on the certificate you just created.

![Bundle ID](http://i.imgur.com/r3EOCJP.png)

* In the `signing` section, make sure your development account is set as the `Team`.

![Signing](http://i.imgur.com/l3xOl7L.png)

* Click on the current build device and select `Generic iOS Device` from the drop down menu.

![Generic iOS Device](http://i.imgur.com/WJF9aUl.png)

* Go to the `Product` menu item and select `Archive`.

![Archive](http://i.imgur.com/0rPRmky.png)

* When the new window opens, click the `Upload to App Store...` button.

![Upload to App Store...](http://i.imgur.com/VXrUqH2.png)

* Make sure your team is selected and click `Choose`.
* When it is done loading, click `Upload`.
* Wait for the app to upload, this can take a couple of minutes.

## Test Flight

* Go back to [iTunes Connect](https://itunesconnect.apple.com/).

### Internal Testing

#### Test Users

* Click `Users and Roles`.

![Users and Roles](http://i.imgur.com/tz6v1OZ.png)

* Click the `+` button next to the number of users.

![Add User](http://i.imgur.com/dGLZTcm.png)

* Enter the test user's name and email and click `Next`.
* Check the developer check box and click `Next`.
* Click `Save`. 

* Click the `iTunes Connect` in the top corner to go back to the main screen.
* Click on `My Apps`.
* Select your app from the list of apps.
* Select `TestFlight` from the top menu, and `Internal Testing` from the left menu.

![Internal Testing](http://i.imgur.com/8UoTIAi.png)

* Select the `+` button next to `Internal Testers` and select all users that you want to be testers.
* Click the `Save` button in the top right corner.
* Click the `Select Version to Test` link and select the version you uploaded earlier.

![Version](http://i.imgur.com/dzMywsr.png)

* Click `Ok`, Select `No` on the next screen, and click `Ok` again.
* Click the `Start Testing` button and celebrate 🤗



