# 키친포스

## 요구 사항

### 상품

- 상품을 등록할 수 있다.
- 상품의 가격이 올바르지 않으면 등록할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 이름이 올바르지 않으면 등록할 수 없다.
    - 상품의 이름에는 비속어가 포함될 수 없다.
- 상품의 가격을 변경할 수 있다.
- 상품의 가격이 올바르지 않으면 변경할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 가격이 변경될 때 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 크면 메뉴가 숨겨진다.
- 상품의 목록을 조회할 수 있다.

### 메뉴 그룹

- 메뉴 그룹을 등록할 수 있다.
- 메뉴 그룹의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴 그룹의 이름은 비워 둘 수 없다.
- 메뉴 그룹의 목록을 조회할 수 있다.

### 메뉴

- 1 개 이상의 등록된 상품으로 메뉴를 등록할 수 있다.
- 상품이 없으면 등록할 수 없다.
- 메뉴에 속한 상품의 수량은 0 이상이어야 한다.
- 메뉴의 가격이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴는 특정 메뉴 그룹에 속해야 한다.
- 메뉴의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 이름에는 비속어가 포함될 수 없다.
- 메뉴의 가격을 변경할 수 있다.
- 메뉴의 가격이 올바르지 않으면 변경할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴를 노출할 수 있다.
- 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 높을 경우 메뉴를 노출할 수 없다.
- 메뉴를 숨길 수 있다.
- 메뉴의 목록을 조회할 수 있다.

### 주문 테이블

- 주문 테이블을 등록할 수 있다.
- 주문 테이블의 이름이 올바르지 않으면 등록할 수 없다.
    - 주문 테이블의 이름은 비워 둘 수 없다.
- 빈 테이블을 해지할 수 있다.
- 빈 테이블로 설정할 수 있다.
- 완료되지 않은 주문이 있는 주문 테이블은 빈 테이블로 설정할 수 없다.
- 방문한 손님 수를 변경할 수 있다.
- 방문한 손님 수가 올바르지 않으면 변경할 수 없다.
    - 방문한 손님 수는 0 이상이어야 한다.
- 빈 테이블은 방문한 손님 수를 변경할 수 없다.
- 주문 테이블의 목록을 조회할 수 있다.

### 주문

- 1개 이상의 등록된 메뉴로 배달 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 포장 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 매장 주문을 등록할 수 있다.
- 주문 유형이 올바르지 않으면 등록할 수 없다.
- 메뉴가 없으면 등록할 수 없다.
- 매장 주문은 주문 항목의 수량이 0 미만일 수 있다.
- 매장 주문을 제외한 주문의 경우 주문 항목의 수량은 0 이상이어야 한다.
- 배달 주소가 올바르지 않으면 배달 주문을 등록할 수 없다.
    - 배달 주소는 비워 둘 수 없다.
- 빈 테이블에는 매장 주문을 등록할 수 없다.
- 숨겨진 메뉴는 주문할 수 없다.
- 주문한 메뉴의 가격은 실제 메뉴 가격과 일치해야 한다.
- 주문을 접수한다.
- 접수 대기 중인 주문만 접수할 수 있다.
- 배달 주문을 접수되면 배달 대행사를 호출한다.
- 주문을 서빙한다.
- 접수된 주문만 서빙할 수 있다.
- 주문을 배달한다.
- 배달 주문만 배달할 수 있다.
- 서빙된 주문만 배달할 수 있다.
- 주문을 배달 완료한다.
- 배달 중인 주문만 배달 완료할 수 있다.
- 주문을 완료한다.
- 배달 주문의 경우 배달 완료된 주문만 완료할 수 있다.
- 포장 및 매장 주문의 경우 서빙된 주문만 완료할 수 있다.
- 주문 테이블의 모든 매장 주문이 완료되면 빈 테이블로 설정한다.
- 완료되지 않은 매장 주문이 있는 주문 테이블은 빈 테이블로 설정하지 않는다.
- 주문 목록을 조회할 수 있다.

## 용어 사전

### 상품
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 상품 | Product | 메뉴에 포함되어 손님에게 제공되는 최소 단위 |
| 식별자 | ID | 상품을 식별할 수 있는 32자리 고유 식별자 |
| 이름 | Name | 상품을 지칭하는 이름. 비속어를 포함할 수 없다. |
| 가격 | Price | 상품의 가격. 0원 이상이어야 한다. |
| 등록하다 | Create | 새로운 상품을 등록할 수 있다. |
| 가격 변경하다 | ChangePrice | 등록된 상품의 가격을 변경할 수 있다. 변경하려는 가격은 0원 이상이어야 한다. |
| 목록 조회하다 | FindAll | 등록된 상품의 목록을 조회할 수 있다. |

