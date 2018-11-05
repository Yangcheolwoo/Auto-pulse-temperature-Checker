
2018 11 05 11주차 ( 실습 예상 보고서)

(+박한샘) 1. 프로젝명 : Auto-pulse-temperature-Checker 
2. 금주 실습할 내용 
o 실습명 : lm35 dz 온도센서 3개와 부저센서 3개 작동여부 확인, 플라스크 서버 구축
o 실습절차
가.lm35 온도센서 작동여부 확인 후 측정값 오차범위 줄이기
나.부저센서 작동여부 확인
다.ip타임 포트포워딩 하기.
라.플라스크 서버 구축 


3. 예상 결과
-센서 오류 발생 (여분으로 대체)
-포트포워딩 설정 완료
-플라스크 서버 구축 오류 ( 구글링으로 해결 가능)

4. 관련 링크
1.ipTime 포트포워딩 : http://wassap.tistory.com/168?fbclid=IwAR34IeMo9UqFi2cF614kHm0kw5xBhZgm3-_hTTt3nLaN0IMAYVjK10kWbXM
2.플라스크 서버 구축 : http://readystory.tistory.com/10?fbclid=IwAR1FMpo8L7HL4Iz6VHumsYB5aFb23p1oJgDLaHABZUpczNnjn5C9XMAgfOQ

3.책 참고 (플라스크 웹 개발 - 미구엘 그린버그) 


---------------------------------------------------------------------------------------------------------------------------------------
2018 11 01 10주차 (실습 보고서)

양철우 (+박한샘) 1. 프로젝명 : Auto-pulse-temperature-Checker 
2. 금주 실습할 내용 
o 실습명 : NodeMcu(온습도센서)와 라즈베리파이MQTT통신
o 실습절차
가.라즈베리파이에 Mosquitto 설치
나.NodeMCU에서 아두이노 스케치에 PubSubClient(MQTT)관련 라이브러리 설치
다.라즈베리파이와 NodeMCU 같은 공유기에 WiFi연결
라.핸드폰 어플 중 Mqtt앱을 설치
마.핸드폰 앱으로 NodeMCU에서 설정한 토픽이름을 써서 온습도값 받기

3. 결과
-라즈베리파이 MQTT설치 후 NodeMCU에서 보내주는 온습도 값을 핸드폰 MQTT앱으로 값 받기 성공

4. 소감 및 질문 
라즈베리파이 MQTT설치후 NodeMCU에 공유기 WiFi 이름과 비밀번호, 라즈베리파이 IP주소 업로딩을 하고 통신을 시작할려고 할때 NodeMCU 씨리얼 모니터에 disconnect라는 문구가 계속 떠 있었다. 이것저것 다시 코딩해보고 하다가 WiFi 5GHz가 아닌 WiFi 2.4GHz로 연결을 했을 때 연결되었다는 메세지가 씨리얼 모니터에 나타나게 되었다. WiFi 주파수 대역도 영향을 끼친다는 것을 알게 되었다. 이제 서버 구축 후 서버쪽에서 구독하는 방법에 대해 생각해 봐야겠다.

o 관련 링크
-Mosquitto 설치 : https://blog.naver.com/roboholic84/221227871374
-NodeMCU(온습도센서) 스케치 코딩: https://blog.naver.com/PostView.nhn?blogId=roboholic84...

--------------------------------------------------------------------------------------------------------------------------------------

2018 10 29 10 주차 ( 실습 예상 보고서)
1. 프로젝명 : Auto-pulse-temperature-Checker 
2. 금주 실습할 내용 (+박한샘)
o 실습명 : NodeMcu(온습도센서)와 라즈베리파이MQTT통신
o 실습절차
가.라즈베리파이에 Mosquitto 설치
나.NodeMCU에서 아두이노 스케치에 PubSubClient(MQTT)관련 라이브러리 설치
다.라즈베리파이와 NodeMCU 같은 공유기에 WiFi연결
라.핸드폰 어플 중 Mqtt앱을 설치
마.핸드폰 앱으로 NodeMCU에서 설정한 토픽이름을 써서 온습도값 받기

