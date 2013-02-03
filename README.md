icon_template
=============

Eclipse Iconpack Project


Make sure you have API7 installed!
Window -> Android SDK Manager -> Check Android 2.1 (API 7) -> Install packages

File -> Import -> Android -> Existing Android.... -> OK

First you have to change the following points:

#1 
MainActivity/src/com.yourname.appname -> Right click -> Refactor -> Rename -> Enter something like com.WHATEVER.WHATEVER -> ok

#2
MainActivity/gen/com.yourname.appname -> Right click -> Refactor -> Rename -> Enter something like com.WHATEVER.WHATEVER (see above) -> ok

#3
MainActivity/AndroidManifest.xml
[...]
package="com.yourname.appname" <- com.WHATEVER.WHATEVER (see above)
android:versionCode="1" <- +1 with every upload in GooglePlayStore
android:versionName="1" <- Whatever you want, can be "abc" or "1.2.3.4"

#4 


#x-1
Copy your icons in MainActivity -> res -> drawable-hdpi 
Copy your wallpapers in MainActivity -> res -> drawable-nodpi 

#x Once you create an apk with this template just update 
/MainActivity/res/xml/appfilter.xml
/MainActivity/assets/appfilter.xml
/MainActivity/res/xml/drawable.xml
/MainActivity/assets/drawable.xml
/MainActivity/res/values/icon_pack.xml
/MainActivity/assets/icon_pack.xml
