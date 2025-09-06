# Arithmetic-operation-using-8086
# 8086 Assembly Language Programs for Arithmetic Operations

## AIM

To write and execute Assembly Language Programs to perform arithmetic operations for the 8086 microprocessor.

---

## APPARATUS REQUIRED

* Personal Computer with MASM Software

---

## 1. ADDITION

#### Algorithm

1. Initialize memory location in HL register.
2. Store 1st data.
3. Increment HL to enter 2nd data.
4. Move 2nd number to accumulator.
5. Decrement HL.
6. Add value in memory with accumulator.
7. Store result.
8. Stop.


## FLOW CHART
<img width="707" height="1024" alt="image" src="https://github.com/user-attachments/assets/b5a7062d-e294-47cd-9683-a40de25e82de" />


#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV CL,00H
MOV AX,[SI]
MOV BX,[SI+02H]
ADD AX,BX
JNC L1
INC CL
L1:
MOV [SI+04H],AX
MOV [SI+06H],CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations
<img width="1280" height="960" alt="image" src="https://github.com/user-attachments/assets/d59bcec9-2aec-4748-a755-4e27249d891c" />
## OUTPUT IMAGE FROM MASM SOFTWARE
<img width="640" height="480" alt="Screenshot (7)" src="https://github.com/user-attachments/assets/b60e6831-29b2-4650-b98e-a90ddcdfa8c5" />
<img width="640" height="480" alt="Screenshot (6)" src="https://github.com/user-attachments/assets/4ad00dbb-7a10-40a5-a5fc-eb88a8c6c949" />
## 2. SUBTRACTION

#### Algorithm

1. Initialize memory and store 1st data.
2. Increment to get 2nd data.
3. Move 2nd data to accumulator.
4. Subtract memory content.
5. Store result.

## FLOWCHART

<img width="578" height="797" alt="image" src="https://github.com/user-attachments/assets/564c3c7a-33ce-4a1c-8920-beb5c24b9b47" />


#### Program



#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations
<img width="1280" height="451" alt="image" src="https://github.com/user-attachments/assets/25215210-916c-45d7-b6be-329306e3d403" />
## OUTPUT SCREEN FROM MASM SOFTWARE
<img width="640" height="480" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/21d824d7-a398-4611-93be-450e6aaa8d25" />
<img width="640" height="480" alt="Screenshot (8)" src="https://github.com/user-attachments/assets/5aa7982c-5107-4cd8-bfd1-35e5aea0ac07" />
## 3. MULTIPLICATION

#### Algorithm

1. Initialize memory and store operands.
2. Move operands to registers.
3. Multiply.
4. Store result.

##FLOWCHART

<img width="569" height="906" alt="image" src="https://github.com/user-attachments/assets/88be88ff-2896-4a88-b73d-84ccffd2fcf9" />



#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
MUL BX
MOV [SI+04H],AX
MOV [SI+06H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations
<img width="1280" height="960" alt="image" src="https://github.com/user-attachments/assets/b8d6f313-4bc7-4487-a6bb-69fd63d0c5ef" />
## OUTPUT SCREEN FROM MASM SOFTWARE
<img width="640" height="480" alt="Screenshot (12)" src="https://github.com/user-attachments/assets/9ee271f5-1694-417d-a650-d7e45882dc04" />
<img width="640" height="480" alt="Screenshot (10)" src="https://github.com/user-attachments/assets/d2672b22-0155-49a7-85f1-aadc34caa49e" />
## 4. DIVISION

#### Algorithm

1. Load memory location of operands.
2. Perform division.
3. Store result.

   ## FLOWCHART
<img width="1065" height="802" alt="image" src="https://github.com/user-attachments/assets/25b4a483-0d42-494b-8639-1af3ea17191b" />


#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
DIV BX
MOV [SI+04H],AX
MOV [SI+06H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations
<img width="1280" height="960" alt="image" src="https://github.com/user-attachments/assets/4bb3d169-386e-48d0-8c99-12b0d86670e1" />
## OUTPUT FROM MASM SOFTWARE
<img width="640" height="480" alt="Screenshot (14)" src="https://github.com/user-attachments/assets/93d1e6af-93c1-483e-b2c8-5471f6c6c015" />
<img width="640" height="480" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/55398ee7-8a34-45ff-ad96-95cef50d1220" />
## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.
