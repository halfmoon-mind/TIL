Flutter로 개발을 하다보면 필연적으로 "상태 관리"에 대해서 배우게 된다.
그 중 가장 많이 사용하는 [GetX](https://pub.dev/packages/get)에 대해서 알아보자.
2024.07.22 기준으로 GetX의 Likes는 14392,  Provider의 Likes는 10018, Bloc는 Likes는 6918개 정도 갖고있다.
GetX를 가장 많이 사용하는 이유는 간단하다.
**"편해서"**
대부분의 기능들이 모두 지원이 된다. 또한 context에 대한 종속성이 없이 특정 값을 갖고 오거나 화면을 띄울 수 있다. 예를 들어보자.
> dialog를 띄운다고 하면 다음과 같이 코드를 작성해야한다
```dart
showDialog(
	context: context,
	builder (BuildContext context) {
		return Dialog(...);
	}
);
```
>GetX를 사용하면 이런 식으로 코드 작성이 가능하다.
```dart
Get.dialog(
	Dialog(...)
);
```
코드에서 볼 수 있듯이, context에 대한 종속성에서 벗어날 수 있다.
또한 Routing을 할 때도 간단하게 `Get.to(()=>DetailScreen());`와 같은 형태로 진행할 수 있다.

Dialog, Bottomsheet와 같은 것들을 띄울 때에도 context에 대한 종속성이 없이 호출할 수 있고, Routing
물론 편하다는 것에 장단점이 있다.
