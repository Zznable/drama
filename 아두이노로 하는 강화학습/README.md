# 아두이노로 하는 강화학습

복수의 드론을 통해서 사람처럼 움직이게 만드는 것이 목표임    
그중에서 `실제로 드론을 어떻게 띄우고 위치를 고정하고 움직이는지`가 가장 중요한 문제인 것 같음   

그러며 나는 `강화학습`을 통해서 이러한 문제를 해결해보고 싶음  
내가 할줄 아는 거는 신경망 구성해서 학습시키고 이런 것들을 할줄 암  
아는 걸로 문제를 해결하자는 생각임  

현재는 다음과 같은 문제점들을 해결 해야 하는 상황임

* 모터 구동
* 패키징
* 학습 환경 구성
* 모델 학습
* 검증


### 모터 구동
실제로 이러한 회로에 대한 이해가 부족한 상황임
드론도 원리만 따지고 보면 프로펠러가 있고 이거를 ESC를 이용해서 잘 날아가도록 제어를 하는 기계임
그러면 먼저 프로펠러를 연결해서 돌려야 다음에 제어가 가능함


### 패키징
현재 모터 구동은 해놓은 상태임  
현재 핀을 끼워서 각 부품을 연결해놓음  
실제 이러한 연결 상태로는 움직였다가는 회로가 빠져서 대참사가 일어날 것 같음  
1. 현재 띄워야 하는 부품은 어떤 부품이고  
2. 이에 대해서 프로펠러가 만들어내는 추력 및 전력 시스템이 충분한가?  
3. 이를 어떻게 보호 할 것인가?  
와 같은 것들을 고민해서 안정적인 비행이 가능하도록 만들 예정  

### 학습 환경 구성
위 문제를 해결하면 이제 띄울 수는 있는 상태임  
이제 소프트웨어적으로 어떻게 띄을 수 있는 지 생각해야 할 타임  
텐서플로우에서 이러한 임베디드 기기용 라이브러리를 제공하고 있음  
라이브러리를 이용해서 학습 환경을 구성할 예정임  
* 센서에서 들어오는 타입은 어떤식인가?
* 모델은 어떤식으로 구성해야 하나?
* reward 함수는 어떤식으로 구성?

이러한 문제점들을 고민해야함  

### 모델 학습
실제로 모델을 학습시키면서 문제가 없는지 확인이 필요함

### 검증
실제로 아두이노 단일로만 했을때 잘 나는지 확인이 필요 