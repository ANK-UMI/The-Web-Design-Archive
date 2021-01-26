<h3>Web API(Application Programming Interfaces)</h3>
웹에는 여러 유용한 작업을 수행할 수 있는 다양한 API가 제공된다. <br>
Web API는 DOM 조작, 오디오 및 비디오 재생, 3D 그래픽 구현 등의 작업을 위해 사용한다. <br>
이러한 API는 자바스크립트(JavaScript)코드를 사용하여 접근할 수 있으며 <code>window</code>나 <code>element</code>에 대한 간단한 작업에서부터 WebGL이나 WebAudio와 같은 API를 사용해 복잡한 그래픽 및 오디오 효과를 만들어내는 것까지 가능하다. <br>
웹 코드를 작성한다면 많은 API를 사용할 수 있다. <br>
Web API는 보통 JavaScript와 함께 사용하지만, 항상 그렇지는 않다. <br>
모든 API에 대한 각각의 인터페이스는 다음 <a href="https://developer.mozilla.org/ko/docs/Web/API/Blob">색인</a>에 열거되어있다. <br>
또한 이벤트 레퍼런스에 <a href="https://developer.mozilla.org/ko/docs/Web/Events">이용가능한 모든 이벤트 목록</a>도 있다. 
문서 객체 모델(Document Object Model, DOM)은 문서를 조회하거나 수정할 수 있는 API이다.
Web API로는 크게 W3C와 크로노스의 API가 있다. <br>
W3C에는 오디오, 캔버스, CORS, DOM, DOM 이벤트, EME, 파일, Geolocation, IndexedDB, MSE, SSE, SVG, 비디오, WebRTC, 웹소켓, 웹 메시징, 웹 스토리지, 웹 워커, XMLHttpRequest 가 있다. <br>
크로노스에는 WebCL(웹 컴퓨팅 언어, 웹 가속), WebGL(Web Graphics Library)이 있다. <br>
<br>
<h3>WebCL</h3>
WebCL은 플러그인 없이 웹 브라우저만을 이용하여 별렬 컴퓨팅을 수행하기 위한 OpenCL의 자바스크립트 바인딩이다. <br>
WebCL은 OpenCL을 자바스크립트로 바이딩해서 GPU의 자원을 활용하거나 멀티 프로세스를 이용해서 병렬적인 처리를 웹 애플리케이션단에서 사용할 수 있는 기술이다. <br>
기본적으로 멀티코어 CPU와 GPU가 제 성능을 발휘할 수 있도록 해준다. <br>
웹 브라우저 안에서도 물리엔진이나 캔버스 요소 그리고 영상 편집 등 많은 계산이 필요한 컴퓨터 프로그램이 원활하게 구동되도록 해준다. <br>

<br>
<h3>WebGL</h3>
WebGL은 플러그인을 사용하지 않고 웹 브라우저에서 상호작용 가능한 3D와 2D 그래픽을 표현하기 위한 JavaScript API이다. <br>
OpenGL ES 2.0 기반의 API를 이용하여 HTML <code><canvas></code>에서 3D 랜더링을 할 수 있도록 해 준다. <br>
WebGL은 HTML5 <code><canvas></code> 요소에서 사용할 수 있는, OpenGL ES 2.0을 대부분 충족하는 API를 제공한다. <br>
현재(2020년 기준) WebGL은 Firefox 4+, Google Chrome 9+, Opera 12+, Safari 5.1+, Internet Explorer 11+, Microsoft Edge build 10240+에서 사용할 수 있다. <br>
그러나 사용자 장치의 하드웨어도 WebGL 기능을 지원해야 한다. <br>
현재 <canvas> 요소와 WebGL은 일부 오래된 브라우저에서 지원되지 않으나, 최근 버전의 모든 주요 브라우저에서 지원된다. <br>
하지만 2010년경에만 해도 WebGL을 지원하지 않는 브라우저가 많았다. <br>
따라서 당시에는 WebGL을 사용하지 않고 Canvas로 3D등을 구현하는 라이브러리를 개발하려는 시도가 있었다. <br> 
그 예로 SVG와 Canvas로 3D를 구현한 데모가 있는데 <a href="http://matthew.wagerfield.com/flat-surface-shader/'">Flat Surface Shader'</a>이라는 것이 있다. <br>
WebGL 프로그램은 JavaScript로 작성된 제어 코드와 컴퓨터의 Graphics Processing Unit(GPU)에서 실행되는 특수한 효과를 내는 코드(Shader code)로 구성된다. <br>
WebGL 요소들은 다른 HTML요소들과 섞어서 함께 사용할 수 있으며, 페이지의 다른 부분이나 페이지 배경과 함께 사용 할 수 있다. <br>
WebGL 그래픽을 그리기 위해서는 <canvas>요소를 사용해야한다. <br>
WebGL은 보는 관점에 따라 3D API로 여겨지기도 하고 rasterization engine이라고 여겨지기도 하는데 <a href="https://webglfundamentals.org/webgl/lessons/ko/webgl-2d-vs-3d-library.html">이 부분</a>에 대해서는 논란이 있다. <br>
WebGL이 3d 라이브러리가 아니라고 하는 입장에서는 OpenGL과 Three.js가 3D 라이브러리의 형태로 3D를 처리하는 반면, OpenGL ES와 WebGL은 '3D 라이브러리'와는 다른 밤주로 Canvas 2D와 유사한, rasterization 엔진일 뿐이라고 말한다. <br>
즉, WebGL이 3D API라 불리기에는, WebGL로는 3D 그래픽을 그리는 라이브러리를 작성할 수는 있지만 그 자체로 3D 그래픽을 수행하지는 않는다고 말한다. <br>
WebGL은 컴퓨터에 있는 GPU에서 실행되므로 GPU에서 실행되는 코드를 제공해야한다. <br>
해당 코드는 함수 쌍 형태로 제공해야 한다.  <br>
이 두 함수는 vertex shader와 fragment shader로 불리고 C/C++처럼 엄격한 Type을 가지는 GLSL로 작성되어 있는데 이 두 개를 합쳐서 <i>program</i>이라고 부른다. <br>
vertex shader의 역할은 vertex 위치를 계산하는 것이다. <br>
함수가 출력하는 위치를 기반으로 WebGL은 점, 선, 삼각형을 포함한 다양한 종류의 primitive들을 rasterization 할 수 있다. <br>
rasterization 할 때 primitive들은 fragment shader라 불리는 두 번째 사용자 제공 함수를 호출한다. <br>
fragment shader의 역할은 현재 그려지는 각 primitive 화소의 색상을 계산하는 것이다. <br>
<a href="https://webglfundamentals.org/webgl/lessons/ko/webgl-fundamentals.html">이 사이트</a>에서 예제를 작성하고 실행해볼 수 있다. <br>
그래픽을 그리기 전에 canvas 크기를 디스플레이 크기에 맞게 조절해야한다. <br>
CSS는 canvas가 표시되는 크기를 결정하는데, 항상 CSS로 원하는 canvas 크기를 설정해야한다. <br>
