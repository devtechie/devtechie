# SwiftUI Blog

<[DevTechie.com](https://www.devtechie.com)


## SwiftUI Layouts

SwiftUI has three basic layouts: VStack, HStack and ZStack. There are lazy version of VStack and HStack also available. 

#VStack

Let's start with VStack. VStack is a view that arranges its child views in a vertical line. 

```swift
struct VStackExample: View {
   var body: some View {
       VStack {
           Text("Hello")
           Text("World")
           Text("This")
           Text("is")
           Text("Hello")
       }
   }
}
```
In this example, we have 5 Text views arranged in vertical line.

#HStack

HStack arranges its child views in a horizontal line.

```swift
struct HStackExample: View {
   var body: some View {
       HStack {
           Text("Hello")
           Text("World")
       }
   }
}
```

#ZStack

ZStack arranges its child views in z space or in other word they are layed out on the top of each other.
```swift
struct ZStackExample: View {
    var body: some View {
        ZStack {
            RoundedRectangle(cornerRadius: 10.0)
                .fill(Color.orange)
                .frame(width: 200, height: 200)
            Circle()
                .fill(Color.blue)
                .frame(width: 100, height: 100)
            Text("Hello World!")
                .foregroundColor(Color.white)
        }
    }
}
```
