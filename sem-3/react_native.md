REACT NATIVE

◯ core components :- 

▢ what are components :- components are reusable building blocks of the UI.

▢ what is the benifit of components :-  
Reusability — Write once, use anywhere.  
Maintainability — Easier to update and fix bugs.  
Organization — Clean and structured code.  
Consistency — Same button style across the entire app.  

1. view :- It is a basic block of code, It is used to create containers and organize other components.  

| Important props | What it does                             | Common values       |
| :---------------: | :----------------------------------------: | :-------------------: |
| style           | Main way to style the View               | Style object        |
| onLayout        | Get dimensions of the View               | (nativeEvent) => {} |
| accessible      | Makes View accessible for screen readers | true / false        |

1. text :- used to display text.
| prop          | what it does                            | common values                    |
| :-------------: | :---------------------------------------: | :--------------------------------: |
| style         | Applies styling (fontSize, color, etc.) | Style object                     |
| numberOfLines | Limits the number of lines              | 1, 2, 3                          |
| ellipsizeMode | How to truncate text                    | "tail", "head", "middle", "clip" |
| onPress       | Makes text clickable                    | () => {}                         |

1. Image :- Displays images from local assets or remote URLs.
| prop                   | what it does                          | common values                           |
| :----------------------: | :-------------------------------------: | :---------------------------------------: |
| source                 | Image source (local or remote)        | require() or { uri: '...' }             |
| style                  | Width, height, borderRadius, etc.     | Style object                            |
| resizeMode             | How image fits in the container       | "cover", "contain", "stretch", "center" |
| defaultSource          | Placeholder image while loading (iOS) | Local image                             |
| loadingIndicatorSource | Placeholder while loading (Android)   | Local image                             |

1. scrollview :- It is used to see content that is bigger than the screen by scrolling.
| prop                           | what it does                          | common values          |
| :------------------------------: | :-------------------------------------: | :----------------------: |
| horizontal                     | Enables horizontal scrolling          | true                   |
| refreshControl                 | Adds pull-to-refresh                  | <RefreshControl ... /> |
| showsVerticalScrollIndicator   | Shows/hides vertical scrollbar        | false                  |
| showsHorizontalScrollIndicator | Shows/hides horizontal scrollbar      | false                  |
| contentContainerStyle          | Style for the inner content container | Style object           |

1. flatlist :- It is used to display a list of items. It shows only the items currently visible on the screen, so it works well with large lists.
| prop                   | What it does                        | example                                |
| :----------------------: | :-----------------------------------: | :--------------------------------------: |
| data                   | Array of data to display            | users                                  |
| renderItem             | Function to render each item        | ({ item }) => <Text>{item.name}</Text> |
| keyExtractor           | Returns unique key for each item    | (item) => item.id                      |
| ItemSeparatorComponent | Component rendered between items    | () => <View style={{height: 1}} />     |
| ListHeaderComponent    | Component at the top of the list    | <Text>Header</Text>                    |
| ListFooterComponent    | Component at the bottom of the list | <Text>End of list</Text>               |
| refreshControl         | Pull-to-refresh functionality       | <RefreshControl ... />                 |

1. section list :- It used to display a list of items grouped into different sections, where each section has its own heading.
| props          | what is does                                     | common values                 |
| :--------------: | :------------------------------------------------: | :-----------------------------: |
| onPress        | Called when pressed                              | () => {}                      |
| onLongPress    | Called when long pressed                         | () => {}                      |
| style          | Can accept a function for dynamic styling        | ({ pressed }) => ({})         |
| disabled       | Disables the pressable                           | true / false                  |
| android_ripple | Customize ripple effect on Android               | { color: '#fff', radius: 20 } |
| hitSlop        | Increases touchable area without changing layout | { top: 10, bottom: 10 }       |

1. pressable :- It is a modern alternative to TouchableOpacity that gives you better control over touches and lets you change styles dynamically when pressed.
| props   | when it does                                     | common values           |
| :-------: | :------------------------------------------------: | :-----------------------: |
| hitSlop | Increases touchable area without changing layout | { top: 10, bottom: 10 } |

1. touchable opacity :- It makes a component clickable and makes it slightly transparent when pressed.
| prop          | What it does                               | Common Values |
| :-------------: | :------------------------------------------: | :-------------: |
| onPress       | Function called when pressed               | () => {}      |
| activeOpacity | How much opacity reduces on press (0 to 1) | 0.7, 0.8, 0.5 |
| style         | Styling for the touchable area             | Style object  |
| disabled      | Disables the button                        | true / false  |
| onLongPress   | Called when long pressed                   | () => {}      |

