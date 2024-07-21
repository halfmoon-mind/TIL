Device Activity를 처음 배우면서 에러가 났다.
DeviceActivityReport.Context 안에 totalActivity에 대해서 Context라는 속성이 없다는 오류였다.
왜 안되지 싶었는데 DeviceActivityReport로 Target을 추가하여 완전히 동일한 이름이기 때문에 해당 struct에 대해서 Context 속성이 없다고 하는 것이었다.
지나고 보면 진짜 별거 아니였지만, 처음 만지는 입장에서 그냥 Target을 생성했는데 에러가 발생하는 이유가 뭔지 이해하기 어려웠다.
### 결론
Apple에서 제공하는 API와 동일한 이름으로 Target을 생성하면 문제가 발생할 수 있다.