# 함수
## Detector 클래스
Detector 클래스는 가속도 센서와 압력감지 센서를 관리 및 관찰하며 변화를 감지합니다.

`Detector.on()`
이 함수는 감지기를 활성화하며, 백그라운드에서 센서를 확인합니다.

감지된 상황일 경우 alert() 함수를 주기적으로 실행합니다.

감지되지 않은 상황일 경우 non_alert() 함수를 주기적으로 실행합니다.

`Detector.off()`
이 함수는 감지기를 비활성합니다.

alert() 함수 내에 이 함수를 추가하면 감지가 되었을 때에 바로 감지기를 멈출 수 있습니다.


## Buzzer 클래스
부저를 관리하는 클래스입니다.

alarm 이름으로 미리 선언되어 있습니다.

`alarm.on()`

부저를 켭니다.

`alarm.off()`

부저를 끕니다.


## 기타 함수
`button()`

전면 버튼이 눌렸을 때에 실행되는 함수입니다.


# PC 시리얼 통신
`#define ENABLE_SERIAL_DEBUG`주석을 해제해서 시리얼 통신으로 값을 확인할 수 있습니다.

X가속도 Y가속도 Z가속도 가속도절대값 가속도감도 압력감도 압력값 순으로 출력합니다.

## 감도 조정
왼편 가변저항을 조절하여 인식 감도를 설정할 수 있습니다.

왼쪽 가변저항은 압력감지센서, 오른쪽 가변저항은 가속도센서 감도 설정입니다.

왼쪽으로 돌리면 민감해지고 오른쪽으로 돌리면 둔해집니다.
