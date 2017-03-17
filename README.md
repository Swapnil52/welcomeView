# welcomeView
A UIView subclass to display a series of welcome messages in iOS apps

### Usage
- Download and add the welcomeView.swift file into your Xcode project. Remember to check 'Copy if needed' otherwise only a reference of the file will be added.
- In your desired view controller, add an instance of welcomeView

```swift
var _welcomeView : welcomeView!
```

- It takes the following arguments to initialise:
  - frame : CGRect //Specify the frame property
  - messagesArray : [String] //Specify an array of messages to be displayed
  - backgroundColor : UIColor
  - textColor : UIColor
  - buttonColor : UIColor //Colour of the next button
  - completion : () -> Void //Completion handler called when the user taps the last 'next' button

  For example:
  
  ```swift
  _welcomeView = welcomeView(CGRect(x : 0.1*self.view.bounds.width, y : 0.1*self.view.bounds.height, width : 0.8*self.view.bounds.width, height : 0.8*self.view.bounds.height), ["First message!", "Second message!"], getColor(red: 61, green: 78, blue: 245), UIColor.white, UIColor.white, {
                
               
               //Do something e.g. set up the views do be displayed after the welcome view completes.
                    
                    
           })
  self.view.addSubview(self._welcomeView)
```










### GIF


<img src = "http://i.giphy.com/ijxFAmo2tg6wo.gif" height = 350>


### Contributors

This repository is actively maintained by Swapnil Dhanwal

*swapnildhanwal@hotmail.com*

*+91 9872704275*


