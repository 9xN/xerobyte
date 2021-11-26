# xerobyte

## What is it & how does it work
xerobyte is an exploit that takes advantage of an unintended and undesirable side effect in dynamic random-access memory (DRAM) in which memory cells interact electrically between themselves by leaking their charges, possibly changing the contents of nearby memory rows that were not addressed in the original memory access (Turning 0's into 1's in computer code and vice versa) This circumvention of the isolation between DRAM memory cells results from the high cell density in modern DRAM, and can be triggered by specially crafted memory access patterns that rapidly activate the same memory rows numerous times.

This is also known as the row hammer effect and has been used in some privilege escalation computer security exploits, but xerobyte is different, the purpose of xerobyte is to call, activate and run cached malware on the target system in a minimalistic manner.

Read operations are of a destructive nature because the design of DRAM requires memory cells to be rewritten after their values have been read by transferring the cell charges into the row buffer. Write operations decode the addresses in a similar way, but as a result of the design entire rows must be rewritten for the value of a single bit to be changed.

## So what could you do with this?
xerobyte aims to allow users to cache a payload or a series of exploits via very little amounts of OSINT investigation or social engineering skills and poses risk to anyone with a communication platform that caches or stores any information on the users computer including but not limited to; visiting ANY WEBSITE with cookies or javascript enabled, Discord, Instagram, Facebook, signal, telegram, matrix apps, as well as many more client side applications that store ANY content from another user on the target machine. So what is the plan of attack after creating a payload and sending it to your victim? Calling the row hammer exploit to gain privledge escalation, then use xerobyte to call and run ANY form of data on the system, including but not limited to; plaintext, byte code, executables, and more. Payload options include and are also not limited to; anti-virus removal and detection software, credential and other information stealing scripts, remote acess tools/trojans, ransomware, as well as man in the middle internet and keylogging traffic interception attacks (man in the middle attacks).
## Usage
Researchers were able to gain unrestricted access to all physical memory by flipping bits in the page table entry, which maps the memory address locations. The same research also demonstrated how untrusted applications could gain root privileges. In another case, researchers used Rowhammer to obtain a 2048-bit encryption key out of memory. This could be detrimental towards privacy concerned individuals as law enforcement agencies as well as anyone once this knowledge becomes mainstream as encryption methods such as pgp become useless as even if you are storing your keys offline in theory once an offline storage device containing the keys is connected you can store code containing pertinent info and utilize a cached specialy crafted payload into sending over valuable information as well as hidding persistent and near IMPOSSIBLE to discover and remove malware.

## Old exploits
On March 9, 2015, Google's Project Zero revealed two working privilege escalation exploits based on the row hammer effect, establishing its exploitable nature on the x86-64 architecture. One of the revealed exploits targets the Google Native Client (NaCl) mechanism for running a limited subset of x86-64 machine instructions within a sandbox, exploiting the row hammer effect to escape from the sandbox and gain the ability to issue system calls directly. This NaCl vulnerability, tracked as CVE-2015-0565, has been mitigated by modifying the NaCl so it does not allow execution of the clflush (cache line flush) machine instruction, which was previously believed to be required for constructing an effective row hammer attack.

The second exploit revealed by Project Zero runs as an unprivileged Linux process on the x86-64 architecture, exploiting the row hammer effect to gain unrestricted access to all physical memory installed in a computer. By combining the disturbance errors with memory spraying, this exploit is capable of altering page table entries used by the virtual memory system for mapping virtual addresses to physical addresses, which results in the exploit gaining unrestricted memory access.

## Mitigation
As Razavi and Jattke of ETH Zurich, the team behind the research also includes Victor van der Veen of Qualcomm, Pietro Frigo of VU Amsterdam, and Stijn Gunter, the team that discovered the row hammer technique officially stated;

“Concluding, our work confirms that the DRAM vendors’ claims about Rowhammer protections are false and lure you into a false sense of security,” the researchers wrote. “All currently deployed mitigations are insufficient to fully protect against Rowhammer. Our novel patterns show that attackers can more easily exploit systems than previously assumed.”

As far as I or anyone for the matter can tell the only threat mitigation possible at this time appears to be including and building a threat model trying to prepare for such an attack. 


## Summary
xerobyte is a series of computer exploits that involves the use of highly advanced memory overloading techniques to trick your computer into running code and possibly malware that can overide even your own control as an administrative user as well as steal sensitive and private data such as your crypto wallet and real world banking information as well as email accounts and passwords for sites and other applications, all without the need for you to even touch your computer once.

## Final excerpt and legal information

