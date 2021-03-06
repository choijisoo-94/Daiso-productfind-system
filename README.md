# 다이소 물건찾기 시스템

-----------

> 안녕하세요!

>> **찬스** 팀

>>> **장종욱 / 최지수** 입니다.

-----------------

## 프로젝트 계획 이유

----------------

경제의 어려움을 겪고 있는 21세기에서 생활용품을 싸게 파는 곳이 있다면 단연코 다이소라고 말할 수 있을 것입니다. 하지만 저렴하다는 이유로, 커다란 매장에 별 생각 없이 방문해 원하는 것을 찾는 과정에서 그다지 필요없는 물건들도 충동구매하는 경우가 많으셨을 겁니다. 이러한 경험을 바탕으로 저희 팀은 고객의 입장에서 원활하고 편리한 시스템을 이용했으면 좋겠다는 생각을 갖고 프로젝트를 시작하게 되었습니다. 고객의 입장에서 계획을 시작했던 프로그램이었지만, 다이소의 직원분들에게도 필요하다는 생각이 들어 상품의 관리용 시스템을 추가하게 되었습니다. 처음엔 작은 프로젝트였지만 여러 가능성을 구상하며 다양한 기능들을 추가하게 되었고, 다이소 채팅봇 서비스를 구현하는 거대한 프로젝트로 거듭났습니다.

- 이 프로그램은 여러가지 기능들을 담고 있습니다. **다이소 물건찾기 시스템** 은 고객분들과 직원분들이 간편하고 손쉽게 물건을 찾을 수 있는 다양한 기능들이 구현되어 있습니다.
- 다이소에 가기 전 **고객** 분들은, 필요한 물건들이 자신이 가고자 하는 매장에 있는지 검색하고 재고확인을 한 후 재고의 걱정 없이 물건을 pick up 할 수 있습니다.
- 다이소에 일하고 계시는 **직원** 분들은, 고객들의 끝없는 "ㅇㅇ물건 어디 있죠?" 라는 질문 루틴에서 벗어나 업무의 효율성을 조금 더 높일 수 있습니다.

--------------------

## 다이소 물건찾기 시스템 기능 설명

------------------

### [채팅봇 MODE 선택 기능]

------------------

1. **회원가입 기능** >> 다이소 물건찾기 시스템을 가입하는 기능(ID / PW 값 입력)

2. **로그인 기능** >> 다이소 물건찾기 시스템 로그인(본인의 ID / PW 값 확인 후 입력)

3. **Customer/고객 기능** >> 고객이 사용 가능한 기능(물건 이름 검색, 재고 보유 지점 확인 등)

4. **Administrator/관리자 기능** >> 관리자가 사용 가능한 기능(상품 추가, 상품 위치, 재고 업데이트, 상품 삭제 등)

5. **로그아웃 기능** >> 다이소 물건찾기 시스템 종료

-------------------

### [MemberJoin / 회원가입 기능]

--------------------

#### 1. 다이소 물건찾기 시스템을 이용하고 싶은 고객들의 정보를 저장해 회원가입 가능
    - 회원 가입을 희망하는 고객들의 정보(고객 ID / 고객 PW) 를 받아 MEMBERSHIP을 이용할 수 있는 혜택을 제공해주는 기능

----------------------

### [LogIn / 로그인 기능]

-----------------------

#### 1. 회원가입한 정보를 토대로 멤버 로그인 가능
    - 회원가입한 멤버 DB(DATABASE)를 토대로 로그인 시스템을 활성화시켜 MEMBERSHIP 시스템을 이용하게 해주는 기능

------------------------

### [Customer mode / 고객 기능]

-----------------------

#### 1. 매장 내 모든 상품정보 검색 기능
    - 고객이 찾는 매장의 모든 상품들을 출력해주는 기능
#### 2. 매장 내 고객이 찾는 특정 상품정보 검색 기능
    - 고객이 찾는 특정 상품들로만 검색해서 위치 등 상품의 상세정보를 출력해주는 기능
#### 3. 상품을 검색했을 때 구매가능한 매장을 추천해주는 기능
    - 고객이 특정 상품을 검색했을 때 구매 가능한 매장의 상세 정보(가맹점 이름 / 가맹점 전화번호 / 재고 위치 / 가격) 을 알려주는 기능

------------------------

### [Administrator mode / 관리자 기능]

------------------------

#### 1. 모든 상품정보 검색
    - 현재 어떠한 상품들이 매장내에 있는지 모두 출력시켜주는 기능
#### 2. 특정 상품정보 검색
    - 특정 상품의 디테일한 정보(이름 / 재고현황 / 매장내 위치 / 가격)를 출력시켜주는 기능
    - 존재하지 않는 상품을 검색했을 때 에러 메세지 기능
#### 3. 새로운 상품들을 등록
    - 새로운 상품을 물품정보에 추가할 수 있는 기능
    - 존재하는 상품을 새로운 상품으로 등록했을 때 에러 메세지 기능
#### 4. 재고 수정 기능
    - 매장 내 유동적으로 변화하는 재고값을 수정하는 기능
    - 재고가 없는 상품에 대한 에러 메세지 기능
#### 5. 위치 수정 기능
    - 매장 내 고객들이 편리하게 이용 가능하도록 물건의 위치를 수정하는 기능
     - 매장 내 위치 정보가 정확하지 않은 제품에 대해 에러 메세지 기능
#### 6. 상품의 삭제 기능
    - 매장 내 더이상 판매하지 않는 제품 삭제하는 기능
    - 삭제해야 하는 항목이 존재하지 않을 때 에러 메세지 기능

-------------------

### [로그아웃 기능]

------------------
#### 1. 다이소 물건찾기 시스템 종료 시스템
    - 다이소에 로그인 했던 고객들의 정보를 로그아웃 시키는 기능