o 예상 결과
-라즈베리파이의 Mosquitto 설치문제가 생길 수 있다. - SD카드초기화 후 다시 설치하여 문제 해결가능
-NodeMCU 아두이노 스케치의 코팅 오류문제가 나올 수 있다. - 오류부분 구글링하여 문제해결 가능
-NodeMCU의 고장의 원인으로 통신문제가 발생할 수 있다. - 다른 NodeMCU로 교체

o 관련 링크
-Mosquitto 설치 : https://blog.naver.com/roboholic84/221227871374
-NodeMCU(온습도센서) 스케치 코딩: https://blog.naver.com/PostView.nhn?blogId=roboholic84...



--------------------------------------------------------------------------------------------------------------------------------------


필요한 부품:
1.TMP36 온도센서 3개. http://itempage3.auction.co.kr/DetailView.aspxitemno=A868357606

2.nodeMcu - 4개   http://m.devicemart.co.kr/1385151 

3.FQ-050 부저센서 - 3개  http://m.devicemart.co.kr/1361134

4.pulse sensor - 2개  http://m.devicemart.co.kr/1174964


학교에 있으면 안사도 되는물품:

1.점프선 암 수   http://www.devicemart.co.kr/1321195 품절 20cm  31일 입고 예정
                http://www.devicemart.co.kr/1328408 10cm

3.점프선 수 수  http://www.devicemart.co.kr/1321196 20cm

4.점프선 수 수 http://www.devicemart.co.kr/1328409 품절 23일 입고 예정 10cm

5.저항   http://www.devicemart.co.kr/886 

6.브레드보드 3개   http://www.devicemart.co.kr/1328148


# Auto-puslse-tamperature-Checker
![image](https://user-images.githubusercontent.com/32381811/46915443-deab5c00-cfe6-11e8-873d-3728c5e3ee33.png)
![image](https://user-images.githubusercontent.com/32381811/46915445-e10db600-cfe6-11e8-989a-514f4dfebaae.png)
![image](https://user-images.githubusercontent.com/32381811/46915448-e2d77980-cfe6-11e8-8c17-883b059cd6e6.png)
![image](https://user-images.githubusercontent.com/32381811/46915449-e4a13d00-cfe6-11e8-93f8-ffb4ce2a1072.png)
![image](https://user-images.githubusercontent.com/32381811/46915450-e7039700-cfe6-11e8-847a-d5a0f1515366.png)
![image](https://user-images.githubusercontent.com/32381811/46915452-e9fe8780-cfe6-11e8-8811-8607b976cf9a.png)
![image](https://user-images.githubusercontent.com/32381811/46915454-ebc84b00-cfe6-11e8-864e-a74ffa0a5cd6.png)
![image](https://user-images.githubusercontent.com/32381811/46915456-eec33b80-cfe6-11e8-9858-b56d7b2956d6.png)
![image](https://user-images.githubusercontent.com/32381811/46915459-f1259580-cfe6-11e8-9edf-9e2eab7891df.png)
![image](https://user-images.githubusercontent.com/32381811/46915460-f4208600-cfe6-11e8-96ea-e7381ec76cd6.png)
![image](https://user-images.githubusercontent.com/32381811/46915461-f8e53a00-cfe6-11e8-91fb-b57154261c62.png)
![image](https://user-images.githubusercontent.com/32381811/46915464-000c4800-cfe7-11e8-935b-fe4d064c5cd9.png)
![image](https://user-images.githubusercontent.com/32381811/46915470-0d293700-cfe7-11e8-917f-df6786b0574d.png)

맥박센서 : http://deneb21.tistory.com/391
플라스크 서버 : http://orangineer4.blogspot.com/2017/08/raspberrypi.html
