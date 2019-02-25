# Veteran
A Custom Xcode Template that supports [InjectionIII](https://github.com/johnno1962/InjectionIII) and [Sherlock](https://sherlock.inspiredcode.io). 


This template is for developers that:
- Use Hot Reloading for the iOS simulator 
- Don't use **Main.storyboard**
- Use the same extensions over various projects
- Forget to implement `@objc func injected()` and the following code for InjectionIII

```Objective-C
#if DEBUG
Bundle(path: "/Applications/InjectionIII.app/Contents/Resources/iOSInjection10.bundle")?.load()
#endif
```



Added Files: 

`Extensions.swift` - An extension for UIView to help activate constraints  (Optional)

`SwiftInjection.swift` - Used for InjectionIII


 # Preview
<p align="center">
  <img src = "/Demo/Demo1.png" height = "350"> 
</p>

## InjectionIII

<p align="center">
  <img src = "/Demo/InjectionTest.gif" height = "500"> 
</p>


## Sherlock

<p align="center">
  <img src = "/Demo/SherlockTest.gif" height = "500"> 
</p>


## Get Started
Drag the Veteran folder to `~/Library/Developer/Xcode/Templates/Project Templates`

## Credit
Helmet by Veysel Kara from the Noun Project
