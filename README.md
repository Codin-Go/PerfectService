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
 
https://velog.velcdn.com/images%2Fsunnysideup%2Fpost%2F144a3119-e00f-4361-834b-f3c96b53d0d2%2FScreen%20Shot%202021-09-27%20at%2010.00.47%20PM.png

## L
Lecture 4: Memorize Game Logic



[ObservableObject] Protocol and [@Published]

.When Model Changed, Publish(return and fresh)


class EmojiMemoryGame: ObservableObject {
    ...
    
    @Published private var model = createMemoryGame()
    
    ...
}
내용을 입력하세요.

@ObservedObject

.When [viewModel] is [published], rebuild [body]


struct ContentView: View {
    @ObservedObject var viewModel: EmojiMemoryGame
    
    var body: some View {
        ...
    }
}
내용을 입력하세요.
enum (enumeration)

.overview : dont need value

.Sytax : Type and case

.Iterating enum cases (tea, water)

.Associated Values (upc, qr. can be changed)

.Raw Values (previous choosen. not like Associated Values)

..Implicitly Assigned Raw Values (mercury=1, venus.. , north, south)

..initializing from a Raw Value

..Recursive Enumerations (indirect enum)



.ref.

.. https://bbiguduk.gitbook.io/swift/language-guide-1/enumerations

.. https://www.google.com/search?client=safari&rls=en&q=%EC%9E%AC%EA%B7%80+%EB%9C%BB&ie=UTF-8&oe=UTF-8&safari_group=9


재귀 뜻 - Google Search
재귀란? (개념 이해하기) | 재귀 알고리즘 | Khan Academy - 칸아카데미 ko.khanacademy.org › 컴퓨팅 › 컴퓨터과학 › 알고리즘 › 재귀 알고리즘 이처럼 어떤 문제를 해결하기 위해 알고리즘을 설계할 때 동일한 문제의 조금 더 작은 경우를 해결함으로써 그 문제를 해결하는 것입니다. 문제가 간단해져서 바로 풀 수 ... 재귀함수 - 나무위키 namu.wiki › 재귀함수 Jan 13, 2022 · 재귀함수(再歸函數)는 정의 단계에서 자신을 재참조하는 함수를 뜻한다. 어떤 사건이 자기 자신을 포함하고 다시 자...

www.google.com


﻿


 
## Reference 
1. Standford, [cs193p site by Stanford](https://cs193p.sites.stanford.edu)
2. Skkimeo, https://github.com/skkimeo/
3. devxoul, https://github.com/devxoul/


## License
**Then** is under MIT license. See the [LICENSE](LICENSE) file for more info.
