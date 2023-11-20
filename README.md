# brandland-ar

## iOS & Android Build Settings
#### Configure Android Project:
+ Switch to Android
+ Change to Gamma
+ Graphics API > Disable / Remove Vulkan
+ Minimum API = Version 28
+ Scripting Backend = IL2CPP
+ ARM64 Only
+ Under XR-Plugin Managemenr > Android > Enable ARCore Plugin or configure it
#### Configure iOS Project
+ Switch to iOS
+ Add Camera Usage Description
+ Add Location Usage Description
+ Enable Requires ARKit Support
#### iOS & Android Device Deployment
##### Android
Simply connect to your computer via USB-C > Build And Run
##### iOS
Simply connect to your computer via Lightninig to USB-C > Build And Run
In XCode generated project apply these changes:
Search for BitCode under Build Settings > Set It To No
Add ARCore package to Unity-iPhone
Enable ARCore Geospatial component
💡 For a more detailed manual on Geospatial configuration take a look at [Google's ARCore documentation](https://developers.google.com/ar/geospatialcreator/intro)

## MetaAds configuration

+ Register on our website https://metaads.team/
+ Go to the Landowner -> My Ad Spaces and press button Add Ad Space
+ Select metaverse Unity
+ Download the personal unity MetaAds asset and install it on your project.
+ In project select game obgect AdSpotPlaneRight, copy unique Id and past it when create new Ad Space (enter name, description, default ad image, jump url).
+ Do this for all screens on which you want your advertisement to be broadcast. (Asset is downloaded only once.)
### Setting up an advertising company
#### Add Creatives
+ Go too tab Advertiser -> My Creatives
+ Press button Add Creative
+ Select Image or video file from your computer click Next button
+ Enter name, description and external target link then press Save button
#### Add Audience
+ Go too tab Advertiser -> Audience
+ Press button New template
+ Enter name, description and press Next Stepp button 
+ Add rules and creatives and press button Save & Quit
#### Create Compaigns

+ Go too tab Advertiser -> My  Compaigns
+ Press button New Compaign
+ Enter Name, description end select compaign starts end compaign ends date-times.
+ Select target Audience end press Next Step button
+ Set shedule and rules and press Next Step button
+ Choose Ad Spaces and press Next Step button
+ And finaly press Start Campaign button.
+ Your created compaign start in your select time.

## Adding new metaAds screen

+ In your project go to directory Assets -> MetaAds -> prefab 
+ Select prefab AdSpotPlane.prefab and drag and drop it in Scene.
+ Copy Unigue Id and register new Ad Space with this screen Unigue Id in our website https://metaads.team/
