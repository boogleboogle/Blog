# Windows 10용 Internet Explorer 11 지원 종료

[2022년 6월 15일 부로 microsoft에서 제공하는 internet explorer가 종료된다.](https://docs.microsoft.com/ko-kr/lifecycle/announcements/internet-explorer-11-end-of-support)
대신에 Edge가 있으니까, 혹은 crome을 사용하고 있으니까 상관 없을 수도 있다.

microsotf는 왜 지원을 종료하는지 찾아 봤다. ([참고](https://blogs.windows.com/wp-content/uploads/prod/sites/2/2021/05/Microsoft-Edge_Korean-Blog-and-FAQ-1.pdf))
1. 개선된 호환성: Microsoft Edge가 크로미엄(Chromium) 프로젝트 상에서 구축되었기 때문에 모던 웹사이트에 대한 세계 최고 수준의 지원을 제공한다.
2. 간결함을 통한 생산성 향상: Edge가 듀얼 엔진으로 간결함을 제공해
생산성을 향상한다.
3. 강력한 브라우저 보안성: Edge는 Microsoft Defender SmartScreen의 업계 최고 등급 피싱 및 맬웨어 차단 기능을 바탕으로 사용자를 보호, 사용자의 개인 자격 증명이 손상된
경우에는 Password Monitor를 통해 다크 웹을 스캔한다.
---
그렇다고 internet explorer를 아예 사용 불가능 한 것은 아니다.
edge에 [IE모드]((https://www.microsoft.com/ko-kr/edge/business/ie-mode)를 사용 할 수 있고, 이는 최소 2029년 까지 지원된다고 한다.

---
개인의 경우는 IE에서 Edge로 변경하면 간단하겠지만,
개발자들은 어떨까?

개발자 커뮤니티에서는 환영하는 분위기다.
internet exploer로 작업하는것이 점점 더 어려워졌기 때문이다.

---
그럼에도 IE를 사용하던 여러 플랫폼들은 곤란하지 않을까?
microsoft에서는 <br>

영향을 받는:

    • 반기 채널 (SAC- semi-annual channel)을 통해 제공되는 Internet Explorer 11 데스크톱 응용 프로그램:
        • Windows 10 desktop SKUs (20H2+)
        • Windows 10 IoT (20H2+)

영향을 받지 않는:

    • Microsoft Edge의 Internet Explorer 모드
    • Internet Explorer 플랫폼 (MSHTML / Trident)
    • Internet Explorer 11 데스크톱 응용 프로그램:
        • Windows 8.1
        • Windows 7 ESU
        • Windows 10 Server SAC (all versions)
        • Windows 10 IoT LTSC (all versions)
        • Windows 10 Server LTSC (all versions)
        • Windows 10 client LTSC (all versions)

이라고 말했다. <br>
또한 Windows 10 LTSC 및 서버는이 변경에 영향을 받지 않는다고 한다.

---

또 종료될 서비스는 없을까? <br>
[제품 및 서비스 수명 주기 정보 검색](https://docs.microsoft.com/ko-kr/lifecycle/products/)에서 자세한 사항을 확인 할 수 있고,
현재 출시 된 Windows 버전의 서비스 종료 날짜는 아래와 같다.
![마이크로 소프트 서비스 종료 예정일](../tech%20news/microsoft%20End%20of%20Support%20Date.png)

---

자세한 사항은 [여기](https://blogs.windows.com/wp-content/uploads/prod/sites/2/2021/05/Microsoft-Edge_Korean-Blog-and-FAQ-1.pdf)를 참고