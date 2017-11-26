# 네아로

## 네아로 등록

https://developers.naver.com/apps/#/register 로 들어간다

1. 다음과 같이 입력하면 등록하기 버튼이 활성화 된다.

![](/res/a.png)

2. 등록하기를 누르면 생성이 완료된다.

3. Client id와 Client secret과 생성한 애플리케이션 이름을 기억한다.

## 네아로 설정

https://developers.naver.com/docs/login/android/ 로 들어간다

1. 라이브러리에 들어가 4.2.0 zip버전을 다운로드한다.

2. zip파일에 들어가서 보면 폴더가 두가지가 있는데 4.2.0으로 된 폴더 안에 있는 sdk_4.2.0.arr을 다운로드 받는다

![](/res/1.png)

3. 다운받은 파일을 다음과 같은 경로에 넣는다.

![](/res/2.png)

4. app의 gradle에 다음과 같이 추가한다.

![](/res/3.png)

![](/res/5.png)

5. proguard를 적용한다

````
-keep public class com.nhn.android.naverlogin.** {
       public protected *;
}
````

여기까지 네이버 로그인 설정 완료