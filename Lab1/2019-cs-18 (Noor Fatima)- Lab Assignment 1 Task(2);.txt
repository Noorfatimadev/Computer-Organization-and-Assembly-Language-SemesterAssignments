
;********Lab task 2********


INCLUDE Irvine32.inc

.386
.model flat,stdcall
.stack 4096
ExitProcess proto,dwExitCode:dword

 .data
 
 .code
 main PROC
  mov eax, 4
  mov ebx, 5
  mul ebx           ;(4*5)
 mov ecx,eax        ;ecx=4*5
  mov eax, 7         ;eax=7
mov edx , 21        ;edx=21
mul edx              ;eax=7*21
  mov  edx, 3        ; edx=3
 
  add eax,edx           ; eax=3+(7*21)

  sub eax , ecx     ;eax = eax-ecx

 
 
  call writeint
  call readint
  exit

 main ENDP
 END main

 