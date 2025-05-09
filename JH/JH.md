- 자전거 대여 정보 조회
회원이 현재 대여 중인 자전거를 조회하면 해당 리스트가 출력되고 각 항목에는 대여소 이
름, 대여소 위치, 자전거 ID, 자전거 제품명, 자전거 유형을 보여 준다.
- 자전거 예약대기 정보 조회/취소
회원이 자전거 예약대기 정보(대여소 이름, 대여소 위치, 자전거 ID, 자전거 제품명, 자전
거 유형)를 조회하면 해당 리스트가 출력된다. 또한, 각 예약대기에 대해 취소할 수 있다.
- 자전거 반납 및 식당 예약 서비스 연계 기능
회원은 자전거 대여 정보 조회 화면에서 특정 자전거를 지정된 대여소에 반납할 수 있다.
자전거 반납 후에는 원하는 경우 사용자 위치 정보를 기반으로 근처 식당을 추천받아서 예
약할 수 있는 외부 서비스와 연결된다. 해당 자전거에 대기 예약한 회원이 있는 경우 대기
1순위 회원에게 예약되었다 는 이메일을 보낸다.

| 순서 | 요구사항 | 유즈케이스 |
| --- | --- | --- |
| 1 | 회원은 현재 대여 중인 자전거를 조회하면 해당 자전거 목록을 볼수있다. | 자전거 대여 정보 조회 |
| 2 | 회원은 해당 자전거 목록에서 대여소 이름, 대여소 위치, 자전거ID, 자전거 제품명, 자전거 유형을 볼수있다. | 자전거 대여 정보 조회 |
| 3 | 회원은 자전거 예약대기 정보를 조회할수있다. | 자전거 예약대기 정보 조회/취소 |
| 4 | 회원은 자전거 예약대기 정보를 조회하고 대여소 이름, 대여소 위치,자전거 ID, 자전거 제품명, 자전거 유형 리스트를 볼수있다. | 자전거 예약대기 정보 조회/취소 |
| 5 | 회원은 각 예약대기에 대해 취소를 할수있다.  | 자전거 예약대기 정보 조회/취소 |
| 6 | 회원은 특정 자전거를 지정된 대여소에 반납할 수있다. | 자전거 반납 |
| 7 | 회원은 자전거 반납 후 원하는 경우 사용자 위치 정보를 기반으로 식당을 추천받을수있다. | 식당 예약 서비스 연계기능 |
| 8 | 회원은 근처 식당을 추천받아서 예약할수있는 외부 서비스와 연결된다. | 식당 예약 서비스 연계기능 |
| 9 | 회원은 해당 자전거에 대기 예약한 회원이 있는 경우 대기 1순위 회원에게 예약되었다는 이메일을 받을수있다. | 이메일 서비스 |


| Actor Action | System Response |
| --- | --- |
| 1. 회원은 검색된 특정 대여소를 선택 | 2. 상세정보화면을 출력 |
| 3. 남아 있는 자전거 즉시 대여 | 4. 대여 완료 문자 |
| 5. 자전거가 없는 경우 예약 대기신청 | 6. 예약대기 완료 문자 |
| 7. 자전거 예약대기 정보 입력 | 8. 해당 리스트 출력 |
| 9. 예약 대기 취소를 한다. | 10. 예약 대기 취소 완료 |
| 11. 자전거 반납을 한다. | 12. 자전거 반납 완료 |
| 13. 근처 식당 추천을 원한다. | 14. 사용자 위치기반으로 근처 식당을 추천 |
| 15. 추천 식당 선택 | 16. 예약할수 있는 외부서비스 연결 |

| Actor Action | System Response |
| --- | --- |
| 1. 회원이 현재 대여 중인 자전거를 조회한다. | 2. 해당 리스트 ( 대여소 이름, 대여소 위치, 자전거ID, 자전거 제품명,  자전거 유형) 을 보여준다. |
| 3. 회원은 특정 자전거를 지정된 대여소에 반납한다. | 4. 반납을 한 후 사용자 위치 기반으로 근처 식당 추천 |
| 5. 추천 받은 식당 예약 | 6. 외부 서비스와 연결 |
