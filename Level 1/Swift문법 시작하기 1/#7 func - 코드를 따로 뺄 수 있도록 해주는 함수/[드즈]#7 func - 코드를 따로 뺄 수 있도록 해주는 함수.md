# 7. Function

## function

---

필요할 때마다 실행할 수 있는 이름이 지정된 코드 세트

```swift
func 함수이름(~~매개변수: 타입~~) ~~-> 반환타입~~ {
    코드
}
```

### 호출

```swift
함수이름(~~인자값: 할당값~~)
```

### 활용

```swift
@State var myMind: String = "nothing"
@State var isChangeMind: Bool = false

VStack {
    Text(myMind)
		
    Button {
        isChangeMind.toggle()

        **if isChangeMind {
                myMind = "always open"
        } else {
                myMind = "but closed"
        }**
    } label: {
        Text("Change my mind!")
    }
}
```

---

```swift
@State var myMind: String = "nothing"
@State var isChangeMind: Bool = false

VStack {
    Text(myMind)
    
    Button {
        isChangeMind.toggle()

        **myMind = getMind(isChangeMind: isChangeMind)**
    } label: {
        Text("Change my mind!")
    }
}

**func getMind(isChangeMind: Bool) -> String {
    if isChangeMind {
        return "always open"
    } else {
        return "but closed"
    }
}**
```

### 장점

- 코드를 따로 빼서 가독성이 올라감
- 여러번의 코드를 사용할 때, 함수만 호출하면 되기에 보기가 깔끔함
