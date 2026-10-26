REACT NATIVE

◯ core components :- 

▢ what are components :- components are reusable building blocks of the UI.

what is the benifit of components :-
Reusability — Write once, use anywhere.
Maintainability — Easier to update and fix bugs.
Organization — Clean and structured code.
Consistency — Same button style across the entire app.

1. view :- It is a basic block of code, It is used to create containers and organize other components.
| important props | what it does                             | common values         |
| :---------------: | :----------------------------------------: | :---------------------: |
| style           | Main way to style the View               | Style object          |
| onLayout        | Get dimensions of the View               | ({nativeEvent}) => {} |
| accessible      | Makes View accessible for screen readers | true / false          |

2. text :- used to display text.
| prop          | what it does                            | common values                    |
| :-------------: | :---------------------------------------: | :--------------------------------: |
| style         | Applies styling (fontSize, color, etc.) | Style object                     |
| numberOfLines | Limits the number of lines              | 1, 2, 3                          |
| ellipsizeMode | How to truncate text                    | "tail", "head", "middle", "clip" |
| onPress       | Makes text clickable                    | () => {}                         |

3. Image :- Displays images from local assets or remote URLs.
| prop                   | what it does                          | common values                           |
| :----------------------: | :-------------------------------------: | :---------------------------------------: |
| source                 | Image source (local or remote)        | require() or { uri: '...' }             |
| style                  | Width, height, borderRadius, etc.     | Style object                            |
| resizeMode             | How image fits in the container       | "cover", "contain", "stretch", "center" |
| defaultSource          | Placeholder image while loading (iOS) | Local image                             |
| loadingIndicatorSource | Placeholder while loading (Android)   | Local image                             |

4. scrollview :- It is used to see content that is bigger than the screen by scrolling.
| prop                           | what it does                          | common values          |
| :------------------------------: | :-------------------------------------: | :----------------------: |
| horizontal                     | Enables horizontal scrolling          | true                   |
| refreshControl                 | Adds pull-to-refresh                  | <RefreshControl ... /> |
| showsVerticalScrollIndicator   | Shows/hides vertical scrollbar        | false                  |
| showsHorizontalScrollIndicator | Shows/hides horizontal scrollbar      | false                  |
| contentContainerStyle          | Style for the inner content container | Style object           |

5. flatlist :- It is used to display a list of items. It shows only the items currently visible on the screen, so it works well with large lists.
| prop                   | What it does                        | example                                |
| :----------------------: | :-----------------------------------: | :--------------------------------------: |
| data                   | Array of data to display            | users                                  |
| renderItem             | Function to render each item        | ({ item }) => <Text>{item.name}</Text> |
| keyExtractor           | Returns unique key for each item    | (item) => item.id                      |
| ItemSeparatorComponent | Component rendered between items    | () => <View style={{height: 1}} />     |
| ListHeaderComponent    | Component at the top of the list    | <Text>Header</Text>                    |
| ListFooterComponent    | Component at the bottom of the list | <Text>End of list</Text>               |
| refreshControl         | Pull-to-refresh functionality       | <RefreshControl ... />                 |

6. section list :- It used to display a list of items grouped into different sections, where each section has its own heading.
| props          | what is does                                     | common values                 |
| :--------------: | :------------------------------------------------: | :-----------------------------: |
| onPress        | Called when pressed                              | () => {}                      |
| onLongPress    | Called when long pressed                         | () => {}                      |
| style          | Can accept a function for dynamic styling        | ({ pressed }) => ({})         |
| disabled       | Disables the pressable                           | true / false                  |
| android_ripple | Customize ripple effect on Android               | { color: '#fff', radius: 20 } |
| hitSlop        | Increases touchable area without changing layout | { top: 10, bottom: 10 }       |

7. touchable opacity :- It makes a component clickable and makes it slightly transparent when pressed.
| prop          | What it does                               | Common Values |
| :-------------: | :------------------------------------------: | :-------------: |
| onPress       | Function called when pressed               | () => {}      |
| activeOpacity | How much opacity reduces on press (0 to 1) | 0.7, 0.8, 0.5 |
| style         | Styling for the touchable area             | Style object  |
| disabled      | Disables the button                        | true / false  |
| onLongPress   | Called when long pressed                   | () => {}      |

8. safearea view :- It keeps your app content away from areas like camera cutouts, bottom gesture bar etc.
| props | what it does                              | common values                      |
| :-----: | :-----------------------------------------: | :----------------------------------: |
| style | Main styling (usually flex: 1)            | { flex: 1 }                        |
| edges | Control which edges get safe area padding | ["top", "bottom", "left", "right"] |

9. StatusBar :- It Controls the appearance of the device status bar.
| app router | page router |
| :----------: | :-----------: |

10. pressable :- It is a modern alternative to TouchableOpacity that gives you better control over touches and lets you change styles dynamically when pressed.



9.  activity indicator :- It is native component that displays a loding spinner, it is commonly used to show that content is loading.

10. refresh control :- It is native component that provides pull to refresh functinoality.

11. text input :- It is the equivelent of html input and textarea elements.




