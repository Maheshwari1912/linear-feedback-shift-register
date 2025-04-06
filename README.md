# linear-feedback-shift-register

**Introduction to LFSR (Linear Feedback Shift Register)**

A Linear Feedback Shift Register (LFSR) is a shift register whose input bit is a linear function (usually XOR or XNOR) of its previous state. It is widely used in applications like pseudo-random number generation, error detection/correction (CRC), scrambling, and encryption.

**Working of the LFSR Module**

The LFSR is initialized with a non-zero seed value (4'b0001 in this case).

On every positive clock edge, the register shifts its bits to the right.

The feedback bit is computed as lfsr[3] ^ lfsr[2], ensuring a pseudo-random sequence.

The new bit enters from the left, creating a new state.

If rst is high, the LFSR is reset to its initial state (4'b0001).

**Aim of LFSR**

**Pseudo-Random Number Generation** – LFSRs generate a sequence of bits that appear random.

**Data Scrambling** – Used in digital communication systems to randomize data patterns.

**Error Detection and Correction** – LFSRs help generate Cyclic Redundancy Check (CRC) codes.

**Efficient Hardware Implementation** – Requires fewer resources than traditional random number generators.

**Encryption & Cryptography** – Used in stream ciphers for secure data transmission.

This 4-bit LFSR will generate a pseudo-random sequence before repeating itself, depending on the initial seed and feedback function. 

**simulation results:**

![image](https://github.com/user-attachments/assets/ca7ccaa4-39fd-4013-a9ae-b8d7e4d77ecd)

**schematic:**

![image](https://github.com/user-attachments/assets/b7c9a056-418d-45b9-8015-3840b1716627)

