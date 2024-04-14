## 2024/04/14 - WebSocket-STOMP 구현

### STOMP

STOMP는 Simple Text Oriented Messaging Protocol의 약자이다.

간단한 메시지를 전송하기 위한 프로토콜로 메시지 브로커를와 publisher - subscriber 방식을 사용한다.

메시지의 발행자와 구독자가 존재하고, 메시지를 보내는 사람과 받는 사람이 구분되어 있다.

메시지 브로커는 발행자가 보낸 메시지를 구독자에게 전달해주는 역할을 한다.

STOMP는 HTTP와 비슷하게 frame 기반 프로토콜 command, header, body로 이루어져 있다.

### STOMP frame 구조

COMMAND

header1:value1

header2:value2

Body^@

참조 : https://growth-coder.tistory.com/157