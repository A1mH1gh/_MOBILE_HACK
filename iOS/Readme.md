## Step 1. /private/var/containers/Bundle/Application/target-abcd-2413
ipa 추출은 rootfull 탈옥 기긱에서..

## Step 2. /private/var/mobile/Containers/Data/Application/target-efgh-1324
Mobile -> LocalPC
```
(PC) scp -r mobile@{MOBILE-IP}:/from_mobile ./to_local
```
## 기타
+ 플러터 앱 프록시 잡기
https://blog.nviso.eu/2020/06/12/intercepting-flutter-traffic-on-ios/

+ plist 위치
/private/var/containers/Bundle/Application/[UUID]/앱이름.app/Info.plist /private/var/mobile/Containers/Data/Application/[UUID]/Library/Preferences/com.example.app.plist

+ export PS1=$'%F{green}%~%f\n%F{red}>%f

+ 재탈옥 후 sslkiller 등 트윅 설치하기
  /private/var/mobiel/Containers/Shared/AppGroup/[APP-id}/File Provider Storage/DOwnloads
