<div align="center">
  <h3>Apache Jmeter에 대해 알아보자</h3>
  <img src="https://user-images.githubusercontent.com/118269278/219256599-ea7344b4-a934-436c-bc03-27a6da1d9b53.png" width=500 height=260 />
  
  <div>
    <h4>Apache Jmeter는 서버가 제공하는 성능 및 부하를 측정할 수 있는 테스트 도구이다.</h4>
  </div>
  
  <hr>
  
  <table border="1">
    <tr>
      <th><h3>Apache Jmeter의 특징</h3></th>
    </tr>
    
   <tr>
     <td><h4>1. Jmeter는 순수 Java 애플리케이션 오픈 소스이다.</h4></td>
   </tr>
   
   <tr>
     <td><h4>2. 서버나 네트워크 또는 개체에 대해 과부하를 시뮬레이션하여 강도를 테스트한다.</h4></td>
   </tr>
   
   <tr>
     <td><h4>3. 다양한 부하 유형에서 전체 성능을 분석하는 데 사용한다.</h4></td>
   </tr>
  </table>
  
  <br>
  
  <div align="left">
    <li>다양한 프로토콜/서버를 테스트할 수 있다.</li>
    <br>
    <ul>
      <ul>
        <li>웹 - HTTP, HTTPS</li>
        <li>SOAP / REST 웹 서비스</li>
        <li>FTP</li>
        <li>데이터베이스 (JDBC 사용)</li>
        <li>Mail (SMTP, POP3, IMAP)
        <li>...</li>
      </ul>
    </ul>
  </div>
  
  <br>
  
  <div align="left">
    <li>CLI 지원</li>
    <br>
    <ul>
      <ul>
        <li>CI 또는 CD 툴과 연동할 때 편리하다.</li>
        <li>UI를 사용하는 것보다 메모리 등 시스템 리소스를 적게 사용한다.</li>
      </ul>
    </ul>
  </div>
  
  <br>
  
  <div align="left">
    <li>시나리오 기반 테스트가 가능하다.</li>
    <li>다양한 외부 플러그인을 사용하여 기능 확장이 가능하다.
  </div>
  
  <hr>
  
  <div align="left">
    <h3>Apache Jmeter의 주요 개념</h3><br>
    <ul>
      <ul>
        <li>Thread Group: 몇 개의 쓰레드가 동시에 요청을 보내는 자</li><br>
        <li>Sampler: 어떤 유저가 해야 하는 액션</li><br>
        <li>Listener: 응답을 받았을 때 어떤 동작을 취하는 지 (검증, 리포트, 그래프 그리기 등)</li><br>
        <li>Configuration: Sampler 또는 Listener가 사용할 설정 값 (쿠키, JDBC 커넥션 등)</li><br>
        <li>Assertion: 응답 결과의 성공 여부를 판단하는 조건 (응답 코드, 본문 내용 등)</li><br>
      </ul>
    </ul>
  </div>
  
  <hr>
  
  <div align="left">
    <h3>Apache Jmeter 설치</h3>
    <ul>
      <h5>아래의 링크를 통해 다운로드 받으면 된다.</h5>
      <a href="https://jmeter.apache.org/download_jmeter.cgi">다운로드 하기</a><br><br>
      <img src="https://user-images.githubusercontent.com/118269278/219259921-aac0ab6b-9885-4249-9491-e73379843ace.png" width=600 height=250 /><br><br>
      위의 이미지를 참고해서 다운로드 받으면 된다.<br>
    </ul>
    
    왠만해선 환경변수를 설정을 하지 않는 이상 에러는 안날 것이다.
  </div>
  
  <hr>
  
  <div align="left">
    <h4>에러가 안나고 정상적으로 설치가 되었다면 아래의 이미지처럼 나오게 될 것이다. ↓↓</h4><br>
    <img src="https://user-images.githubusercontent.com/118269278/219260641-70104a41-26bb-4bf0-8c3a-3c93c79ddb89.png" width=650 height=290 />
  </div>
  
  <div align="left">
    <h4>Test Plan에 여러분들이 이름을 직접 정해도 된다.</h4><br>
  </div>
  
  <div align="center">
    <h2>Thread Group</h2>
    <h4>Test Plan에 이름을 지정했으면 이제 Thread Group를 설정해야 한다.</h4><br>
    <img src="https://user-images.githubusercontent.com/118269278/219262034-2fc46e0a-e4aa-402a-ab07-98f5b205dae8.png" width=650 height=290 />
  </div>
  
  <br>
  
  <div align="center">
    <h4>아래에 이미지에 Thread Properties가 가장 중요한 부분이다.</h4>
    <img src="https://user-images.githubusercontent.com/118269278/219262915-b76e7a14-7d2e-42fa-8896-28f6c53674aa.png" width=650 height=290 />
  </div>
  
  <br>
  
  <div align="left">
    <ul>
      <li>Number of Threads: 몇 개의 쓰레드(유저 수)로 테스트할 지</li>
      <li>Ramp-up period: {Number of Thread} 만큼의 쓰레드를 몇 초에 걸쳐서 만들 지</li>
      <li>Loop Count: 요청을 몇 번을 반복할지</li>
      <li>추가적으로 Action to be taken after a Sample error는 에러 처리가 되었을 때 취할 액션이다.</li>
    </ul>
  </div>
  
  <hr>
  
  <div align="center">
    <h2>Sampler</h2>
    <h4>정의했던 각각의 유저가 해야 할 일을 Sampler에서 정의한다.</h4>
    <img src="https://user-images.githubusercontent.com/118269278/219264839-50a50f5c-47d9-42db-967d-c86ba67c64ec.png" width=650 height=290 />
    <h4>위의 이미지처럼 실행이 되었다면 아래와 같이 설정 창이 노출된다.</h4>
    <img src="https://user-images.githubusercontent.com/118269278/219265626-bfbdbebf-1f82-489b-91d1-e5a189f3ebf8.png" width=650 height=290 /><br><br>
    위에 나는 저렇게 적었지만 자신의 localhost로 접속해서 사용할 수 있다.<br>
  </div>
  
  <div align="center">
    <h2>Listenr</h2>
    <h4>결과를 받고 행동을 취하는 것이 Listener이다.</h4>
    <h4>아래의 이미지처럼 4개의 Listener만 추가하면 된다.</h4>
    <img src="https://user-images.githubusercontent.com/118269278/219266634-43634a07-74d3-41ff-acd1-049274cfd407.png" width=650 height=290 />
  </div>
  
  <br>
  
  <div align="left">
    <ul>
      <li>Summary Report - 2개</li>
      <li>View Results in Table - 1개</li>
      <li>Aggregate Report - 1개</li>
    </ul>
  </div>
  
  <div align="left">
    <h4>이제 상단에 실행 버튼(초록 삼각형)을 누르면 테스트가 실행된다.</h4>
    <h4>View Results Tree에 확인하면 아래의 이미지처럼 나오게 된다면 성공한 것이다.</h4><br>
    <img src="https://user-images.githubusercontent.com/118269278/219268089-e314fcbf-3286-40f1-83f5-c0c009ba6daf.png" />
  </div>
  
  <br>
  
  <div align="left">
    <ul>
      <li><a href="https://www.apache.org/">아파치 공식문서</a></li>
      <li><a href="">Apache Jmeter 심화편</a></li>
    </ul>
  </div>
</div>
