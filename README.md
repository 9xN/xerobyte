# xerobyte

## What is it
xerobyte is an exploit that takes advantage of an unintended and undesirable side effect in dynamic random-access memory (DRAM) in which memory cells interact electrically between themselves by leaking their charges, possibly changing the contents of nearby memory rows that were not addressed in the original memory access (Turning 0's into 1's in computer code and vice versa) This circumvention of the isolation between DRAM memory cells results from the high cell density in modern DRAM, and can be triggered by specially crafted memory access patterns that rapidly activate the same memory rows numerous times. This is also known as the row hammer effect and has been used in some privilege escalation computer security exploits, but xerobyte is different, the purpose of xerobyte is to call, activate and run cached malware on the target system in a minimalistic manner.

