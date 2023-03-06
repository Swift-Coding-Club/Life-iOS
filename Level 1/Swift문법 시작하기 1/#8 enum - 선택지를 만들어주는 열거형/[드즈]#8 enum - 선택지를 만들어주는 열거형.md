# 8. Enum

## Enumeration

---

관련있는 특정한 열거형 케이스 값을 정의하는 유형

```swift
enum 이름 {
    case 패턴이름
}
```

### 활용

```swift
@State var menu: **String = "chicken"**

if menu == **"beef"** {
    Text("오늘 메뉴는 소고기")
} else if menu == **"pork"** {
    Text("오늘 메뉴는 돼지고기")
} else {
    Text("오늘 뭐 먹지?")
}
```

---

```swift
@State var menu: **Menu = .beef**

**enum Menu {
    case beef, pork, chicken
}**

if menu == **.beef** {
    Text("오늘 메뉴는 소고기")
} else if menu == **.pork** {
    Text("오늘 메뉴는 돼지고기")
} else if menu == **.chicken** {
    Text("오늘 메뉴는 닭고기")
} else {
    Text("이걸 먹을 수 있나?")
}
```
