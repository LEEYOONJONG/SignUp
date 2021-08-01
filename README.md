# SignUp
회원가입 ViewController 연습

<img width="400" alt="스크린샷 2021-07-31 오후 4 08 01" src="https://user-images.githubusercontent.com/29617557/127768852-390f0502-bf58-4305-956d-a8f31ec4dcc1.png">

1. instantiateViewController 함수로 VC 지정하여 데이터 넘겨주고, self.navigationController?.push/popViewController로 뷰컨트롤러 전환
2. self.present 이용하여 뷰컨트롤러 전환 및 modalPresentationStyle 설정
3. DispatchQueue.main.asyncAfter 이용하여 수 초 후 뷰컨트롤러 pop하기
4. 아래 코드 사용하여 맨 처음 화면으로 이동하기
```swift
let signupVC = self.presentingViewController!
let navigationController = signupVC as? UINavigationController
navigationController?.popToRootViewController(animated: true)
self.dismiss(animated: true, completion: nil)
```
       
