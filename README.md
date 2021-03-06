Kinvey-OAuth2-DI-Sample
=======================

Sample Application that uses Instagram's API through OAuth 2.0 and Data Integration. This sample uses Core Location to obtain the user's location, gtm-oauth2 to obtain an access_token for connecting to Instagram, and Kinvey's Data Integration feature to load nearby images. 

![Screen Shot 1](https://github.com/KinveyApps/Kinvey-OAuth2-DI-Sample/raw/master/images/OAuth2Example_screen1.png)
![Screen Shot 2](https://github.com/KinveyApps/Kinvey-OAuth2-DI-Sample/raw/master/images/OAuth2Example_screen2.png)

### KinveyKit
This sample application requires a minimum of iOS 5.0 and KinveyKit 1.17.2. To use the sample app, go to [Kinvey](http://console.kinvey.com) and create a new App. You'll need the App id and App secret to set in `AppDelegate.m` in order to run this sample. 

### OAuth2
This project uses Google's [gtm-oauth2](http://code.google.com/p/gtm-oauth2/) library to obtain an acess token from Instagram. It's your responsiblity to log in to [Instragram's API](http://instagram.com/developer/), create an application with them and obtain the client id and secret. 

### Data Integration
There are two ql.io collections used by this sample app
* `instagram-locations` : provides a list of Instagram locations near a given latitude & longitude 
* `instagram-imagesAtLoc` : provides a list of recent images at a given Instagram location

This repo contains `instagram-locations_qlio_script.txt` and `instagram-imagesAtLoc_qlio_script.txt` which provide the ql.io script to use if you create these collections on your app backend. 

## License

Copyright (c) 2013 Kinvey, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.