## Step 1. /private/var/containers/Bundle/Application/target-abcd-2413
ipa 추출은 rootfull 탈옥 기긱에서..

## Step 2. /private/var/mobile/Containers/Data/Application/target-efgh-1324
Mobile -> LocalPC
```
(PC) scp -r mobile@{MOBILE-IP}:/from_mobile ./to_local
```
# Sideloadly
Sideloadly는 Windows/macOS에서 **iPhone·iPad에 IPA 파일(앱)**을 설치(사이드로딩)할 수 있게 해주는 도구입니다.
App Store를 거치지 않고도 .ipa 파일을 직접 기기에 넣는 역할을 합니다.

## 기타
+ 플러터 앱 프록시 잡기
https://blog.nviso.eu/2020/06/12/intercepting-flutter-traffic-on-ios/

+ plist 위치
/private/var/containers/Bundle/Application/[UUID]/앱이름.app/Info.plist /private/var/mobile/Containers/Data/Application/[UUID]/Library/Preferences/com.example.app.plist

+ export PS1=$'%F{green}%~%f\n%F{red}>%f

+ 재탈옥 후 sslkiller 등 트윅 설치하기
  /private/var/mobiel/Containers/Shared/AppGroup/[APP-id}/File Provider Storage/DOwnloads
+ WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED! -> ssh-keygen -R 1.1.1.34