1. safearea view :- It keeps your app content away from areas like camera cutouts, bottom gesture bar etc.
| props | what it does                              | common values                      |
| :-----: | :-----------------------------------------: | :----------------------------------: |
| style | Main styling (usually flex: 1)            | { flex: 1 }                        |
| edges | Control which edges get safe area padding | ["top", "bottom", "left", "right"] |

1.  StatusBar :- It Controls the appearance of the device status bar.
| props           | when it use                            | common values                   |
| :---------------: | :--------------------------------------: | :-------------------------------: |
| barStyle        | Color of status bar icons/text         | "dark-content", "light-content" |
| backgroundColor | Background color (Android only)        | "#FFFFFF", "#000000"            |
| translucent     | Makes status bar transparent (Android) | true / false                    |
| hidden          | Hide the status bar completely         | true / false                    |
| animated        | Animate changes in status bar          | true / false                    |

1.   model :- It displays content on top of the main screen.
| props          | when it does                               | common values                |
| :--------------: | :------------------------------------------: | :----------------------------: |
| visible        | Controls whether modal is shown            | true / false                 |
| animationType  | Type of animation                          | "slide", "fade", "none"      |
| transparent    | Makes background transparent               | true / false                 |
| onRequestClose | Called when Android back button is pressed | () => setModalVisible(false) |
| onShow         | Called when modal is shown                 | () => {}                     |

1.   activity indicator :- It is native component that displays a loding spinner, it is commonly used to show that content is loading.
| props            | what it does                                      | example value          |
| :----------------: | :-------------------------------------------------: | :----------------------: |
| size             | Size of the spinner                               | "small" or "large"     |
| color            | Color of the spinner                              | "#007AFF" or "#FF0000" |
| animating        | Controls whether the indicator is spinning        | true / false           |
| hidesWhenStopped | Hides the indicator when animating is false (iOS) | true / false           |

1.   switch :- It is a toggle button (ON/OFF switch) commonly used for settings, preferences, dark mode, notifications, etc.
| props               | what it does                                   | example                               |
| :-------------------: | :----------------------------------------------: | :-------------------------------------: |
| value               | Current state of the switch (ON/OFF)           | true / false                          |
| onValueChange       | Function called when switch is toggled         | (newValue) => {}                      |
| trackColor          | Color of the track (background)                | { false: '#767577', true: '#81b0ff' } |
| thumbColor          | Color of the circular knob                     | '#f4f3f4'                             |
| ios_backgroundColor | Background color when switch is OFF (iOS only) | '#3e3e3e'                             |
| disabled            | Disables the switch                            | true / false                          |

1.   refresh control :- It is native component that provides pull to refresh functinoality.
| props      | when to use                                | example value |
| :----------: | :------------------------------------------: | :-------------: |
| refreshing | Controls whether the loader is visible     | true / false  |
| onrefresh  | Function called when user pulls to refresh | () => {}      |

1.   TextInput :- TextInput is React Native’s equivalent of the HTML input and textarea elements. It is essential for forms, login screens, search bars, chat inputs, and almost any user data collection.
| props           | when it does            | common values |
| :---------------: | :-----------------------: | :-------------: |
| secureTextEntry | Masks input (passwords) | true / false  |

◯ Native features :-

1. Camere components : 

▢ CameraView : users see what their phone's camera is capturing, just like when they open the camera in WhatsApp or Instagram.
→ We used it for camera apps, qr code scanners, barvode scanners, banking applications, document scanning apps, attendance system, face verification app, social media apps.

▢ CameraView props : 
1. facing - It is a prop of CameraView that determines which camera the application should use: the front camera or the back camera. (front, back)
2. flash - The flash prop controls how the camera flash behaves when taking a photo. (on, off, auto)
3. autofocus - The autofocus prop controls whether the camera automatically adjusts its focus to make the subject look sharp and clear.(on, off)
4. mirror - The mirror prop controls whether the camera preview or captured image is flipped horizontally, like looking in a mirror. (true, false)
5. mute - The mute prop controls whether audio is included when recording a video. 
   false : Records video with audio., true : Records video without audio.
6. zoom - The zoom prop controls how much the camera is zoomed in or zoomed out. (0-no zoom(default), 0.5-meduim zoom, 1-maximum zoom)

▢ camera view methods :

1. takePictureAsync() - It is a method provided by expo-camera that is used to capture a photo from the device camera.
→ When the user taps the Capture button, this method takes a picture and returns information about the captured image.
→ Is takePictureAsync() Asynchronous? - It is an asynchronous method, which means it does not return the captured photo immediately, instead it returns a promise  
→ It returns - uri, width, height


