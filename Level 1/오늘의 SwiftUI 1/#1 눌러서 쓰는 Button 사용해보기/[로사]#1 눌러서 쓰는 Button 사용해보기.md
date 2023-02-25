### 목표

- Button 생성과 활용
- Text를 사용해서 Button 꾸미기

### 짚어보기

아래내용에 대해 알고 있다면, 건너뛰어도 좋습니다. 

- 다양한 Button 생성 방법에 대해 알고있나요?
- Button 을 꾸밀 수 있는 방법에 대해 아시나요?

### SwiftUI 문서 바로가기

- [Button](https://developer.apple.com/documentation/swiftui/button)
- [Text](https://developer.apple.com/documentation/swiftui/text/)

### 공부하기

> Button을 생성하는 다양한 방법들에 대해 알아보자.
> 
1. 문자열을 입력하여 Label 을 생성하는 버튼 
    
    ```swift
    Button("버튼의 타이틀") {
      // 버튼을 눌렀을때 동작할 Action 정의
    }
    ```
    
2. Custom Label 을 표시하는 버튼 생성
    
    ```swift
    Button {
      // 버튼을 눌렀을때 동작할 Action 정의
    } label: {
      // 버튼의 생김새 정의
    }
    ```
    
3. Custom Label  을 표시하는 role을 가진 버튼 생성
    
    ```swift
    Button("Delete", role: .desctructive) {
      // 버튼을 눌렀을때 동작할 Action 정의
    }
    ```
    

### 더 해보기

- 모서리가 둥근 버튼을 만들고, Action 으로 print(”Hited!”) 를 넣어보세요.
- ButtonRole 은 어떻게 쓰일까요? 다양한 role 에 대해 알아보고 만들어보세요.
- 이미지를 넣은 Button 을 만들어보세요.

---

### 단축키

| 설명 | 단축키 |  |
| --- | --- | --- |
| UI 그릴수 있는 목록 불러오기 | command + shift + L | Xcode → View → Show Library |