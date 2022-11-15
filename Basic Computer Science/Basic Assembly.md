# 어셈블리어란?
어셈블리어는 기계어와 일대일 대응이 되는 컴퓨터 프로그래밍의 저급 언어 입니다.

# Intel 문법과 AT&T 문법
어셈블리어에는 Intel문법과 AT&T 문법이 존재하며
또한 이들은 서로 호환되지 않습니다.

명령어 수행 방식 

ADD EAX EBX

Intel : EAX와 EBX 더한 결과값을 EAX 저장
AT&T : EAX와 EBX 더한 결과값을 EBX 저장

숫자 표기 방식

Intel : 1,2,3,4,5
AT&T : $1,$2,$3,$4,$5

레지스터 표기 방식

Intel : EAX,EBX,EBP
AT&T : %EAX,%EBX,%EBP

# 어셈블리에서 사용되는 레지스터 종류

범용 레지스터

EAX : 사칙연산 등 산술 연사에 자동으로 사용
EBX : 간접 번지 지정 사용
ECX : 반복 Count 역할
EDX : EAX 보조 ex) 나누기 몫 : EAX 나머지 : EDX 

인덱스 레지스터

ESI : 복사나 비교를 할 경우 출발지 주소 저장
EDI : 복사나 비교를 할 경우 목적지 주소 저장

포인터 레지스터

EIP : 다음 실행할 명령어 주소 저장
ESP : Stack Pointer의 가장 최근에 저장된 공간의 주소 저장
EBP : Stack Pointer의 기준점 저장

# 어셈블리어 자주 사용하는 명령어

명령어      예제        설명
push        push eax    eax의 값을 저장
pop         pop eax     스택 가장 상위값을 꺼내서 eax에 저장
mov         mov eax,ebx 메모리나 레지스터의 값을 옮길 때 사용
call        call proc   프로시저 호출
ret         ret         호출했던 바로 다음 지점으로 이동