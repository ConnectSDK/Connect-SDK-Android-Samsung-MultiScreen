#Samsung MultiScreen module for Connect SDK (Android)
The Samsung MultiScreen module extends Connect SDK to add Samsung MultiScreen SDK support. This repository is included as a submodule in the main project, and has some manual setup before the main project will compile.

##General Information
For more information about Connect SDK, visit the [main repository](https://github.com/ConnectSDK/Connect-SDK-Android).

##Setup
###Connect SDK Integration
1. Go to the [Samsung MultiScreen site](http://multiscreen.samsung.com/downloads.html) and download the SDK
2. Extract the contents of the downloaded ZIP file, and locate the SamsungMultiScreen.framework bundle
3. Move the framework bundle into your samsung-multiscreen folder
4. Run your project

###Connect SDK Lite Integration
1. Clone this repository into a subfolder of the Connect SDK Lite project
2. Import the source files into the Connect SDK Lite Eclipse project
3. Follow the steps above for Connect SDK integration
4. In Connect SDK Lite's 'DefaultPlatform.java' file add line  'devicesList.put("com.connectsdk.samsungmultiscreen.MultiScreenService", "com.connectsdk.discovery.provider.SSDPDiscoveryProvider");' inside 'getDeviceServiceMap()' method.

##License
Copyright (c) 2013-2014 LG Electronics.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

> http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
