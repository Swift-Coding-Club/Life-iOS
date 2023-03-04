# 9. switch - case의 패턴으로 나눠주는 Switch

switch도 일종의 조건문이라고 할 수 있다.

해당 값이 ~ 인경우를 정의하는 방법이다.

```swift
 enum Menu {
        case beef, pork, chicken
    }

 var myDinner: Menu = .pork

 switch myDinner {
    case .pork:
      print("pork")
    case .beef:
      print("beef")
    case .chicken:
      print("chicken")
  }

// pork

```

조건은 모두 쓰지않아도 에러가 나지않는다. 대신 이 경우 default를 넣어야한다.

만약 조건에 없다면 default를 넣어주면 조건을 명시하지않은 나머지 조건에 해당한다.

```swift
 enum Menu {
        case beef, pork, chicken
    }

 var myDinner: Menu = .beef

 switch myDinner {
    case .pork:
      print("pork")
    case .chicken:
      print("pork")
    default:
      print("다른거")
  }

// 다른거
```

위에서 나온 enum과 switch를 같이 사용할 때도 좋다.

```swift
enum Device {
    case iPhone
    case iPad
    case iMac
    case appleWatch
    
    func deviceType() -> String {
        switch self {
        case .iPhone:
            return "스마트폰"
        case .iPad:
            return "태블릿"
        case .iMac:
            return "데스크톱 컴퓨터"
        case .appleWatch:
            return "스마트워치"
        }
    }
}

let myDevice: Device = .iPhone
let deviceTypeName = myDevice.deviceType()
print(deviceTypeName) // 스마트폰
```


---
[긱코드의 Swift문법1 총정리 링크](https://github.com/isGeekCode/TIL/blob/main/swift/Swift1.md)
[긱코드의 TIL 총정리 링크](https://github.com/isGeekCode/TIL)
[깃허브](https://github.com/isGeekCode/)
[블로그](https://h1guitar.tistory.com/)
[링크드인](https://www.linkedin.com/in/hyeonseok-bang-52b780235/)
