# Uninitialized Signal in VHDL

This repository demonstrates a common error in VHDL code: uninitialized signals within processes.  The `bug.vhdl` file contains the erroneous code, resulting in unpredictable initial values. The `bugSolution.vhdl` file shows the corrected version.

**Problem:**
The `data_reg` signal is not initialized with a default value. In simulation, this might result in a random or 'X' value during the first clock cycle, causing incorrect data_out.

**Solution:**
Explicitly initialize `data_reg` to a known value (e.g., "00" or others) to ensure predictable behavior.
