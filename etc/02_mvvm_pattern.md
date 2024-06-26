# MVVM Pattern
> Model-View-ViewModel Pattern

코드를 작성하다 보면 중복 코드나 복잡한 로직이 등장할 수 있기 마련입니다.
코드를 분리하지 않다보면 코드의 품질도 떨어지고 유지보수가 어려울 수 있습니다.
따라서 이를 효율적으로 관리하기 위해 여러 디자인 패턴 혹은 아키텍처 패턴이 도입됩니다.
그 중 모바일 앱에서 자주 쓰이는 MVVM 패턴에 대해 알아보겠습니다.

### MVVM
MVVM 패턴은 각 역할에 따라 Model, View, ViewModel로 구성되어 있습니다.
흐름은 View-ViewModel-Model 순으로 가거나 역순으로 진행됩니다.

### View
- UI 화면 구성 담당
- 이벤트나 기능을 ViewModel에 요청
- 바인딩된 데이터에 따라 UI 빌드

### ViewModel
- 앱 비즈니스 로직 담당
- View에서 요청받은 기능을 수행, 데이터 변경 시 Model에 알림
- 데이터가 변경되면 View에 알림

### Model
- 데이터 비즈니스 로직 담당
- DB, 파일, 서버와의 통신 담당
- ViewModel에서 받은 알림에 따라 데이터 수정

MVVM 패턴을 사용하면 Model에서 제공하는 데이터를 UI로 표시하기 쉬운 형태로 변환해 줄 수 있습니다.
또한 View에서 복잡한 로직을 배제하여 확실하게 역할을 구분할 수 있습니다.
