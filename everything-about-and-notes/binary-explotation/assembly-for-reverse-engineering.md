# Assembly for Reverse Engineering

These are some assembly instructions to do reverse engineering more easy:

* **MOV (Move)**: Copies the value from one location to another.

```armasm
mov eax, 42     ; Move the value 42 into the eax register
```

* **ADD**: Adds two values.

```armasm
add ebx, eax    ; Add the value in eax to the value in ebx
```

* **SUB**: Subtracts one value from another.

```armasm
sub ecx, edx    ; Subtract the value in edx from the value in ecx
```

* **CMP (Compare)**: Compares two values and sets flags based on the result.

```armasm
cmp esi, edi    ; Compare the values in esi and edi and set flags accordingly
```

* **JMP (Jump)**: Unconditionally transfers control to another instruction.

```armasm
jmp label       ; Unconditionally jump to the location labeled "label"
```

* **JE (Jump if Equal)**: Jumps to a specific location if the zero flag is set.

```
je equal_label  ; Jump to "equal_label" if the zero flag is set (previous comparison was equal)
```

* **JNE (Jump if Not Equal)**: Jumps to a specific location if the zero flag is not set.

```armasm
jne not_equal_label  ; Jump to "not_equal_label" if the zero flag is not set (previous comparison was not equal)jz label       ; Jump to "label" if the zero flag is set (eax == 0)
```

* **JZ**: It's a conditional jump instruction that transfers program control to a specified label or memory location if the zero flag (ZF) is set.

```
jz label       ; Jump to "label" if the zero flag is set (eax == 0)
```

* **CALL**: Calls a subroutine or function.

```armasm
call my_function  ; Call the subroutine or function labeled "my_function"
```

* **RET (Return)**: Returns from a subroutine.

```armasm
ret            ; Return from a subroutine
```

* **PUSH**: Pushes a value onto the stack.

```armasm
push eax       ; Push the value in eax onto the stack
```

* **POP**: Pops a value from the stack.

```
pop ebx        ; Pop a value from the stack into the ebx register
```

* **AND, OR, XOR**: Performs logical AND, OR, and XOR operations on values.

```armasm
and edx, ebx   ; Perform bitwise AND between edx and ebx
or ecx, eax    ; Perform bitwise OR between ecx and eax
xor esi, edi   ; Perform bitwise XOR between esi and edi
```

* **SHL/SHR (Shift Left/Right)**: Shifts bits left or right.

```
shl eax, 2     ; Shift the bits in eax left by 2 positions
shr ebx, 1     ; Shift the bits in ebx right by 1 position
```

* **INC/DEC (Increment/Decrement)**: Increases or decreases a value by one.

```armasm
inc ecx        ; Increment the value in ecx by one
dec edx        ; Decrement the value in edx by one
```

* **LOOP**: Decrements a counter and jumps if the counter is not zero.

```
mov ecx, 5     ; Set ecx to 5 (loop counter)
loop loop_label ; Decrement ecx and jump to "loop_label" while ecx is not zero
```

* **NOP (No Operation)**: Does nothing and acts as a placeholder.

```armasm
nop            ; No operation, does nothing
```

* **INT (Interrupt)**: Triggers an interrupt or software-generated exception.

```
int 0x80       ; Trigger a software interrupt (Linux system call)
```

* **LEA (Load Effective Address)**: Loads the address of a memory location.

```armasm
lea ebx, [ecx+edx]  ; Load the effective address of ecx+edx into ebx
```

* **CMPXCHG (Compare and Exchange)**: Compares and swaps a value if conditions are met (used in multi-threading).

```armasm
cmpxchg [eax], ebx  ; Compare the value in eax with the value at the memory address pointed by eax and exchange with ebx if equal (used in multi-threading)
```

* **XOR**: Performs bitwise XOR on two values.

```armasm
xor eax, eax   ; Clear the eax register by XORing it with itself
```
