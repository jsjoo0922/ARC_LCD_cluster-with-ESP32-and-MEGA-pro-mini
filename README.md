# ARC_LCD_cluster-with-ESP32-and-MEGA-pro-mini
similar with only ESP32 base system. But Mega shoot CAN analysis info to ESP32 with UART network. 
ESP32 와 아두이노 MEGA 2560 을 함께 쓰는 구조입니다.
ESP32는 UI제어만, MEGA는 CAN 분석만 전담하는 분할구조입니다.
두 MCU는 TX, RX를 이용한 UART통신으로 작동합니다.
ESP32의 부담을 감소시키고, UI의 다양성 확보를 위해 구상하였습니다.
나이트모드, Sports모드, 에코모드 등의 여러 테마 대응을 기대하고 있습니다.
또한 CAN ID 및 데이터가 정리되는대로 MEGA에 최신화하여 추후 각종 기능을 담은 모듈에 대응하기 위해 CAN분석허브로 응용할 계획입니다.

사용 부품 (ui 부문)
  1. ESP32
  2. GC981A01
  3. 조도센서 (디지털 출력을 지원하는 광포토셀)
  4. 7핀 커넥터 하네스

사용부품 (CAN 해석 부문)
  1. 아두이노 MEGA 2560 PRO MINI
  2. MCP2515
  3. 3핀 커넥터 하네스
  4. 12v-5v DCDC컨버터 (차량의 출력전원 직접인가 목적)
  5. 레벤 컨버터 (MEGA에서 5V로 출력되는 신호를 스텝다운 목적)

(아직 열심히 구상중입니다.)
