# Veteran
A Custom Xcode Template that embeds [InjectionIII](https://github.com/johnno1962/InjectionIII) and removes **Main.storyboard**. This is for developers that use Hot Reloading for the iOS simulator and programmatically create constraints. 

Added Files: 

`Extensions.swift` - An extension for UIView to help activate constraints. 

`Injection.swift` - For Hot Reloading

 # Preview
<p align="center">
  <img src = "/Demo/Demo1.png" height = "300"> 
  <img src = "/Demo/Demo2.png" height = "300"> 
</p>


Modified Files:

`AppDelegate.swift`

```objc
    func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions:[UIApplication.LaunchOptionsKey: Any]?) -> Bool {
        // Override point for customization after application launch.
        window = UIWindow(frame: UIScreen.main.bounds)
        window?.rootViewController = HomeViewController()
        window?.makeKeyAndVisible()

        #if DEBUG
        Bundle(path: "/Applications/InjectionIII.app/Contents/Resources/iOSInjection10.bundle")?.load()
        #endif
        return true
    }

```


## Get Started
Drag the Veteran folder to `~/Library/Developer/Xcode/Templates`

## Credit
Helmet by Veysel Kara from the Noun Project
