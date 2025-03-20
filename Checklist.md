# 리패키징
```
java -jar apktool_2.5.0.jar d test.apk -o test
```
```
java -jar apktool_2.5.0.jar b test
java -jar apktool_2.5.0.jar b test --use-aapt2 //brut.androlib.AndrolibException: brut.common.BrutException: could not exec (exit code = 1) 오류 시 사용
```
```
java -jar uber-apk-signer-1.2.1.jar -a login\dist\login.apk
```
