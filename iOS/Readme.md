## Step 1. /private/var/containers/Bundle/Application/target-abcd-2413
Mobile -> LocalPC
```
scp -r mobile@192.168.219.124:/private/var/containers/Bundle/Application/A0E01AC8-6F1A-4709-A18D-34CF0D328A40 ./
```

## Step 2. /private/var/mobile/Containers/Data/target-efgh-1324

## 기타
+ 플러터 앱 프록시 잡기
https://blog.nviso.eu/2020/06/12/intercepting-flutter-traffic-on-ios/

+ plist 위치
/private/var/containers/Bundle/Application/[UUID]/앱이름.app/Info.plist /private/var/mobile/Containers/Data/Application/[UUID]/Library/Preferences/com.example.app.plist