▢ useCameraPermission() :- That helps us check whether the user has allowed the app to use the device's camera and request permission when needed.
→ what does the hook return :
| value               | description                                   |
| :-------------------: | :---------------------------------------------: |
| permission          | Contains the current camera permission status |
| requestPermission() | Requests camera permission from the user      |

→ permission states : granted(user allowed camera access), denied(user rejected camera access), undetermind(application has never requested camera permission before)

▢ takePictureAsync() options :-
| option         | purpose                                | value                     |
| :--------------: | :--------------------------------------: | :-------------------------: |
| quality        | Controls image quality and compression | 0-low, 1-high             |
| base64         | Returns the image as a Base64 string   | true, false(Default)      |
| exif           | Returns EXIF metadata of the image     | true, false(default)      |
| skipProcessing | Skips additional image processing      | true, false(default)      |
| shutterSound   | Enables or disables the shutter sound  | true, false(if supported) |

◯ Vedio recording :-

▢ there are 2 primary methods for vedio recording :-
| method          | purpose                           |
| :---------------: | :---------------------------------: |
| recordAsync()   | Starts recording a video          |
| stopRecording() | Stops the current video recording |

◯ QR code and barcode scanning :-

▢ QR code :-
Code is a two-dimensional barcode that can store different types of information like website urls, contact information, wifi Credentials, payment information, text messages, product information.

▢ Barcode :- 
It is a machine-readable representation of numbers or characters, usually represented by a pattern of parallel lines and spaces.

2. Location :-

◯ How Does Expo Get Your Location?
→ through gps, wifi, mobile network.

▢ GPS :- It is a satellite-based navigation system used to determine the location of a device on Earth.
→ location is represented using latitude and logitude 

▢ latitude - tells us how far a location is north or south of the Equator.
→ range is between -90ॱ to +90ॱ 

▢ Longitude - tells us how far a location is east or west of the Prime Meridian.
→ range is -180ॱ to +180ॱ 

◯ What is accuracy :-
It tells how close the reported location is to the user's actual position.

◯ Foreground location :- It means your application accesses the user's location while the app is open and being used, or under the operating system's permitted foreground conditions.
→ used for maps, food dilivery app, ride booking app

◯ Background location :- It means an application can receive location updates while it is not actively displayed on the screen, subject to operating-system restrictions and permissions.
→ used for fitness tracker, running app etc

◯ geocoding :- It is the process of converting a human-readable address or place name into geographic coordinates (latitude and longitude).

◯ reverse geocoding :- It is the process of converting geographic coordinates (latitude and longitude) into a human-readable address or place name.

▢ geocoding vs reverse geocoding :-
| geocoding                     | reverse geocoding            |
| :-----------------------------: | :----------------------------: |
| address → coordinates         | coordinates → address        |
| input - string                | input - latitude & longitude |
| output - latitude & longitude | output - address             |
| used for search               | used for display             |

◯ What is heading :- It tells us the direction in which a device, such as a smartphone, is pointing or facing.

◯ altitude :- location.coords.altitude represents the device's estimated height above sea level, measured in meters.

◯ timestamp :- location.timestamp represents the date and time when the location information was captured or recorded.

3. contacts :- 

◯ Why Do We Use * as Contacts?
import * as Contacts means import all the available functions from expo-contacts into one group called Contacts.

▢ getContactsAsync() - It is used to get or fetch the contacts saved on the user's device.

▢ { data } - It extracts the data property from the result and stores it directly in a variable called data.

▢ Optional chaining - It helps prevent errors when a value is missing, but it does not prevent every possible error.

▢ Linking - It allows your app to open another app or a webpage using a URL.

▢ tel: - It is a URL scheme that tells the phone to handle a telephone number.

▢ VCF(Virtual Contact File) file - It is a file that stores contact information and allows you to transfer contacts from one device to another.

4. clipboard :-
It is temporary storage where copied content is kept until you paste it somewhere.
→ setStringAsync() copies a string of text into the clipboard.
→ getStringAsync() reads the text currently stored in the clipboard.
→ hasStringAsync() checks whether the clipboard contains text.

→ seturlAsync() - copies only url
→ geturlAsync() - reads only url
→ hasurlAsync() - checks

→ hasImageAsync() - Checks whether an image exists: (true/false in result)
→ getImageAsync() - Actually retrieves the image (image or null)

▢ Base64 - It is a way to represent data, such as an image, using text characters.

▢ clipboard listener - It detects when the clipboard content changes while your app is open.

5. Share :- 
It allows users to share content from your app with other apps. 

