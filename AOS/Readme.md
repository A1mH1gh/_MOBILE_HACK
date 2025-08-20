# Step 1. APK 추출
+ Jadx 디컴파일러
+ MobSF
+ Drozer
  > 자세히
  > (python 2.7)
adb forward tcp:31415 tcp:31415

python -m pip install --upgrade pip
pip install protobuf pyOpenSSL twisted

drozer console connect

0) 패키지
run app.package.list
run app.package.list -f test
run app.package.manifest com.test
run app.package.attacksurface com.test

1) 액티비티
run app.activity.info -a com.test
run app.activity.start --component com.test com.test.MainActivity
run app.activity.start --component com.test com.test.MainActivity --extra strings id "meow"
1
2) 서비스
run app.service.info -a com.test
run app.service.send com.test com.test.activity

3) 브로드캐스트
run app.broadcast.info -a com.test
run app.broadcast.send --component com.test com.test.MyReceiver
run app.broadcast.send --component com.test com.test.MyReceiver --extra string phonenumber 1234 --extra string newpass a1mh1gh

4) 프로바이더
run scanner.provider.finduris -a com.test
run scanner.provider.injection -a com.test
run scanner.provider.sqltables -a com.test
run app.provider.query content://com.test.provider --projection ' (sqli 가능여부 감별)
run app.provider.query content://com.test.provider/table/index
run app.provider.update content://com.test.provider/table/index --string Password "meow"
run scanner.provider.traversal -a com.test
