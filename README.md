# sm_week06
스마트모바일프로그램설계 6주차

5주차 팀 프로젝트 활동 : https://github.com/Kim-KyungJin/sm_week05

### 팀 구성   
스마트정보통신공학과 201621216 이준석   
스마트정보통신공학과 201921036 김경진   
스마트정보통신공학과 201921054 박유리   
스마트정보통신공학과 201921083 이혜정   
스마트정보통신공학과 201921104 홍수빈    
스마트정보통신공학과 201990009 미르자크메더브 사르더르    

   ***   
### 모든 항목은 변경되거나 삭제될 여지가 있습니다   
   ***   
   
### 5주차 보완   
>진행과정   
>각자 진행하여 만들어둔 레이아웃 파일을 앱의 테마에 맞추어 색과 이미지들을 통일하는 작업을 해주었습니다.  
>페이지의 이동을 임시로 제작한 mainActivity를 기준으로 간단하게 나타내었습니다.

 
>[통합 테마 영상](https://user-images.githubusercontent.com/57963888/114380008-8445e300-9bc4-11eb-80e7-42a8eb5c74ab.mp4)   


>음식점 게시판   
>![KakaoTalk_20210412_183849597](https://user-images.githubusercontent.com/57963888/114380001-8314b600-9bc4-11eb-83ab-72fe42859c7d.png)   

>마이페이지   
>![KakaoTalk_20210412_183904789](https://user-images.githubusercontent.com/57963888/114380006-83ad4c80-9bc4-11eb-9f2f-747e074d68c8.png)   
>>*마이페이지 같은 경우에는 배달 어플의 UI를 참고하여 비슷하게 만들 예정입니다.*   
>>![KakaoTalk_20210412_160004830](https://user-images.githubusercontent.com/57963888/114385351-e570b500-9bca-11eb-859d-40aabfdd86db.jpg)   

>정보수정   
>![KakaoTalk_20210412_183823464](https://user-images.githubusercontent.com/57963888/114380016-860fa680-9bc4-11eb-8bba-f82150622b34.png)   



***   

### 데이터베이스 연동   
>진행과정1   
>회원가입 후 로그인 하는 과정에서, 데이터베이스에 데이터를 추가하고 데이터를 불러오는 기능도 넣었습니다.   
>>[회원가입&로그인 영상](https://user-images.githubusercontent.com/57963888/114373417-82c4ec80-9bbd-11eb-9670-c00b35f7d66d.mp4)   
>>>![RegisterActivity1](https://user-images.githubusercontent.com/79889548/114402238-95035280-9bde-11eb-8e75-23c22a98bd2d.PNG)   
>>>![RegisterActivity2](https://user-images.githubusercontent.com/79889548/114402241-96347f80-9bde-11eb-8e53-01d4bcb6572c.PNG)   
>>>![RegisterRequest](https://user-images.githubusercontent.com/79889548/114402242-96347f80-9bde-11eb-90fb-5020e52346ac.PNG)   
>원래는 사용하기에 익숙한 Mysql로 개발하려고 했지만, 동시접속이 불가능하다는 점과 실시간으로 데이터가 이동하지 않는다는 것을 알고  
>이 단점들을 보완할 데이터베이스를 사용하기로 하였습니다.   
>다음 주부터 Mysql로 조작하던 데이터를 Firebase를 사용하여 데이터를 관리하려고 합니다.   

>진행과정2   
>처음 써보는 데이터베이스라서 연습삼아 데이터 테이블과 속성들을 입력해보았습니다.   
>>![image](https://user-images.githubusercontent.com/57963888/114385784-662fb100-9bcb-11eb-98f3-bf8f04b6650c.png)   
>>![image](https://user-images.githubusercontent.com/57963888/114385856-79428100-9bcb-11eb-88a7-f05b1007d82b.png)   
>이러한 데이터 테이블 및 투플들을 생성하고 관리할 예정입니다.   

>![image](https://user-images.githubusercontent.com/57963888/114386304-038ae500-9bcc-11eb-9321-7bfa2c56c9df.png)   
>>연습용 코드로 데이터를 생성하려고 했지만 오류를 고칠 수 없어서 팀원들과 의논 중에 있습니다.  
>>익숙하지 않은 데이터베이스이고 문법도 생소해서 적응하는 데에 시간을 많이 들여야 할 거 같습니다.   


***

### UI 합체 시도
>저번 주차에 각자 나눠서 작업했던 activity들을 합치는 과정 중 똑같은 버그의 반복 발생으로 인해 해결방안을 찾고있습니다.   
>정확한 원인은 모르지만 내부함수와 작성한 함수가 충돌하는 듯해 보입니다.   
>원래 로그인을 누르면 프래그먼트와 함께 activity_nav_activity.xml 화면이 나와야하는데 튕기는 증상을 보입니다.   
>![20210412_224206](https://user-images.githubusercontent.com/76034369/114404102-5cfd0f00-9be0-11eb-9b23-3f40a5238ac8.png)   

>[문제 상황 영상](https://user-images.githubusercontent.com/57963888/114407216-22e13c80-9be3-11eb-96c9-a141cde5b8be.mp4)   
>> 문제 상황 영상   

>[정상적 동작 영상](https://user-images.githubusercontent.com/57963888/114406697-b5351080-9be2-11eb-8f39-3702d7ef784f.mp4)   
>>정삭적으로 보여져야할 모습    



***


### 업주 관련 UI
>진행과정
>>가게관련 페이지 구성해봤습니다  (tab 부분, 영화관, 옷가게 및 등 페이지와 똑같이 쓸 수 있게 코드를 써 봤습니다)   

>activity_main.xml   
>>![activity_main](https://user-images.githubusercontent.com/79883669/114404324-8fa70780-9be0-11eb-8ff7-5dab81a973dc.png)   

>AndroidManifiest.xml의 application 부분 (다음 주까지 완성할 예정)   
>>![manifiest_application 부분](https://user-images.githubusercontent.com/79883669/114404687-e7457300-9be0-11eb-8cdb-6bfb09df092a.png)   


