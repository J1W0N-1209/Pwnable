# 함수 호출 규약 개요
함수 호츌 규약이란 함수를 호출하는 방식에 대한 약속이다.

# Cdecl
인자 전달 순서      가장 오른쪽 인자부터 전달
인자 전달 매체      Stack을 사용한다
Stack Frame 정리 방법       함수를 호출한 Caller가 인장 정리
C언어,C++ 표준 함수 호출 규약,가변인자 사용 O

# Stdcall
인자 전달 순서      가장 오른쪽 인자붙터 전달한다 
인자 전달 매체      Stack을 사용한다
Stack Frame 정리 방법       호출을 당한 Callee가 함수를 종료하면서 인자를 정리한다.
Window API,Visual Basic에서 사용하는 표준 규약,가변인자 사용 X

# Fastcall
인자 전달 순서      가장 오른쪽 인자부터 전달
인자 전달 매체      ECX,EDX,Stack 순서
Stack Frame 정리 방법       호출을 당한 Callee가 함수를 종료하면서 인자를 정리한다.
인자가 3개 이상이면 Stack을 사용해 인자 전달

