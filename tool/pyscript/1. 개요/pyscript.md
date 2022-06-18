# PyScript

pyscript란 anaconda에서 개발한 window용 무료 오픈소스 python 통합 개발환경으로, 
<br>
1. 브라우저에서 python을 사용가능하다.
2. python의 패키지를 사용가능하다.(numpy, pandas...)
3. python과 javascript의 objects와 namespaces가 소통가능하다.
<br>라는 장점을 내세우고 있고, 이를 이용하여 간단한 어플리케이션을 만들어보면 좋을 것 같다.
<br>


이는 python이 js에서 실행된다는 것이 아니고, WebAssembly와 Pyodide를 통해 브라우저에서 사용가능해진다

- WebAssembly<br>
  웹 어셈블리는 c나 python 과 같은 프로그래밍 언어를 컴파일링해서 바이너리형식으로 바꿔주는 기술인데, 이를 통해 python이 브라우저에서 작동하게끔 만든다.

- Pyodide <br>
  pyodide는 CPython의 포트로, python의 인터프리터이지만 웹어셈블리로 컴파일 된것이다.

사용하는 방법은 매우 간단한데,
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <script defer src="https://pyscript.net/alpha/pyscript.js"></script>
</head>
<body>
    <py-script>
        print('hello world')
    </py-script>
</body>
</html>
```
위와 같이 js파일을 가져와서 PyScript를 로딩해주면,
py-script 태그 안에서 자유롭게 파이썬이 사용가능하다.

vscode에서 작성한 후, liver server를 이용하여 열어보니

![pyscript.html](/pyscript.html.png)
<br>
와 같이 간단히 출력되었다.
<br>
\<py-env>태그를 사용하면 파이썬 파일과 다른 패키지들을 가져올 수 있다.

더 많은 예제들은
https://pyscript.net/examples/ 와 <br> 
https://github.com/pyscript/pyscript/tree/main/pyscriptjs/examples 에서 확인할 수 있다.

* pyscript는 아직 베타단계이기 때문에, 불안정하고 불완전하지만 재미있게 쓰일 것으로 보인다.