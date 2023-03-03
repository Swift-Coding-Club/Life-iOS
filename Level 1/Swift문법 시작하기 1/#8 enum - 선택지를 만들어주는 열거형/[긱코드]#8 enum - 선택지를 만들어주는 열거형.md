# 8. enum - 선택지를 만들어주는 열거형

enum이란 쉽게 말해 타입을 하나 만드는 것으로 볼 수 있다. enum타입은 특정 유형의 값을 가지는 연관된 그룹을 정의하는데 사용된다.

- enum은 특별하게 따로 숫자를 정해주지 않아도 rawValue를 0부터 순서대로 가진다.
- 새롭게 숫자를 부여할 수 도 있고 그밖의 다른 값들도 들어갈 수 있다.

```swift
enum Color {
    case red
    case blue
    case green
}

var selectedColor: Color = .red

print(selectedColor) // .red
print(selectedColor.rawValue) // 0

```


---
[긱코드의 Swift문법1 총정리 링크](https://github.com/isGeekCode/TIL/blob/main/swift/Swift1.md)
[긱코드의 TIL 총정리 링크](https://github.com/isGeekCode/TIL)
[깃허브](https://github.com/isGeekCode/)
[블로그](https://h1guitar.tistory.com/)
[링크드인](https://www.linkedin.com/in/hyeonseok-bang-52b780235/)
