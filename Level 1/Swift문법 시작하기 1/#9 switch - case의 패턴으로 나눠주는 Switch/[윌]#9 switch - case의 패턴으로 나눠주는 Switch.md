## 9. switch-case

**Switch는 값을 여러 패턴과 비교하고, 일치하는 첫 번째 패턴에 따라 적절한 코드 블록을 실행합니다.** 스위치 문은 여러 잠재적 상태에 응답하기 위한 if 문의 대안을 제공합니다.

**모든 switch문은 모든 경우의 수를 반영해야합니다. 즉, 고려되는 유형의 가능한 모든 값은 switch `case` 중 하나에 의해 일치해야 합니다.**  해당하는 케이스가 없는 경우, `default`  키워드를 이용해서 나머지 케이스에 대해 정의 할 수 있고, 항상 마지막에 표시되어야 합니다.

```swift
struct ContentView: View {
    enum Menu {
        case beef
        case fork
        case salad
    }
    var today = Menu.beef
        
    var body: some View {
        
        
        VStack {
            switch today {
            case .beef:
                Text("오늘은 소고기")
            case .fork:
                Text("오늘은 돼지고기")
            case .salad:
                Text("오늘은 샐러드")
            }
        }
    }
}
```