| api                     | purpose             |
| :-----------------------: | :-------------------: |
| Share from React Native | share text and urls |
| expo-sharing            | share local files   |

◯ Share Sheet - It is the menu that appears when you want to share something with another app.

▢ message is the actual shareable text. title is not a guaranteed heading that the recipient will receive or that the user will visibly see in the native share UI.

→ trim() removes extra spaces from the beginning and end of a string.

▢ Understanding the share result :-

1. Share.sharedAction - It helps check whether the sharing action was completed.
2. Share.dismissedAction - It indicates that the user closed or dismissed the Share Sheet without completing the sharing action.
3. activityType - It is mainly relevant to iOS and may be undefined if the information is not available.
→ activityType: null on Android is normal because Android does not provide the iOS-specific sharing activity information through this API.

6. Notification :- 
It is a message displayed by the operating system to inform the user about something.

▢ There are 2 typesof notification :- 
→ local notificatino and push notification.

1. local-notification : It is a reminder that an app schedules on the user's device, and the device displays it at the scheduled time.
2. push-notification : It is a message sent to a user's device from a remote server through a push notification service.

◯ Local vs push notifications :-
| feature                                | local notification      | push notification       |
| :--------------------------------------: | :-----------------------: | :-----------------------: |
| main source                            | devide/app              | remote server           |
| backend required                       | not for basic sceduling | usually yes             |
| Internet required for basic scheduling | no                      | yes for remote delivery |
| example :                              | water reminder          | new chat message        |

◯ scheduled notification - It is a notification that is set to appear at a specific future time or when a specified condition occurs.

▢ Immidiate notification :- Show the notification now.
▢ sceduled notification :- Show the notification later.  

▢ foreground state :- It means your app is open and visible on the phone screen, and the user is using it.
▢ background state :- It means your app is no longer visible on the screen because the user has switched to another app or the home screen.

▢ setNotificationHandler() - It tells your app how to display a notification when it arrives while your app is open (in the foreground).

▢ There are mainn 4 features of notification handler :- 
| option           | purpose                                        |
| :----------------: | :----------------------------------------------: |
| shouldShowBanner | Show a notification banner                     |
| shouldShowList   | Show the notification in the notification list |
| shouldPlaySound  | Play a notification sound                      |
| shouldSetBadge   | Allow badge-related behavior                   |

→ A notification ID helps your app identify and manage individual notifications, such as cancelling a specific scheduled notification.
→ scheduleNotificationAsync() schedules a notification for later; it does not necessarily display it immediately.

▢ What If the App Is Closed? - This means a scheduled local notification can still appear even after the user closes the app, because the operating system manages the scheduled notification.

▢ notification trigger - It tells the operating system when a scheduled notification should appear.
→ There are 3 main concepts of notification trigger.
| concept              | purpose               | example               |
| :--------------------: | :---------------------: | :---------------------: |
| time interval        | After some time       | After 10 seconds      |
| Specific Date / Time | At a particular time  | October 28 at 8:00 PM |
| Repeating Schedule   | Repeats on a schedule | Every day at 8:00 AM  |

▢ Recurring notifications - They are notifications that appear repeatedly according to a schedule, instead of appearing only once.

▢ notification channel - It is a category used to organize notifications on Android. It lets users control settings such as the sound, vibration, and importance of different types of notifications.
→ There are 3 settings of notification chanel :- exist, sound, vibration 

7. authentication :- 

▢ expo-local-authentication allows your app to verify the user using the device's biometric authentication, such as a fingerprint or face recognition.

▢ Biometric Hardware - It means the physical sensor or technology available on the device.
e.g. - fingerpint sensor, face recognitino hardware

▢ Biometric Enrollment - It means the user has already registered their fingerprint or face on the device.
e.g. - The user has set up Face ID on their phone, The user has added their fingerprint in phone settings

▢ Main api's :-
| API                                   | what it does                                               | Return                               |
| :-------------------------------------: | :----------------------------------------------------------: | :------------------------------------: |
| hasHardwareAsync()                    | Checks whether biometric hardware exists                   | Promise<boolean>                     |
| isEnrolledAsync()                     | Checks whether an authentication credential is enrolled    | Promise<boolean>                     |
| supportedAuthenticationTypesAsync()   | Gets supported authentication types                        | array                                |
| getEnrolledLevelAsync()               | Gets the enrolled authentication security level            | Promise<SecurityLevel>               |
| authenticateAsync()                   | Starts actual authentication                               | Authentication result                |
| cancelAuthenticate()                  | Cancel active authentication on Android                    | void                                 |

▢ Why Do We Check Hardware First? 
We check biometric hardware first to know whether the device supports biometric authentication before trying to use it.

