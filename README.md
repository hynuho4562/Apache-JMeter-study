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
      <img src="https://user-images.githubusercontent.com/118269278/219259921-aac0ab6b-9885-4249-9491-e73379843ace.png" width=700 height=450 /><br><br>
      위의 이미지를 참고해서 다운로드 받으면 된다.<br>
    </ul>
    
    왠만해선 환경변수를 설정을 하지 않는 이상 에러는 안날 것이다.
  </div>
  
  <hr>
  
  <div align="left">
    <h4>에러가 안나고 정상적으로 설치가 되었다면 아래의 이미지처럼 나오게 될 것이다. ↓↓</h4><br>
    <img src="https://user-images.githubusercontent.com/118269278/219260641-70104a41-26bb-4bf0-8c3a-3c93c79ddb89.png" />
  </div>
</div>
