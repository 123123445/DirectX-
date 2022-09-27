# DirectX
마이크로소프트 플랫폼에서 컴퓨터 그래픽스 작업을 위한 API의 집합이다.<br>
3차원 그래픽 하드웨어를 사용하여 높은 품질의 3차원 그래픽을 빠르게 렌더링할 수 있다.<br><br>
게임과 그래픽카드가 소통할 수 있게끔 해주는 연결다리의 역할을 한다<br><br>
<h3>구성요소</h3>
- <b>Direct2D</b> : DirectX 10.1 표준에 포함된 2D 그래피 표현 API이다. GDI, GDI+를 대체한다.<br><br>
- <b>Direct3D</b> : 3D 그래픽을 렌더링하는 데 쓰인다.<br><br>
- <b>XInput</b> : Windows 크로스 플랫폼 표준 입력(키보드, 마우스, 조이스틱 등)의 API이다. Windows및 XBox360을 지원하며   XBox360 전용 콘트롤러 및 고유한 기능(버튼, 진동 등)을 Windows에서도 사용할 수 있다.<br><br>
- <b>DirectMusic</b> : 다이렉트 뮤직 프로듀서에 의해 만들어지는 사운드 트랙 재생이다.<br><br>
- <b>DirectAudio</b> : 게임 중 음향 효과에 쓰인다. <br><br>
- <b>DirectWrite</b> : DirectX 10.1 표준에 포함된 글꼴 표현 API이다.<br><br>
- <b>DirectShow</b> : 동영상같은 멀티미디어 재생 API이다. 현재는 Windows SDK에 포함된 상태이다.<br><br>
- <b>DirectPlay</b> : 네트워크 게임을 위한 API를 제공한다.<br><br>
- <b>DirectCompute</b> : DirectX 11에 포함된 그래픽 프로세서를 통한 범용 연산 API이다.<br><br>

<h3>Direct3D의 렌더링방식</h3>
이중버퍼링을 하며 front 버퍼와 back 버퍼 두 개의 버퍼를 이용하여 렌더링한다. 먼저 front 버퍼를 화면에 나타내고 back 버퍼의 내용은 모두 지우고 출력을 back 버퍼에 한다. 이와같은 과정을 거친 후에 front 버퍼와 back 버퍼이 역할을 바꿔 다시 화면에 다음 장면을 출력하는 페이지플리핑(pageflipping)의 방식으로 렌더링한다<br><br>
