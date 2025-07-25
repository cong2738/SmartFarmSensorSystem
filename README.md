# FlagGame

> **2025년 HARMAN Semicon Academy 1기** <br/> **개발기간: 2025.06.03 ~ 06.12**

## 개발팀 소개

|박호윤                                          |지설윤                                            |                           
| :--------------------------------------------: | :--------------------------------------------:     |
|   [@cong2738](https://github.com/cong2738)     |   [JIseolyun](https://github.com/JIseolyun)      |

## Introduce

<img width="auto" height="500" alt="image" src="https://github.com/user-attachments/assets/58c4a25d-e220-48d6-9a3e-927ff25495d1" />

-  SmartFarm(RISC-V With AMBA Advanced Peripheral Bus)
   - APB INTERFACE를 직접 RTL Design하며 버스 인터페이스 이해를 높힌다
   - 직접 구현한 My RISC-5 AMBA Interface를 통해 높은 확장성 기대
   - 온도센서를 통해 스마트팜 공조장치 제어
   - 거리센서를 이용, 물탱크 수위 조절
   - FND와 UART를 통해 사용자에게 스마트팜 상태 알림

## Stacks

 - 핵심기술: APB Interface, RISC-5, RTL
 
### Environment

![Vivado](https://img.shields.io/badge/Tool-Vivado-904cab?style=for-the-badge&logo=&logoColor=white)
![Verdi](https://img.shields.io/badge/Tool-Verdi-00c853?style=for-the-badge)
![VCS](https://img.shields.io/badge/Tool-VCS-00695c?style=for-the-badge)

### Development & Simulation
![Verilog](https://img.shields.io/badge/HDL-Verilog-ff5722?style=for-the-badge)
![SystemVerilog](https://img.shields.io/badge/HDL-SystemVerilog-ff9800?style=for-the-badge)

### Board
![Basys3](https://img.shields.io/badge/Board-Basys3-2196f3?style=for-the-badge)</br>

## Object Diagram

<img width="500" height="auto" alt="image" src="https://github.com/user-attachments/assets/13095d2c-959b-49a8-a8f9-895cfe7360eb" /></br>  

_ _ _ _ _ _

### APB Interface

<img width="500" height="auto" alt="image" src="APB _INTERFACE.png" /></br>  

### APB Protocol
- CPU는 모든 PP를 메모리로서 인식하며 패리패럴의 선택은 매모리맵을 이용 주소로 구분, 모든 신호의 구조(프로토콜)은 동일

- 프로토콜 시퀀스(MASTER기준)
    - CPU의 PWRITE에 따라 PP모드 설정
    - CPU의 PADDR신호로 특정 PP 선택
    - CPU의 PSEL신호로 PP 준비
    - CPU의 PEN신호로 PP동작
    - PP의 READY신호를 통해 CPU에 완료확인 신호 송신

- 결과적으로 CPU를 활용하면 복잡한 회로를 사용하여 리소스를 많이 쓰지만 제어 부분과 주변장치 부분을  분리, 설계와 확장에 용이함


<img width="500" height="auto" alt="image" src="https://github.com/user-attachments/assets/ccd7e78e-2760-4bf3-86ba-329bc7b8bc1f" /></br>  

<img width="500" height="auto" alt="image" src="https://github.com/user-attachments/assets/c80013ca-ebad-4594-8bb0-34ab33777bad" /></br>  

<img width="500" height="auto" alt="image" src="https://github.com/user-attachments/assets/3180242c-d0ed-4234-b367-6528570d9b1d" /></br>  

_ _ _ _ _ _

## asset

<table>
   <tr>
      <td>Basys3</td>
      <td>HC-HR04</td>
      <td>DHT11</td>
   </tr>
   <tr>
      <td><img src="https://github.com/user-attachments/assets/aca0338d-1c94-465d-a12a-9e5662fabbaf" width="auto" height="150"/></td>
      <td><img src="https://github.com/user-attachments/assets/3205b368-2ceb-4e1a-b2f8-e8da18699177" width="auto" height="150"/></td>
      <td><img src="https://github.com/user-attachments/assets/a33fdd1a-3935-4a75-b439-8bd5020b9573" width="auto" height="150"/></td>
   </tr>
</table>

## video  
click!--></br>
<img width="500" height="auto" alt="image" src="image34.gif" /></br>  
<img width="500" height="auto" alt="image" src="image35.gif" /></br>  
<img width="500" height="auto" alt="image" src="image36.gif" /></br>  
