작년에 할 땐 못봤는데 요번에 bootstrap cdn을 가지고 오려고보니 intergrity crossorigin이 새로 붙어있었다.
이유를 찾아보니 보안 때문...

W3C에서 Subresource Integrity라는 HTTP가 스크립트를 제어할 수 있는 기능을 추가했는데,
해쉬값으로 스크립트를 증명하고 해쉬값이 브라우저 값과 일치하지 않으면 실행되지 않도록 한다고 한다.

integrity는 소스코드가 조작된 경우 코드가 로드되지 못하도록 브라우저에서 체크하도록 하는 해쉬값이고
crossorigin(anonymous, use-credentials)은 요청이 same-origin이 아닌 경우, Subresource Integrity 요구사항 검사가 Cross-Origin Resource Sharing을 사용하여 로드될 수 있도록 하기 위한 것인듯..

영어를 안 읽어버릇 했더니 점점 독해력이 떨어지고 있다...ㅠㅠ

정보출처 : http://stackoverflow.com/questions/32039568/what-are-the-integrity-and-crossorigin-attribute
Subresource Intergrity 보안관련: http://blog.alyac.co.kr/321
W3C Subresource Intergrity Reference : http://www.w3.org/TR/SRI/


출처: http://ssmlim.tistory.com/27 [현실도피]
