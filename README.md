# response
기본적인 response.js 내용 (API 통일 전, [젤브봇](https://play.google.com/store/apps/details?id=be.zvz.newskbot) 기준)



## 사용법

response 기본 주석입니다.

```javascript
/** @param {String} room - 방 이름
  * @param {String} msg - 메세지 내용
  * @param {String} sender - 발신자 이름
  * @param {Boolean} isGroupChat - 단체채팅 여부
  * @param {Object} replier - 세션 캐싱 답장 메소드 객체
  * @param {Object} imageDB - 프로필 이미지와 수신된 이미지 캐싱 객체
  * @method imageDB.getImage() - 수신된 이미지가 있을 경우 Base64 인코딩 되어있는 JPEG 이미지 반환, 기본 값 null
  * @method imageDB.getProfileImage() - Base64 인코딩 되어있는 JPEG 프로필 이미지 반환, 기본 값 null
  * @method replier.reply("문자열") - 메시지가 도착한 방에 답장을 보내는 메소드 */
```
`room` 변수에는 방 이름이 들어있습니다.

`msg` 변수에는 메시지 내용이 들어있습니다.

`sender` 변수에는 발신자 이름이 들어있습니다.

`isGroupChat`으로 단체 채팅인지 알 수 있습니다.

`replier.reply(답장)`로 그 방에 답장을 보낼 수 있습니다.

`replier` 객체를 저장해두면 원할 때에 답장을 보낼 수도 있습니다.

