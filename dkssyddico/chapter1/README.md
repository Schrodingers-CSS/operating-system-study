# Chapter 1

> 인프런 강의 및 교재 기반 정리

### 운영체제가 뭔가요?

- Operating system: a software that operates a **computer**
- ex: Window 10, Linux, Mac OS X

  - is a program running at all times on the computer
  - to provide system services to application programs
  - to manage **processes**, resourses, user interfaces, and so on

  <br>

### 컴퓨터는 뭔가요?

- Computer: a machine that processes the **information**
- calculator is not a machine, but smartphone is

- four components of computer system: hardware, operating system, application programs, user

  <br>

### 정보가 뭔가요? 컴퓨터가 정보를 어떻게 처리하죠?

- Information: a quantative representation that measures the uncertainty
- 정보의 최소 단위: bit(binary digit)
- 정보의 처리: 정보의 상태 변환 (0에서 1로, 1에서 0로)
- 부울 대수(Boolean Algebra): NOT, AND, OR
- 논리 게이트: NOT, AND, OR, XOR, NAND, NOR
- 논리회로: IC, LSI, VLSI, ULSI, SoC, ....
  - 무어의 법칙, 황의 법칙
- 정보의 저장과 전송: 플립-플롭, 데이터 버스

  <br>

- 덧셈은? 반가산기, 전가산기
- 뺄셈은? 2의 보수 표현법
- 곱셈과 나눗셈은? 뎃셈과 뺄셈의 반복
- 실수 연산은? 부동 소수점 표현법
- 함수? GOTO
- 삼각함수, 미분, 적분, 사진 촬영, 동영상 재생...

  <br>

### 컴퓨터가 만능이라는 건가요?

- 범용성: universality

  - NOT, AND, OR 게이트만으로 모든 계산을 할 수 있다
  - NAND 게이트만으로 모든 계산을 할 수 있다.
  - 범용 컴퓨터: general-purpose computer

- 계산가능성: computability

  - Turing-computable: 튜링 머신으로 계산가능한 것
  - 정지 문제: Halting Problem: 튜링 머신으로 풀 수 없는 문제

  <br>

### 프로그램이 뭔데요?

- Program is a set of **instrunctions**

  - that tells a computer's hardware to perform a task

  <br>

### 1.1 Whate Operating Systems Do

- An operating system is

  - a software that manages a computer's hardware
  - It also provides a basis for application programs and
    - acts as an intermediary between
    - the computer user and the computer hardware

- A computer system can be divided roughly into four components

  - the hardware
  - the operating system
  - the application programs
  - and a user

- Defining Operating Systems

  - There are No universally accepted definition of an operating system
  - A more common definition is that
    - "the one program running at all times on the computer"
    - usually called the **kernel**
  - Along with the kernel, there are two other types of programs:
    - **system programs**
    - **application programs**

  <br>

### 1.2 Computer-System Organization

- A modern computer system consist of:

  - one or more CPUs and
  - a number of device controllers connected through a common bus

- a **bootstrap** program is

  - the first program to run on computer power-on,
  - and then loads the operating system

- Interrupts

  - Hardware may trigger an **interrupt** at any time
    - by sending a signal to the CPU, usually by way of the system bus
    - 키보드 A가 눌렸으면 A라는 문자가 눌렸다는 것을 interrupts라는 방법으로 CPU에게 알려줌

- von Neumann architecture

  - A typical instruction-executiom cycle
    - first fetches an instruction from memory
    - and stores that instruction in the **instruction register**
  - the instruction is then decoded
    - and may cause operands to be fetched from memory
    - an stored in some internal register
  - After the instruction on the operands
    - has been **executed**,
    - the result may be stored back in memory

- The wide variety of storage systems can be organized in a hierarchy according to:

  - storage capacity,
  - and access time

- I/O Structure
  - A large portion of OS code is dedicated to managing I/O

### 1.3 Computer System Architecture

- Definitions of Computer System Components

  - **CPU** - The hardware that executes instructions.
  - **Processor** - A physical chip that contains one or more CPUs.
  - **Core** - The back computation unit of the CPU.
  - **Multicore** - Including multiple computing cores on the same CPU.
  - **Multiprocessor** - Including multiple processors.

  <br>

- **Symmetric multiprocessing (SMP)**

  - The most common multiprocessor systems,
    - in which each peer CPU processor performs all tasks.
  - **Asymmetric** multiprocessing:
    - each processor is assigned a specific task.

  <br>

- Multi-core design

  - with several cores on the same processor chip.

  <br>

### 1.4 Operating System Operations

- Multiprogramming

  - runs more than one program at a time.

  - keeps several processes in memory simultaneously.

  - to increase CPU utilization.

<br>

- Multitasking (=multiprocessing)

  - a logical extension of multiprogramming.

  - in which CPU switches jobs so frequently that
  - users can interact with each job while it is running.

  - **CPU scheduling**:

  - If several processes are ready to run at the same time,
  - the system must choose which process will run next

<br>

- Two separate mode of operations:
  - **user mode** and **kernel mode**
  - to ensure that an incorrect program
    - cannot cause other programs to execute incorrectly

<br>

### 1.7 Virtualization

- **Virtualization** is

  - a technology that allow us
    - to abstract the hardware of a single computer
    - into several different execution environments.

- **VMM**: Virtual Machine Manager
  - VMware, XEN, WSL, and so on.

<br>

### 1.10 Computing Environments

- Operating Systems in the Variety of Computing Environments

  - Traditional Computing
  - **Mobile** Computing
  - **Client-Server** Computing
  - **Peer-to-Peer** Computing
  - **Cloud** Computing
  - **Real-Time** Embedded Systems
