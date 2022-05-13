# PerfectService

![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)

- 1Y1M.
- In 1 Year, How Can We Make 1 Million Dollar?
- In 1 Year, Service 10 Million Dollar. How Can We Make It?  
- Log of Study, Apply, Reflect.
- Codin Go.


<br> 


## Table of Contents

[Objective](#Objective)

[Chapter 1. Service](#Chapter-1-Service)

[Chapter 2. Kits](#Chapter-2-Kits)

[Chapter 3. Language](#Chapter-3-Language)

* [3.1. Stanford Lecture](#31-Stanford-Lecture)

* [3.2. Swift.org](#32-Swiftorg)


[Chapter 4. Today](#Chapter-4-Today)

[Reference](##Reference)

[License](##License)

<br> 
<br> 




# Objective
.Service.App <br> 
..SeeCode <br> 
...Standford <br> 
....Index QA <br> 
....SeeCode <br> 
....ShareSummary <br> 

.1MHA <br> 
.One Month Hundred App <br>
..App <br>
..Web <br>
..Lecture <br>
..Book 

<br> 
<br> 

# Chapter 1 Service 

1. Google Web, App 
2. Apple Web, App 
3. AMAZON Web, App
4. TikTok App
5. WeChat App, Web
6. NAVER App, Web
7. KAKAO App, Web

<br> 
<br> 

# Chapter 2 Kits 

- 1MHA. One Month Hundred App. 
- Examples and Kits for Main Service. 
- Index Q&A
  - https://www.icloud.com/numbers/01bT1ZT_bO1_NXSSUJi5ZBYaA#Map_of_iPhoneAppMaking

<br> 
<br> 
﻿

# Chapter 3 Language

## 3.1 Stanford Lecture

## Lecture : What we can learn?

. Game . TapGesture . (RoundedRectangle, emoji) <br> 
. struct . (View, some, body, ZStack HStack, Bool, @State, Array, ForEach, \.self, spacer, padding, systemName, LazyVGrid, GridItem, aspectRatio, ScrollView, <br> 
. meaning . (Option + Click, 0..<6 <br> 
. word . (immutable, snippet, infer, <br> 
. whole . (readable, simple, short, <br> 
. Model . (MVVM Model-View-VieModel, <br> 


## Lecture 1: Getting started with SwiftUI

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

## Lecture 2: Learning more about SwiftUI

[@State] :

. like Pointer. Pointing Memory (Same). even memory changes.

[#spacer()] :

. all the remains space

<br>

## Lecture 3: MVVM

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

<br> 

## 3.2 Swift.org 
- https://www.swift.org

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

<br> 

## Lecture 4: Memorize Game Logic

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
<br> 


# Chapter 4 Today

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
- Practice Day4 220513 Standford Lecture 4 (o)
   - Impressive 3: Structure Understanding, Making App One Step More, Amazing Structure Managing using Markdown.
   - Core: `_`,  `$0>$1`, override func, enum (a given raw value, and rest in order), Class, Structure. 
   - Q: More Fast Follower? 
   - Review: MVVM, Assignment1 on swiftorg (Object Class, Struct, Enum, )
   - Reflect: Side -> Core 
   - Improve: 14min, 50min, Target Time, Dig in core first. 
- Practice Day5 220514 

<br> 
<br> 

## Reference
1. Standford, Paul Hegarty CS193p (Stanford, Spring 2021), https://cs193p.sites.stanford.edu
2. Skkimeo, https://github.com/skkimeo/
3. devxoul, https://github.com/devxoul/
4. Sunny, Note of CS193p, https://velog.io/@sunnysideup/Stanford-CS193p-Spring-2021
5. Apple, symbols, developer.apple.com/sf-symbols
6. sh9404, MVVM, https://lsh424.tistory.com/68
7. Swift, KR, https://bbiguduk.gitbook.io/swift/language-guide-1/enumerations
8. HJ Song BG Lee, Making iPhone using Swift (easyspub, 2022)

<br> 

## License
Above is under MIT license. See the [LICENSE](LICENSE) file for more info.
