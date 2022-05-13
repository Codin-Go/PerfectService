# PerfectService

![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)

- Log of Study, Apply, Reflect
- Codin Go

<br> 


## Table of Contents

[Objective](#Objective)

Chapter 1. Service

Chapter 2. Example

[Chapter 3. Language](#Chapter-3-Language)



# Objective
.Service.App <br> 
..SeeCode <br> 
...Standford <br> 
....SeeCode <br> 
....ShareSummary <br> 

.1MHA <br> 
.One Month Hundred App <br>
..App <br>
..Web <br>
..Lecture <br>
..Book <br>


﻿
# Chapter 3 Language

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

## Lecture 2: Learning more about SwiftUI

[@State] :

. like Pointer. Pointing Memory (Same). even memory changes.

[#spacer()] :

. all the remains space


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

﻿

!
   [](https://velog.velcdn.com/images%2Fsunnysideup%2Fpost%2F144a3119-e00f-4361-834b-f3c96b53d0d2%2FScreen%20Shot%202021-09-27%20at%2010.00.47%20PM.png)

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

![](https://images.velog.io/images/sunnysideup/post/80b54ce3-dbe7-4ff6-a2b4-3d26993382a2/Stanford-CS193p-Spring-2016-Lecture12-Slides1.jpg)


 
## Reference 
1. Standford, [cs193p site by Stanford](https://cs193p.sites.stanford.edu)
2. Skkimeo, https://github.com/skkimeo/
3. devxoul, https://github.com/devxoul/


## License
**Then** is under MIT license. See the [LICENSE](LICENSE) file for more info.
