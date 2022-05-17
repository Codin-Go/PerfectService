# PerfectService

![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)
![1M1H.app](https://img.shields.io/badge/1M1H.app-0.1-blue.svg)
![1Y1M.dollar](https://img.shields.io/badge/1Y1M.dollar-0.1-blue.svg)


- In 1 Year, How Can We Make 1 Million Dollar?
- In 1 Year, Service 10 Million Dollar. How Can We Make It?  
- Best Expert, Development x Business  
- This is the Log of Study, Apply, and Reflect. by Codin Go


<br> 


## Table of Contents

[Objective](#Objective)

[Chapter 1. Service](#Chapter-1-Service)

[Chapter 2. Modules](#Chapter-2-Modules)

  Map of Component
  - log in: phone log in; facebook, google, kakao, apple log in
  - info,ads: page view, style 
  - community: single id, database(JSON?)
  - playground: ai, ml, picture, video, voice, draw ; video draw, video popular 
  - coin: link w coinbase 
  - target: global or KR or govern
  - subscribe: 
  - pay: project, 

  Detail Side Project
  - Split Contents
  - CardGo1, CardGo2, CardGo3, AddDateChkList, Health  
  -  EmojiArt > EmojiGo1, BuildGo(Lego), EmojiDiary

[Chapter 3. Language](#Chapter-3-Language)

* [3.1. Stanford Lecture](#31-Stanford-Lecture)

* [3.2. Swift.org](#32-Swiftorg)
  1. Getting Start with SwiftUI
  2. Learning More about SwiftUI
  3. MVVM
  4. More MVVM enum Optionals
  5. Properties Layout @ViewBuilder
  6. Protocol Shapes
  7. ViewModifier Animation
  8. Animation Demo
  9. EmojiArt Drag/Drop
  10. Gesture
  11. Persistence Error Handling
  12. Binding Sheet Navigation EditMode
  13. Publisher More Persistence
  14. Document Architecture
  15. UIKit Integration
  16. Multiplatform (macOS)
  17. (2020) Enroute Picker Codable REST API
  18. (2020) Core Data


[Chapter 4. Today](#Chapter-4-Today)

[Reference](##Reference)

[License](##License)

<br> 
<br> 




# Objective
- Best Expert in iOS App Developer 
<br>

- Service.App 
  - SeeCode (Core: Language 10% understand and go)
    - Stanford
    - Index QA
    - SeeCode
    - ShareSummary 

<br>

- 1MHA, One Month Hundred App
  - App
  - Web
  - Lecture
  - Book 

<br>



<br> 
<br> 

# Chapter 1. Service 

1. Google Web, App 
2. Apple Web, App 
3. AMAZON Web, App
4. TikTok App
5. WeChat App, Web
6. NAVER App, Web
7. KAKAO App, Web

<br> 
<br> 

# Chapter 2. Modules 

- 1MHA. One Month Hundred App. 
- Examples and Kits for Main Service. 
- Index Q&A
  - https://www.icloud.com/numbers/01bT1ZT_bO1_NXSSUJi5ZBYaA#Map_of_iPhoneAppMaking

- Structure: 
   - Objective - Due - Materials - Required Test - Hint - Thinks to Learn - Evaluation - Extra Credit 

<br> 
<br> 
﻿

# Chapter 3 Language

## 3.1 Stanford Lecture


<details>

  <summary>Click to details</summary>


### Lecture : What we can learn?

. Game . TapGesture . (RoundedRectangle, emoji) <br> 
. struct . (View, some, body, ZStack HStack, Bool, @State, Array, ForEach, \.self, spacer, padding, systemName, LazyVGrid, GridItem, aspectRatio, ScrollView, <br> 
. meaning . (Option + Click, 0..<6 <br> 
. word . (immutable, snippet, infer, <br> 
. whole . (readable, simple, short, <br> 
. Model . (MVVM Model-View-VieModel, <br> 


### Lecture 1: Getting started with SwiftUI

[View]:

. is: On Screen, Get Input and Return Output

. types: [simple view], [combine view], [bag view]

```swift 
struct ContentView: View {
   var body: some View {
      Text("Hello World!")
   }
}
```
<br> 

### Lecture 2: Learning more about SwiftUI

[@State] :

. like Pointer. Pointing Memory (Same). even memory changes.

[#spacer()] :

. all the remains space

<br>

### Lecture 3: MVVM

[_] :

. in function, underbar, don't have name

```swift
func multiply(_ operand: Int, by otherOperand: Int) -> Int {
    return operand*operOperand
}
multiply(5, by: 6) 
```

[init] :

. struct and class

. initializers

```swift 
struct RoundedRectangle { 
  init(cornerRadius: CGFloat) {
}
```

struct x class :

. stract : value type, coppied, Functional programming, No inheritance, Free init All vars, Mutability on explicitly state, Seen so far is a struct (except view, protocol), <br> 

. class : reference type, pointer, Object-oriented programming, Inheritance, Free init No vars, Mutable, MVVM is a class (UIKit (old style iOS) is class-based)


Generics :

. "don't care" type


MVVM.component:

. Model: Data capsulation

. View : UI(Control..), Layout(Visual..)

. ViewModel: Model Data process to show on View


MVVM.proscons:

.pros: on View no UIKit, independent test on UI, less strees on Controller

.cons: binding library or lots of code.


static func:

. global function. share the variable with other all object


![](https://velog.velcdn.com/images%2Fsunnysideup%2Fpost%2F144a3119-e00f-4361-834b-f3c96b53d0d2%2FScreen%20Shot%202021-09-27%20at%2010.00.47%20PM.png)


### Lecture 4: Memorize Game Logic

[ObservableObject] Protocol and [@Published]

.When Model Changed, Publish(return and fresh)

```swift
class EmojiMemoryGame: ObservableObject {
    ...
    
    @Published private var model = createMemoryGame()
    
    ...
}
```


@ObservedObject

.When [viewModel] is [published], rebuild [body]

```swift
struct ContentView: View {
    @ObservedObject var viewModel: EmojiMemoryGame
    
    var body: some View {
        ...
    }
}
```

enum (enumeration)

.overview : dont need value

.Sytax : Type and case

.Iterating enum cases (tea, water)

.Associated Values (upc, qr. can be changed)

.Raw Values (previous choosen. not like Associated Values)

..Implicitly Assigned Raw Values (mercury=1, venus.. , north, south)

..initializing from a Raw Value

..Recursive Enumerations (indirect enum)

<br> 

</details>



<br>

## 3.2 Swift.org 

<details>
<summary> Click to details </summary>

Index 

A Swift Tour <br> 
- Simple Value
- Control Flow
- Functions and Closures
- Objects and Classes
- Enumerations and Structures
- Protocols and Extensions
- Error Handling
- Generics
- https://docs.swift.org/swift-book/GuidedTour/GuidedTour.html

API Design Guidelines <br> 
- Fundamentals
- Naming
  - Promote Clear Usage
  - Strive for Fluent Usage
  - Use Terminology Well
- Conventions
  - General Conventions
  - Parameters
  - Argument Labels
- Special Instructions 
- https://www.swift.org/documentation/api-design-guidelines/

The Basics
- Constants and Variables
- Comments
- Semicolons
- Integers
- Floating-Point Numbers
- Type Safety and Type Inference
- Numeric Literals
- Numeric Type Conversion
- Type Aliases
- Booleans
- Tuples
- Optionals
- Error Handling
- Assertions and Preconditions
- https://docs.swift.org/swift-book/LanguageGuide/TheBasics.html 

Language Guide
- The Basics
- Basic Operators
- Strings and Characters
- Collection Types
- Control Flow 
- Functions
- Closures
- Enumerations
- Structures and Classes
- Properties
- Methods
- Subscripts
- Inheritance
- Initialization
- Deinitialization
- Optional Chaining
- Error Handling
- Concurrency
- Type Casting
- Nested Types
- Extensions
- Protocols
- Generics
- Opaque Types
- Automatic Reference Counting
- Memory Safety
- Access Control
- Advanced Operators
- https://docs.swift.org/swift-book/LanguageGuide/TheBasics.html 

Language Reference 
- Lexical Structure
- Types
- Expressions
- Statements
- Declarations
- Attributes
- Patterns
- Generic Parameters and Arguments
- Summary of the Grammar 
- https://docs.swift.org/swift-book/ReferenceManual/AboutTheLanguageReference.html


Q & A

Typealias 
  - Not create new types. But provide new name to an existing type 
  ```swift
  typealias name = existing type
  ```

Shorthand Argument Names 
- $0 and $1 refer to the closure’s first and second String arguments. Because $1 is the shorthand argument with highest number
```swift
reversedNames = names.sorted(by: { $0 > $1 } )
```

Heap
- Area of preserved computer main memory that a program process can use to store data in some variable amount that won't be known until the program is running. 

Generic 
- Generic Functions can work with Any Type.
```swift
func swapTwoValues<T>(_ a: inout T, _ b: inout T) {
    let temporaryA = a
    a = b
    b = temporaryA
}
```
Protocol
- A protocol defines a blueprint of methods, properties, and other requirements 


```swift
struct SomeStructure: FirstProtocol, AnotherProtocol {
    // structure definition goes here
}
```

Method

</details>

<br> 
<br> 


# Chapter 4 Today

## 4.1. Previous 

<details>
<summary> click here previous story </summary>

### Days
Base Book
- Do it, Making iPhone App using Swift
- Base Day1
- Base Day2
- Review Day1
- Review Day2

Practice 1MHA
- Practice Day1 220510  
- Practice Day2 220511
- Practice Day3 220512
- Practice Day4 220513 Stanford Lecture 4 (o)
   - Impressive 3: Structure Understanding, Making App One Step More, Amazing Structure Managing using Markdown.
   - Core: `_`,  `$0>$1`, override func, enum (a given raw value, and rest in order), Class, Structure. 
   - Q: More Fast Follower? 
   - Review: MVVM, Assignment1 on swiftorg (Object Class, Struct, Enum, )
   - Reflect: Side -> Core 
   - Improve: 14min, 50min, Target Time, Dig in core first. 
- Practice Day5 220514 Stanford Lecture 5 (..)
- P.D6.0515 CS193p Lec5~6
- P.D7.0516 CS193p Assn, Lec6,7,8,9,10; 11,12,13 ;  

  <details>

  <summary>Click to details</summary>

  #### Persistence
    - JSON

  #### MVVM 

  #### $0, $1
    - closure's first and second Shorthand Argument Names 
    ```swift 
     let coffee: [String] = ["Cappucinno","Esspresso","Latte","Ristretto"]

   reverseOrder = coffee.sorted {$0 > $1}
   // RESULT: ["Ristretto", "Latte", "Espresso", "Cappuccino"] 
    ```

  #### "_" Operator
    - Underscore Operator represents an unnamed parameter/label. 

  #### JSON
    - JavaScript Object Notion (JSON) is text-based format for representing structured data. It is used for transmitting data in Web App. 

  #### Property Wrappers
    - @ Things 
    - e.g. @State, @Published, @ObservedObject
    - @Binding, $
      ```swift
      struct OtherView: View {
        @Binding var sharedText: String {
          var body: View {
            Text(sharedText)
            TextField("shared", text: $sharedText)
          }
        }
      }
      ```
    - @EnvironmentObject: same as @ObservedObject
    - @ObservedObject: A property wrapper type that subscribes to an observable object 
      ```swift
      @propertyWrapper @frozon struct ObservedObject<ObjectType> where ObjectType : ObservableObject
      ``` 
    - Publisher, Sink
    - SwiftUI (ViewModels)


### P.D8.0517 CS193p 14,15,16, others, making, community

#### Cloud Kit 
Store structured app and user data in Cloud containers that all users of your app can share 

#### App Architecture 
- App icon 
- PalletStore: multiple documents 
- @SceneStorage  
- @ScaleMetric size 
- Undo: [<] mark
- Redo: undoManager?.redo()
- (v) FileWrapper: A representation of a node(a file, directory, or symbolic link) in the file system.

lec15. 
- Integrating with UIKit. 
- Delegation 
- Wrap in NavigationView  
- iPhone Camera, Paste. 
- SwiftUI: Framework. Declare the user interface and behavior for your app on every platform.
- UIKit: Framwork. Construct and manage a graphical, event-driven UI for your iOS or tvOS app. 
    - UIImagePickerController: Controller. UIKit world, there is no MVVM. UIKit called MVC.

lec16.
- Multiplatform (macOS + iOS)
- NS 
- utf8PlainText
- if os(iOS) 

Wrap-up
- Impressive: idea realize
- Review: Multi platform, iOS to macOS, camera usage, integrate UIKit. 
- Reflect: Focus Good for using emptyTime. 
- Improv: evisualize and other time. 

#### 
- P.D8.0517.2 CS193p 16, Review

#### lec16: Multiplatform
- popoverPadding 
- URL -> com.apple.security.network.client

#### +1. Picker (Filter)
- Flight Done and Cancel 
- NavigationView
- Hashable ? 

#### +2. Core Data
- Database  
- SQL: Save data
- Map 
- Enroute.xcdatamodeld
- import CoreData
- import Combine
- @FetchRequest 
- Extension 

#### wrap-up
- impressive: possible modules, 1 beautiful example, questions
- review: SwiftUI, MVVM, Data, Multiplatform
- reflect: focus on now, night story, Q&A
- improve: check status, better at night story, clear objective 


</details>


<br>

## 4.2. Today 
### P.D9.0518
- Objective: 1M1H.app 


<br> 
<br> 

# Chapter 5. Questions and Answers

  ## base.Modules
  
  ## app.Modules
  - Generic? ; API? ; How to use Cardify? ; Equatable? ; self? ; 
  - Roles? Struct? 
  - Save File?
  - Log in, Log out?

# Chapter 6. Challenge 
  - 4Day 1Book. (o) 
  - 1MHA
  - Memorize Stanford (App, Say, Video)
  - Local, Univ, School Teaching.
  - epub, book. 
  - 2021 Stanford
  - 2020 Stanford
  - 100days 


<br>

# Reference
1. Stanford, Paul Hegarty CS193p (Stanford, 2021, 2020), https://cs193p.sites.stanford.edu
2. Skkimeo, https://github.com/skkimeo/
3. devxoul, https://github.com/devxoul/
4. Sunny, Note of CS193p, https://velog.io/@sunnysideup/Stanford-CS193p-Spring-2021
5. Apple, symbols, developer.apple.com/sf-symbols
6. sh9404, MVVM, https://lsh424.tistory.com/68
7. Swift, KR, https://bbiguduk.gitbook.io/swift/language-guide-1/enumerations
8. HJ Song BG Lee, Making iPhone using Swift (easyspub, 2022)

<br> 

# License
Above is under MIT license. See the [LICENSE](LICENSE) file for more info.
