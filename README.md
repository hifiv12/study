## The Basics of React
1. React Element
  - html + css + javascript 의 3가지 언어로 웹페이지를 컨트롤을 하는게 기존의 방법
  - React.js 는 javascript로만 html, css, javascript를 한번에 컨트롤 할 수 있게 함
  - ReactDOM.render를 통해 데이터를 전달하여 생성 또는 업데이트를 할 수 있다. 
  - 코드가 한눈에 들어온다는게 장점
  - const var_name = React.createElement ("tag_name", {props}, innerText);
    * {props} 의 태그는 일반적인 태그로 들어가는 속성들을 작성하는 곳

2. Events in React
  - 기존의 방식 > html 태그를 생성 후 이벤트를 호출 > javascript에서 이벤트리스터 명시
  - Reactjs > javscript에서 태그 생성 및 프로퍼티로 이벤트 생성 및 호출
  - React.createElement로 하나의 태그가 아닌 2개 이상을 생성하고 싶다면 변수에 미리 담아놓은 다른 createElement의 변수를 마지막 파라미터로 [] 배열의 형태로 작성하면 된다.

3. JSX
  - 익숙한 방식의 html tag 구조로 script 태그 내에 작성하기 위한 javascript 확장언어
  - cdn : <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>  
  - <script type="text/babel"></script>
  - onClick 등의 이벤트 함수를 불러올 땐 onClick={ () => ___ } 으로 중괄호 안에 작성
  - 2개 이상의 엘리먼트를 하나로 담을 때는 컴포넌트의 형태로 나타내 태그에 포함시킨다.
    * 작성된 엘리먼트는 함수의 형태로 바뀌어야 됨
    * ReactDOM.render에 담기 전 <Component_name /> 로 담아야 되며 첫글자는 대문자로 작성된다.
  - 컴포넌트는 무조건 첫글자는 대문자

4. Understanding State