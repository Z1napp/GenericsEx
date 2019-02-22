# GenericsEx
```swift
//    #1
private func printMethod<T>(inputValue arr: [T]) {
    for object in arr {
        print(object)
    }
}
//    #2
struct GenericsArr<T> {
    var items = [T]()
    mutating func push(item: T) {
        items.append(item)
    }
}

//        #1
let strings = ["test1", "test2", "test3"]
let ints = [1, 2, 3, 4, 5]
let floats = [1.9, 2.2, 3.4]

printMethod(inputValue: strings)
printMethod(inputValue: ints)
printMethod(inputValue: floats)


//---
print("---")
//---


//        #2
let friendsList = ["Kyrylo", "Mykytosuk", "Evdakiy"]
var arr = GenericsArr(items: friendsList)
arr.push(item: "Ananiy")
print(arr)
```

# Output will be:
![ScreenShot](https://github.com/Z1napp/GenericsEx/blob/master/output.png?raw=true)