### 메뉴 그룹
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 메뉴 그룹 | MenuGroup | 특정 카테고리로 여러 메뉴를 묶어놓은 단위 |
| 식별자 | ID | 메뉴 그룹을 식별할 수 있는 32자리 고유 식별자 |
| 이름 | Name | 메뉴 그룹을 지칭하는 이름 |
| 등록하다 | Create | 새로운 메뉴 그룹을 등록할 수 있다. |
| 목록 조회하다 | FindAll | 등록된 메뉴 그룹 목록을 조회할 수 있다. |

### 메뉴
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 메뉴 | Menu | 하나 이상의 상품으로 구성되어 손님에게 판매되는 단위 |
| 식별자 | ID | 상품을 식별할 수 있는 32자리 고유 식별자 |
| 이름 | Name | 메뉴를 지칭하는 이름 |
| 가격 | Price | 메뉴의 가격. 0원 이상이어야 한다. |
| 메뉴 상품 | MenuProduct | 메뉴에 속한 상품. 수량은 0 이상이어야 한다. 메뉴 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다. |
| 메뉴 그룹 | MenuGroup | 메뉴가 속한 메뉴 그룹. 하나의 메뉴 그룹에 속해야 한다. |
| 등록하다 | Create | 새로운 메뉴를 등록할 수 있다. 1 개 이상의 등록된 상품으로 구성한다. |
| 가격 변경하다 | ChangePrice | 메뉴의 가격을 변경할 수 있다. 변경하려는 가격은 0원 이상이어야 한다. |
| 노출하다 | Display | 메뉴를 노출할 수 있다. 메뉴의 가격이 메뉴에 속한 상품 금액의 합과 같거나 낮아야한다. |
| 숨기다 | Hide | 메뉴를 숨길 수 있다. |
| 목록 조회하다 | FindAll | 등록된 메뉴 목록을 조회할 수 있다. |

### 주문 테이블
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 주문 테이블 | OrderTable | 손님에게 제공되는 테이블 |
| 식별자 | ID | 주문 테이블을 식별할 수 있는 32자리 고유 식별자 |
| 이름 | Name | 주문 테이블을 지칭하는 이름 |
| 손님 수 | NumberOfGuests | 방문한 손님 수. 0 이상이어야 한다. |
| 빈 테이블 여부 | Empty | 주문 테이블이 빈 테이블인지 여부 |
| 등록하다 | Create | 새로운 주문 테이블을 등록할 수 있다. |
| 빈 테이블 해지하다 | Sit | 손님이 방문하면 빈 테이블을 해지할 수 있다. |
| 빈 테이블 설정하다 | Clear | 손님이 떠나면 빈 테이블로 설정할 수 있다. |
| 손님 수 변경하다 | ChangeNumberOfGuests | 방문한 손님 수를 변경할 수 있다. 0 이상이어야 한다. |
| 목록 조회하다 | FindAll | 등록된 주문 테이블 목록을 조회할 수 있다. |

### 주문
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 주문 | Order | 구매를 요청하는 행위 |
| 식별자 | ID | 주문을 식별할 수 있는 32자리 고유 식별자 |
| 유형 | Type | 주문의 유형. 배달 주문, 포장 주문, 매장 주문이 있다. |
| 상태 | Status | 주문의 상태. 대기중, 수락됨, 서빙됨, 배달중, 배달됨, 완료됨이 있다. |
| 시각 | OrderDateTime | 주문이 요청된 시각 |
| 항목 | OrderLineItems | 주문에 요청할 수 있는 항목. 수량은 0 이상이어야 한다. |
| 배달 주소 | DeliverAddress | 배달 주문을 배달할 주소. 비워둘 수 없다. |
| 주문 테이블 | OrderTable | 매장 주문을 등록할 수 있는 주문 테이블. 매장 주문이 완료되면 빈 테이블로 설정할 수 있다. 매장 주문이 완료되지 않으면 빈 테이블로 설정할 수 없다. |
| 등록하다 | Create | 주문을 등록할 수 있다. 등록된 주문은 접수 대기할 수 있다. |
| 접수하다 | Accept | 접수 대기중인 주문을 접수할 수 있다. 배달 주문을 접수하면 배달 대행사를 호출할 수 있다. |
| 서빙하다 | Serve | 접수된 주문을 서빙할 수 있다. |
| 배달 시작하다 | StartDelivery | 서빙된 주문을 배달을 시작할 수 있다. |
| 배달 완료하다 | CompleteDelivery | 배달 중인 주문의 배달을 완료할 수 있다. |
| 완료하다 | Complete | 주문을 완료할 수 있다. |
| 목록 조회하다 | FindAll | 요청된 주문 목록을 조회할 수 있다. |

## 모델링
