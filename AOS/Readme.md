# Step 1. /data/app/target.com 추출
+ Jadx 디컴파일러
+ MobSF
```
docker run -it --rm -p 8000:8000 opensecurity/mobile-security-framework-mobsf:latest
```
+ Drozer
+ QARK

# Step 2. /data/data/target.com 추출

# 메모리 덤프
만약, 앱 속성 debuggable="false" 일 경우 되지 않음.<br>
python fridump3.py -u -r [PID] -s
<br>
adb shell am dumpheap <패키지명> /sdcard/app_heap.hprof

# 데이터 주고받기
tar -cvf data_data.tar /data/data/com.testapp/
tar -xvf data_data.tar

# Flutter 전용
+ reflutter
+ doldrum
+ blutter 칼리에서 진행

# blutter 사용
https://datafarm-cybersecurity.medium.com/hunting-secrets-in-flutter-applications-fed008daa60d
