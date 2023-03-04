# 7. func - 코드를 따로 뺄 수 있도록 해주는 함수

반복되는 코드는 함수를 만들어 따로 뺴서 사용할 수 있다.

### 파라미터가 없는 함수

아래는 파라미터가 없는 아주 기본적인 함수이다.

```swift
func printMyName() {
  print("긱코드")
}

printMyName()
// 긱코드
```

### 파라미터가 있는 함수

만약 함수를 사용하는데 상황에 따라 다른 내용을 넣고 싶다면 파라미터를 만들어서 사용할 수 있다.

```swift
func printMyName(name: String) {
  print(name)
}

printMyName(name: "긱코드")
// 긱코드

printMyName(name: "리이오")
// 리이오
```

파라미터는 상황에 따라 얼마든지 추가할 수 있다.


---
[긱코드의 Swift문법1 총정리 링크](https://github.com/isGeekCode/TIL/blob/main/swift/Swift1.md)
[긱코드의 TIL 총정리 링크](https://github.com/isGeekCode/TIL)
[깃허브](https://github.com/isGeekCode/)
[블로그](https://h1guitar.tistory.com/)
[링크드인](https://www.linkedin.com/in/hyeonseok-bang-52b780235/)
