# LifeCycle
iOS Unit Testing by Example - Chapter 2

![image](https://user-images.githubusercontent.com/47273077/178744829-44543765-d038-4d50-938d-7fb790badb98.png)

```swift

@testable import LifeCycle
import XCTest

class MyClassTest: XCTestCase {
    private var sut: MyClass!
    
    override func setUp() {
        super.setUp()
        sut = MyClass()
    }
    
    override func tearDown() {
        sut = nil
        super.tearDown()
    }

    func test_methodOne() {
        sut.methodOne()
    }
    
    func test_mehodTwo() {
        sut.methodTwo()
    }
}

```
