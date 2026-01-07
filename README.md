# No-ALU-Game

https://github.com/user-attachments/assets/8f438f69-9f90-47d4-813a-46acb256a8cd

I was curious: Is it possible to build a simple game using only a Counter and Memory? No ALU, no logic gates, and no arithmetic operations.
So, this project is the answer to that question.

It demonstrates a system where **computation is replaced by memory retrieval**. Instead of calculating pixel movement or game physics via equations, every possible Game State and Frame is pre-stored in RAM using **Look-Up Table (LUT)** logic.

The implementation relies on manually written **Hex Codes**, where the memory output bits are sliced to handle three parallel tasks:
1.  **Pixel Position:** Drawing both the player's location and the obstacles directly from memory bits.
2.  **Control Signals:** Managing game logic
3.  **Address Generation:** The core mechanism where the current **Counter** (Time) and **State Value** (Memory Output) combine to determine the next address, effectively replacing the Program Counter and Branching logic found in standard CPUs.




