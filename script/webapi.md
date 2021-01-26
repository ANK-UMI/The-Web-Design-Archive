<h3>Web API(Application Programming Interfaces)</h3>
웹에는 여러 유용한 작업을 수행할 수 있는 다양한 API가 제공된다. <br>
Web API는 DOM 조작, 오디오 및 비디오 재생, 3D 그래픽 구현 등의 작업을 위해 사용한다. <br>
이러한 API는 자바스크립트(JavaScript)코드를 사용하여 접근할 수 있으며 <code>window</code>나 <code>element</code>에 대한 간단한 작업에서부터 WebGL이나 WebAudio와 같은 API를 사용해 복잡한 그래픽 및 오디오 효과를 만들어내는 것까지 가능하다. <br>
웹 코드를 작성한다면 많은 API를 사용할 수 있다. <br>
Web API는 보통 JavaScript와 함께 사용하지만, 항상 그렇지는 않다. <br>
모든 API에 대한 각각의 인터페이스는 다음 <a href="https://developer.mozilla.org/ko/docs/Web/API/Blob">색인</a>에 열거되어있다. <br>
또한 이벤트 레퍼런스에 <a href="https://developer.mozilla.org/ko/docs/Web/Events">이용가능한 모든 이벤트 목록</a>도 있다.  <br>
문서 객체 모델(Document Object Model, DOM)은 문서를 조회하거나 수정할 수 있는 API이다. <br>
Web API로는 크게 W3C와 크로노스의 API가 있다. <br>
W3C에는 오디오, 캔버스, CORS, DOM, DOM 이벤트, EME, 파일, Geolocation, IndexedDB, MSE, SSE, SVG, 비디오, WebRTC, 웹소켓, 웹 메시징, 웹 스토리지, 웹 워커, XMLHttpRequest 가 있다. <br>
크로노스에는 WebCL(웹 컴퓨팅 언어, 웹 가속), WebGL(Web Graphics Library)이 있다. <br>
<br>
<h3>W3C Web API</h3>
.<br>
<br>
<h3>WebCL</h3>
WebCL은 플러그인 없이 웹 브라우저만을 이용하여 별렬 컴퓨팅을 수행하기 위한 OpenCL의 자바스크립트 바인딩이다. <br>
OpenCL의 자바스크립트 바인딩이라는 것은 크로노스그룹이 GPU에서 일반적인 앱을 돌리기 위해 만든 '오픈CL(OpenCL)'의 웹 플랫폼용 버전에 해당한다는 것을 뜻한다. <br>
WebCL은 OpenCL을 자바스크립트로 바이딩해서 GPU의 자원을 활용하거나 멀티 프로세스를 이용해서 병렬적인 처리를 웹 애플리케이션단에서 사용할 수 있는 기술이다. <br>
기본적으로 멀티코어 CPU와 GPU가 제 성능을 발휘할 수 있도록 해준다. <br>
웹 브라우저 안에서도 물리엔진이나 캔버스 요소 그리고 영상 편집 등 많은 계산이 필요한 컴퓨터 프로그램이 원활하게 구동되도록 해준다. <br>
<br>
<i>
일반적으로 데스크톱이나 고사양 노트북 등 x86 기반 PC 환경의 경우 GPU에 의존하기 이전에 선택 가능한 수단은 여러가지가 있다. <br>
성능이 아쉽다면 GPU 힘을 빌리지 않아도 될만큼 성능이 뛰어난 CPU를 쓰면 된다. <br>
이게 어렵다면 앱 최적화를 통해 처리 속도를 높이는 방법도 있다.<br>
그러나 브라우저 기반으로 돌아가는 웹앱에선 얘기가 달라진다. <br>
웹앱 구동 속도는 통신 환경을 제외하면 기기와 브라우저 성능에 더 크게 좌우된다. <br>
브라우저 성능은 특히 프로세서 사양이 제한적일 수 밖에 없는 모바일, 임베디드 기기에서 떨어진다. <br>
웹CL 기술을 통한 개선이 실질적인 효과를 낼 수 있는 이유다. <br>
그러나 현실은 만만치 않다. 일반 사용자들이 웹CL을 통한 웹앱 속도 개선 효과를 보려면 웹CL 표준을 따라 만들어진 웹앱과 이를 지원하는 브라우저가 필요하다. <br>
브라우저가 웹앱을 실행할 때 GPU가 CPU를 지원하도록 하자는 아이디어는 참신해 보이지만, 업계 공감대는 형성되지 않은 듯하다. <br>
미국 씨넷은 크로노스그룹은 웹앱이 그래픽칩(성능)을 훨씬 더 많이 사용할 수 있기를 희망하며 웹CL이라 불리는 API 1.0 버전을 공개했다며 하지만 대다수 브라우저 세계에서 웹CL은 큰 저항에 부닥쳤다고 지적했다. <br>
웹CL을 둘러싼 분위기는 '웹GL(WebGL)'과는 많이 달라 보인다. <br>
웹GL은 3D그래픽 처리를 빠르게 해주는 가속기술인 '오픈GL(OpenGL)'의 브라우저 버전 성격이다. <br>
웹GL의 경우 브라우저 업체들의 지지를 확보한 상황이다. <br>
현재 PC와 안드로이드용 브라우저 대부분이 웹GL을 지원한다. <br>
심지어 오픈GL과 경쟁하는 윈도 전용 그래픽API '다이렉트X'를 갖고 있는 마이크로소프트(MS)도 최신 인터넷익스플로러(IE)에선 웹GL을 지원하고 있다. <br>
크로노스그룹은 오픈GL과 웹GL, 오픈CL과 웹GL 표준화를 주도한 곳이다.  <br>
브라우저 업체들은 웹GL 도입에는 적극적이었던 반면 웹CL 도입은 소극적이었다. <br>
그리고 웹CL의 원판에 해당하는 오픈CL 기술조차 대중화되지 않은 단계로 보인다. <br>
어떤 회사도 이 기능을 언제부터 본격 상용화할 것이라고 공언하지 않았다. <br>
하지만 분위기상 모질라가 스타트를 외칠 가능성이 높아 보인다. <br>
모질라와 긴밀하게 협력 중인 삼성전자가 직접 웹CL 데모 영상을 통해 그 성능을 시연한 사례가 있고, 노키아는 파이어폭스28 버전에서 돌아가는 웹CL 구현용 확장기능을 만들어 배포 중이다. <br>
[브라우저 성능 전쟁, GPU로 확산 / 모질라, CPU+GPU 기술 '웹CL' 표준으로 고성능 추구 / 임민철 기자 입력 :2014/03/23 13:13 -- 수정: 2014/03/23 14:53]
</i>
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
그 예로 SVG와 Canvas로 3D를 구현한 데모가 있는데, <a href="http://matthew.wagerfield.com/flat-surface-shader/">Flat Surface Shader</a>라는 것이 있다. <br>
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
<br>
<h3>자바스크립트 라이브러리</h3>
자바스크립트를 이용하면 웹에 풍부한 효과를 넣을 수 있지만, 2000년대 초반만 해도 자바스크립트는 별다른 기능도 없고 성능도 별로 좋지 못했기 때문에 무시당하는 언어였다. <br>
하지만 최근 몇 년 사이 다양한 자바스크립트 프레임워크와 라이브러리가 생기면서 자바스크립트 생태계가 크게 확장되는 추세이며 그 위상도 높아지고 있다. <br>
자바스크립트는 1995년 브랜든 아이크에 의해 처음 개발되었다. <br>
그는 1995년 넷스케이프에 근무하면서 자바스크립트 개념을 만들었다. <br>
처음에는 '모카'라고 불리다가 이후 '라이브 스크립트'라고 불렸는데, 당시 자바가 큰 인기를 끌자 마케팅 효과를 노려 자바스크립트로 명칭을 변경하였다. <br>
이후 자바스크립트 기술이 발전했고 이에 대한 표준과 명세를 ECMA 인터내셔널에서 관리하고 있다. <br>
1998년 그는 웹 개방성을 옹호하는 모질라 프로젝트를 새로 시작했고, ‘파이어폭스(FireFox)’라는 웹브라우저를 만들었다.  <br>
이후 모질라에서 개발하는 기술은 그가 총괄하게 된다.  <br>
이러한 이유로 자바스크립트와 관련해 다양하고 자세한 문서를 모질라 커뮤니티 홈페이지에서 볼 수 있다. <br>
자바스크립트는 컴파일 과정이 없기 때문에 다른 언어와 비교했을 때 빠른 시간 안에 스크립트 코드를 작성할 수 있게 도와준다는 장점이 있다. <br>
기존 C나 자바 언어와 달리 굉장히 단순한 구조와 원칙을 가지고 있기 때문에 초보 개발자들이 쉽게 배우고 이해할 수 있다. <br>
예를 들어 자바스크립트 코드 안에서는 변수, 클래스 및 메소드를 선언하지 않아도 되고, 메소드가 ‘public’, ‘private’ 또는 ‘protected’인지 구분하지 않아도 된다. <br>
자바스크립트는 웹에 특화된 기술이기 때문에 운영체제나 플랫폼에 상관없이 잘 작동되고 확장성도 높다. <br>
단점이 있다면 바로 성능과 보안이다. <br>
내부에서 제공되는 기능이 제한적이며 관련된 개발도구가 적은 편이다. <br>
또한 자바스크립트는 HTML 소스코드에 함께 작성되면서 소스코드가 외부로 공개되는데, 이 과정에서 보안 취약점이 발생할 수 있다. <br>
최근에는 자바스크립트 관련 라이브러리나 프레임워크가 개발자들 사이에서 화제가 되었다. <br>
위키피디아에 올라온 '<a href="https://www.wikiwand.com/ko/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8_%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC_%EB%AA%A9%EB%A1%9D">자바스크립트 라이브러리 목록</a>'을 보면 관련된 기술이 90여개인데다 데이터과학, 이용자 조작화면(UI), 서버 등 활용 분야가 다양하다. <br>
디자이너들은 '자바스크립트 그래픽스 라이브러리' 목록에서 '그래픽/시각화 (캔버스 또는 SVG 관련)' 관련 라이브러리를 많이 활용한다. <br>
해당 목록을 보면 디자이너들이 자주 사용하는 라이브러리로는 p5.js, Paper.js, Processing.js 등이 있는데, 이들은 주로 인터랙티브한 2D 모션그래픽에 최적화된 도구로 보인다. <br>
가장 많이 쓰이는 3D 자바스크립트 라이브러리로는 
<a href="https://threejs.org/">Three.js</a>, 
<a href="https://www.babylonjs.com/">Babylon.js</a>, 
<a href="http://www.cannonjs.org/">Cannon.js</a>, 
<a href="https://www.ambiera.com/copperlicht/">CopperLicht</a>, 
<a href="http://www.kevs3d.co.uk/dev/phoria/">Phoria.js</a>, 
<a href="https://github.com/xeolabs/scenejs">Scene.js</a>, 
<a href="https://github.com/d3/d3">D3.js</a>, 
<a href="https://github.com/evanw/lightgl.js">LightGL.js</a>, 
<a href="http://seenjs.io/index.html">Seen.js</a> 
등이 있다. <br>
이 중, 최근까지 꾸준하게 업데이트되고 강력하게 사용되는 툴은 Three.js와 Babylon.js이다. <br>
<br>
<h3>그외 플러그인</h3>
<h4>어도비 플래시</h4>
벡터 그래픽스, 애니메이션, 비디오, 소리와 같은 복잡한 미디어를 제작하기위해 플래시, 퀵타임, 자바 런타임 환경 등과 같은 별도의 플러그인을 사용하기도 한다. <br>
<a href="https://www.blog.google/products/chrome/saying-goodbye-flash-chrome/">어도비 플래시는 2020년 현재 지원이 중단되었다. </a>
지난 20년 동안 Flash는 웹에서 게임을 하고 비디오를 보고 응용 프로그램을 실행하는 방식을 형성하는데 큰 도움이 되었다. <br>
초반에는 데스크톱 Chrome 사용자의 80%가 매일 Flash를 포함하고 있는 사이트를 방문했으나 지원 종료 3년전부터 사용량은 17%로 감소했다. <br>
이러한 추세는 웹 사이트가 Flash보다 더 빠르고 효율적인 개방형 웹 기술로 대체(migration)되고 있다는 것을 보여준다. <br>
Chrome은 2017년 7월, 2017년부터 몇 년 동안 계속해서 Flash를 단계적으로 중단하고 결국 비활성화하여 2020년 말에는 Chrome에서 Flash를 완전히 제거할 예정이라고 밝혔다. <br>
사이트에서 계속 Flash를 사용하고 사이트에 Flash 실행 권한을 부여하면 2020 년 말까지 작동한다고 한다. <br>

