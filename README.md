# docker 교육
## 자료
```
   - 강의자료 : https://bit.ly/202307_Docker
   - 강의소스 : https://github.com/Finfra/dockers
```
## Quickstart
```
docker search ubuntu
# docker pull ubuntu
docker run -it ubuntu
  #사용
  #exit
docker rm {컨테이너명}
docker images
docker rmi ubuntu
```

## docker 주요 명령어
### image 관리
#### rmi : 이미지 삭제
   - docker rmi $image_name
#### search : docker hub에서 이미지 검색
   - docker search $찾을이미지명
#### load : 저장된 images 파일을 불러와서 이미지로 저장
   - docker load -i $파일위치 


### 컨테이너 관련
#### 컨테이너 설치
   * docker run -it --name $컨테이너명 -v $hostos파일경로:$guestos파일경로 $
   ```
   --name : 컨테이너 명 설정
   -v : 볼륨설정
   -p : port 설정
    - -p $host_port:$container_port
      * 로컬의 8888포트를 컨테이너의 80포트로 연결
   -e : 환경변수 선언
   ```
#### run : 이미지 파일에서 신규 컨테이너 생성과 실행
   - docker run -it
#### start : 생성된 컨테이너 실행
   - docker start $컨테이너명
#### stop : 실행된 컨테이너 중지
   - docker stop $컨테이너명
#### rm : 컨테이너 삭제
   - docker rm $컨테이너명
#### attach : 실행 중인 컨테이너에 연결하여 표준 입력, 출력 및 오류를 볼 수 있도록 합니다.
#### exec : 실행중인 docker의 터미널에 접속
   * docker exec -it n1 /bin/bash
#### ctrl + p + q : 컨테이너에서의 cmd 나가기
#### docker images : docker의 images를 표기
   * tag는
   * 
#### cp : docker에 있는 파일을 복사하기
   * docker cp $컨테이너명:$컨테이너 ㅡ

#### save : 저장된 images 파일을 불러와서 이미지로 저장
   - docker load -i $파일위치 

### commit : docker를 이미지로 저장하기
   * docker commit $container $images_name:tag
### pull : docker를 hub에서 가져오기
   * docker pull $images_name:tag
##

access token Password
#### docker token
dckr_pat_pC1lVndsEl62EWtfrS1hO5xWshY
#### git token
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

## GIT 명령어
### git clone 주소명
### git add 
