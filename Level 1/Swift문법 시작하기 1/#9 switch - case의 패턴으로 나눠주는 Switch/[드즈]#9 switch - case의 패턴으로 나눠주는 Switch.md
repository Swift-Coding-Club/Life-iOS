# 9. Switch

# switch

---

특정 비교값이 case 패턴에 충족한 코드를 실행하는 데 사용되는 코드 구조

```swift
switch 비교값 {
case 패턴:
    코드
default:
    코드
}
```

`모든 case를 고려해주어야 합니다.`

`만약 모든 case중에서 한 case라도 빠진다면, default를 꼭 구현해주어야 합니다.`

## 활용

```swift
@State var menu: **String = "chicken"**

switch menu { 
case **"chicken"**:
    Text("오늘 메뉴는 닭고기")
default: 
    Text("이걸 먹을 수 있나?")
} /// 오늘 메뉴는 닭고기
```

### 열거형 활용

```swift
@State var menu: **Menu = .chicken**

enum Menu {
    case **beef, pork, chicken**
}

switch menu {
case **.beef, .pork**:
    Text("오늘 메뉴는 다리가 4개인 고기")
case **.chicken**:
    Text("오늘 메뉴는 다리가 2개인 고기")
/*
default:
    Text("이걸 먹을 수 있나?")
*/
} /// 오늘 메뉴는 닭고기
```
