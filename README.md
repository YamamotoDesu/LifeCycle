# LifeCycle
iOS Unit Testing by Example - Chapter 2

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
