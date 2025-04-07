## 트러블슈팅
어떤 이유에서 앱 설치안될 때, XAPK 파일로 설치하기 (단, 버전 맞추기)

![image](https://github.com/user-attachments/assets/acadd3f3-dfd3-4ad9-b989-042f37cdd416)


## MobSF
```
docker pull opensecurity/mobile-security-framework-mobsf:latest
docker run -it --rm -p 8000:8000 opensecurity/mobile-security-framework-mobsf:latest
//mobsf / mobsf
```

## 
앱 설정에 따라 설치가 안되기도함 그때는 버전, SDK버전 확인

| 안드로이드 버전 | 코드네임         | API 레벨 | SDK 이름         | 갤럭시 기기 예시                                |
|----------------|------------------|----------|------------------|------------------------------------------------|
| Android 14     | —                | 34       | android-34       | 갤럭시 S24 시리즈, Z Fold5, Z Flip5            |
| Android 13     | Tiramisu         | 33       | android-33       | 갤럭시 S23 시리즈, S22, A54, Z Fold4           |
| Android 12     | Snow Cone        | 31~32    | android-31, 32   | 갤럭시 S21 시리즈, A52, Z Flip3                |
| Android 11     | Red Velvet Cake  | 30       | android-30       | 갤럭시 S20 시리즈, A71, Note 20                |
| Android 10     | Q                | 29       | android-29       | 갤럭시 S10 시리즈, A50, Note 10                |
| Android 9      | Pie              | 28       | android-28       | 갤럭시 S9 시리즈, A30, Note 9                  |
| Android 8.0~8.1| Oreo             | 26~27    | android-26, 27   | 갤럭시 S8 시리즈, A8(2018)                     |
| Android 7.0~7.1| Nougat           | 24~25    | android-24, 25   | 갤럭시 S7 시리즈, A5(2017), Note FE            |
| Android 6.0    | Marshmallow      | 23       | android-23       | 갤럭시 S6 시리즈, A7(2016), Note 5             |
| Android 5.0~5.1| Lollipop         | 21~22    | android-21, 22   | 갤럭시 S5 시리즈, A5(2015)                     |
| Android 4.4    | KitKat           | 19       | android-19       | 갤럭시 S4 시리즈, Note 3, 초기 J 시리즈        |

🔹 Android Version
일반 사용자에게 보이는 버전 이름 (예: Android 13)

🔹 API Level
개발자 관점에서 플랫폼 기능 레벨을 숫자로 표현
앱의 호환성을 판단할 때 사용됨 예: API 33 = Android 13

🔹 SDK Version
개발자가 사용하는 도구들의 버전
예: Android SDK 33은 API Level 33 기능을 포함

⚙️ 앱 개발 시 주요 설정
```
<uses-sdk
    android:minSdkVersion="23"
    android:targetSdkVersion="33"/>
```
