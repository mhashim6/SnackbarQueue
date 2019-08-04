# SnackbarQueue  
 A Library (a function, really) to show multiple snackbars sequentially.   
  
## Usage:  
``` kotlin  
Snackbar.make(root, R.string.welcome_message, LENGTH_LONG).enqueue() //first one will immediately show.  
Snackbar.make(root, R.string.introduction_message, LENGTH_LONG).enqueue() //but here, magic happens. 
Snackbar.make(root, R.string.preferences_tutorial, LENGTH_LONG).enqueue()  
Snackbar.make(root, R.string.goodbye_tutorial, LENGTH_LONG).enqueue() //last one to show, after all the others have been sequentially (and gracefully) dismissed. 
```  
## Apps using this library:  
  
 - [Put Back: The laid back reminder](https://play.google.com/store/apps/details?id=mhashim6.android.putback)  
  
## Dependency:  
[![](https://jitpack.io/v/mhashim6/SnackbarQueue.svg)](https://jitpack.io/#mhashim6/SnackbarQueue)  
  
Add it in your root build.gradle at the end of repositories:  
  
``` groovy  
allprojects {  
    repositories { 
       ... 
       maven { url 'https://jitpack.io' } 
    }
 }  
```  
Add the dependency:  
``` groovy  
dependencies {  
 implementation 'com.github.mhashim6:SnackbarQueue:1.0'
 }  
```