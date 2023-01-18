# how-to-Reduce-apk-size-in-react-native
how to Reduce apk size in react-native ? using proguard ?

**if you want to reduce your apk size in react-native than use Proguard**

 Run Proguard on Release builds to minify the Java bytecode.
 use only Proguard when Final Releasing app.

Why/What Proguard:
 * Set this to true to create four separate APKs instead of one,
 * one for each native architecture. This is useful if you don't
 * use App Bundles
 * and want to have separate APKs to upload to the Play Store.
 **Proguard will Convert Your App Code into bytecode easly**
 # how to use Proguard (1 Method)
 ```diff
 +just Enable OR set **true** at **adroid/app/build.gradle**
 ```
 ```
 def enableProguardInReleaseBuilds = true
 ```
#Method (2)
Now you can also set different Platform arch just use this
 just Enable OR set **true** at **adroid/app/build.gradle**
 See Below
```
def enableSeparateBuildPerCPUArchitecture = true
```

with the help of both method your app size will be reduce max 70% 
Now you can generate new release apk for all device.
