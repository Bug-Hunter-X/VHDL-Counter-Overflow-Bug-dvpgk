# VHDL Counter Overflow Bug

This repository demonstrates a common error in VHDL:  an unsigned counter that doesn't handle overflow. The `counter_bug.vhdl` file contains the buggy code.  The `counter_solution.vhdl` file provides a corrected version.

The bug is that when the counter reaches its maximum value ("1111"), the next increment results in an overflow, wrapping around to "0000".  This is often unintended and can lead to subtle errors in the system.

The solution introduces a check to prevent the overflow condition.