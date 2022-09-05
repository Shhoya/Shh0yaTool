# Shh0yaKit
- Analyze tool for windows reverser

### ※ Additional features may or may not be publicly available depending on circumstances and potential for exploitation
### Windows 10 1709(16299) ~ 
### To use or not to use is up to you.

## [0x00] Features
### Process Information(Shortcut : F2)
- Process Basic Information
- Process Module Information
    - Module dump
- Process Dump
- Process Memory Information
    - Alloc base dump
	- Memory dump
- Process Memory Scan(insecure)
- Process Virtual Address Descriptor Information(Not full information)
- Process Handle Information

### Live Memory Editor(Shortcut : F3), (like windbg)
※ There may be errors in command parsing. You should read the `help` command carefully
- Display Memory
    - d(db), dw, dd, dq, !d(!db), !dw, !dd, !dq
	- ex : d <Address, Symbol> /p <ProcessID> : Read process memory
- Enter Memory
    - e(eb), ew, ed, eq
	- ex : e <Address, Symbol> <Value>
- Save Memory(File)
    - ex : wm <Address, Symbol> <Size>
- Scan Kernel Module
    - ex : memscan <Pattern> (At least 8 patterns and '00' must be replaced with '??')
- Unassemble
    - ex : u <Address, Symbol>
	
### Kernel Pool Information(Shortcut : CTRL+P)
- NonPagedPool List

### Kernel Device List(Shortcut : CTRL+D)
- Device List

### Object Callback List(Shortcut : CTRL+O)
- ObCallbacks List

### Process&Thread Notify Routine List(Shortcut : CTRL+N)
- NotifyRoutine List

### Process Monitor(Shortcut : F4)
- like `ProcMon` by Sysinternals, 
- Additional : Intercept write file(%CurrentDir%\MonitorResult\)

### Binary Search(Shortcut : CTRL+B)
- Search PE in File
