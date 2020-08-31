인프라란 무엇인가
----------------
Infra 기반 시설
Architecture 구조
Data Center 인프라 내 서버들의 집합
TOR 서버 렉 최상단에 모든 케이블이 집합된 구역


서버 타입
|-렉마운트 서버: 각 서버를 쌓아서 구성하는 서버 
--블레이드 서버: 모듈의 집합으로 구성된 서버 (스위치 등등)

모든 서버는 기본적으로 일반적인 컴퓨터의 구조를 가진다.


컴퓨터란 무엇인가
----------------
컴퓨터의 모든 연산은 기계어(어셈블리어)로 처리된다.
컴퓨터는 초기 연산을 위한 목적에서 시작하여, 점차 경량화되었고 다양한 분야로 분화되었다.
컴퓨터와 네트워크의 발전으로, 소비자의 행동패턴 및 특성을 파악하기 용이해졌다.

CPU 헤르츠의 종류
base: 
allcoreturbo: 
singlecoreturbo: 

Context Switching
Context Switching을 줄이기 위해서 cpu affinity를 사용가능 (Affinity pinning)

32bit VS 64bit
어플리케이션이 점차 무거워지면서, 더 많은 메모리를 필요로 하게 되었고, 고용량의 메모리를 처리하기 위한 64bit cpu의 필요성이 대두됨.

멀티 코어 / 멀티 쓰레드
멀티 코어: 하나의 cpu에 연산 처리를 위한 다수의 코어를 구성
멀티 쓰레드: 인텔이 개발한 신기술. 하나의 코어에 2개의 쓰레드를 가상으로!! 구성.

GPU
출력을 위한 연산장치이며, 동시 작업이 가능한 패러럴한 처리방식을 사용.
보통 용도와는 다르게 요즘 머신러닝이나 인공지능 처리 등 대규모 연산에도 적극 사용
성능의 발전 방식은 CPU와 동일.

기억장치
CPU - RAM - HDD
연간을 위한 데이터나 중간 데이터 및 결과 데이터를 저장하는데 사용

LAMP(Linux-Appache-Mysql-PHP)
 


Registers                  |
L1 Cache                   |
L2~L3 Cache                |
System Ram                 |
Permanent Storage          |
Network Storage           \/

(내려갈 수록 크고 싸고 느리다)

LPar(Logical Partition)
QOS(Quality Of Service): 

On Premise
전통적 방식의 인프라(??)
네트워크 컴퓨팅 환경을 구축하기 위해 장비를 직접 구입하고 관리
상황에 따른 규모 관리의 어려움과 비용 낭비 (OPEX OPeration Expense)
비즈니스 신속성 부합하지 못함
항상 최대 사용량을 예측하고 구매해야 함 (CAPEX CaPital Expense)

인프라 서비스의 등장
장비의 구매,관리,구축을 대행해주는 서비스 출현 (코로케이션, 서버 호스팅)
회사의 느린 네트워크를 대체하고, 전문적인 인력 상주로 관리의 전문성 높임
정전이나 각종 장애로부터 빠른 대처를 기대할 수 있다. (SLA Service Level Assurance 다운타임에 대한 보증)

On Demand





가상화-가상머신-컨테이너-하이퍼바이저
-------------------------------------




서버와 클라이언트
----------------


인프라에서 중요한 꼭지들
-----------------------



3 Tiers
-------
SPOF (Single Spot Of Failure)

HA (High Availability)
가용한 시간의 비율을 99% 99.9% 등과 같은 퍼센티지로 표현
잘 설계됨과 동시에 잘 테스트도 되어야함

DR (Disaster recovery)
|
|- RTO(복구목표시간 Recovery TIme Objectives)
|- RPO(복구목표시점 Recovery Point Objectives)

장애극복을 위해 HA 및 DR은 함께 쓰이고 있다.