▢ prompt is the authentication message or screen displayed to the user when the app asks them to verify their identity.

▢ Fallback authentication means providing an alternative way to verify the user when the primary authentication method is unavailable or cannot be used.

8. Network :-
expo-network is an Expo SDK library that helps your app get information about the device's network connection.

▢ Network - It allows devices to communicate with each other.
▢ Internet - It allows your device to access online services, such as Google, YouTube, and APIs.

▢ NetworkStateType is an enum in expo-network that provides a predefined set of values to identify the type of network the device is using.

| Value     | Meaning                                          |
| :---------: | :------------------------------------------------: |
| BLUETOOTH | Network connection through Bluetooth.            |
| CELLULAR  | Mobile network, such as 4G or 5G.                |
| ETHERNET  | Wired network connection.                        |
| NONE      | No network connection.                           |
| OTHER     | A network type that falls into another category. |
| UNKNOWN   | The network type cannot be determined.           |
| VPN       | Virtual Private Network.                         |
| WIFI      | Wi-Fi connection.                                |
| WIMAX     | A wireless broadband network technology.         |

9. file-system
expo-file-system is an Expo library that allows a React Native application to create, read, write, copy, move, delete, and manage files and directories on a device.

▢ file vs directory :- 
| File                 | Directory              |
| :--------------------: | :----------------------: |
| Stores data          | Organizes items        |
| Represents one file  | Represents a folder    |
| Example: notes.txt   | Example: notes/        |
| Can be read/written  | Can be listed/managed  |
| Has file metadata    | Has directory metadata |

▢ Path - A path is the location or address of a file or directory in a file system.
→ There are 2 types of path - relative and absolute.

(a) relative path - A relative path describes the location of a file or directory relative to a starting location.
(b) absolute path - It describes the complete location of a file or directory, starting from the file system's root or an appropriate storage root.

▢ What is URI(Uniform Resource Identifier) - A URI is a string that identifies a resource, such as a file, a webpage, or another resource. 
→ URI schemas :- file:// , http:// , https:// , content://

▢ path vs resource :-
path primarily describes the location of a file or directory, URI (Uniform Resource Identifier) identifies a resource.

▢ Persistent data is data that an application wants to keep available for future use, even after the application is closed.
▢ Temporary data is data that is only needed for a short period and can usually be recreated or downloaded again.

▢ What Belongs in Paths.document?
It is a location provided by Expo for storing files that an application wants to keep available for future use.

▢ What is chache?
A cache is a place where data is stored temporarily so it can be reused efficiently instead of being downloaded or generated again.

▢ What is Path.cache?
epresents the application's cache directory in expo-file-system.

▢ A FileHandle provides lower-level control over a file, allowing you to read or write data in smaller portions and control where operations happen within the file.

10. splash screen :-
It Appears during the initial application launch, potentially before React Native renders any components.

▢ it should be used for brand identity, smooth startup experince, consistent appearance.

▢ Diffrence between splash screen and loading screen :-
| Native Splash Screen                                        | React Native Loading Screen                                  |
| :-----------------------------------------------------------: | :------------------------------------------------------------: |
| Appears during native application launch.                   | Appears when React Native renders a loading interface.       |
| Can appear before JavaScript is ready.                      | Requires React Native to render its components.              |
| Configured through native resources and Expo configuration. | Built using components such as View and ActivityIndicator.   |
| Handles the initial launch experience.                      | Handles operations that continue after the interface starts. |
| Commonly displays a logo and background.                    | Can display progress indicators, messages, and other UI.     |

▢ There are 2 ways to controll splash screen :-
Automatic control: Expo handles the normal splash screen visibility lifecycle.
Manual control: You decide when to hide the splash screen, usually after essential initialization finishes.

▢ Important method :-
| Method                 | Purpose                                         | Return Value     |
| :----------------------: | :-----------------------------------------------: | :----------------: |
| preventAutoHideAsync() | Requests manual control over visibility.        | Promise<boolean> |
| hide()                 | Hides the native splash screen.                 | void             |
| hideAsync()            | Backward-compatible asynchronous hiding method. | Promise<void>    |
| setOptions()           | Configures the supported fade-out animation.    | void             |

▢ hide() vs hideasync()
| hide()                                  | hideAsync()                        |
| :---------------------------------------: | :----------------------------------: |
| Synchronous method call.                | Returns a promise.                 |
| Does not require await.                 | Can be used with await.            |
| Preferred for straightforward new code. | Useful for backward compatibility. |

▢ When Is Manual Control Needed?
Manual control is needed when your app must finish essential tasks before showing the first screen.