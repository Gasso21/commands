- 맥에서 SCP 사용하기
1. 맥에서 원격지 서버로 파일 전송
$ scp -p -r "파일이름" "원격지서버UserID"@"IPAddress":"원격지서버 디렉토리"

2. 원격지 서버에서 맥으로 파일 전송
$ scp -p -r "원격지서버UserID"@"IPAddress":"원격지서버 디렉토리(파일)" "저장할 로컬 디렉토리"

"""
-p : 원본파일의 변경 시간, 접근 시간, 퍼미션 보존
-r : 하위 디렉토리 및 파일까지 복사
-P : <Port>포트 지정, SSH포트가 22번이 아닐 때 사용
"""

- 맥에서 크램쉘모드 사용
1. 잠자기 모드 Off
$ sudo pmset -b disablesleep 1

2. 잠자기 모드 On
$ sudo pmset -b disablesleep 0

"""
pmset : Power Management Setting
-a : 모든 상황에서 동일하게 잠자기를 금지 혹은 허용
-b : 배터리 상태일 때 적용
-c : 충전 상태일 때 적용
-u : ups 상태일 때 적용