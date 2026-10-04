# crackmes

A specialized reverse-engineering laboratory divided into levels.

Five small Windows GUI programs that teach you how to analyze
real binaries. Each level opens a window with a lock icon, an
input field, and a status bar. Your job: make it show the
**green** `UNLOCKED` state.

> No source code is provided. Reverse it yourself.

---

## Structure

    crackmes/
    |-- level-1/
    |-- level-2/
    |-- level-3/
    |-- level-4/
    |-- level-5/
    |-- info.txt
    `-- crackmes.zip

Each `level-N/` folder contains **only** `crackme.exe`. The lock
image is embedded inside the binary. Just download, unzip, run.

---

## Levels

| Level | Difficulty | Status bar |
|-------|------------|------------|
| 1     | beginner   | red → green |
| 2     | easy       | red → green |
| 3     | medium     | red / yellow / green |
| 4     | hard       | red → green |
| 5     | expert     | red / yellow / green |

---

## Status bar colors

| Color  | Meaning                        |
|--------|--------------------------------|
| 🔴 red    | LOCKED (default)               |
| 🟡 yellow | leak / info (some levels)      |
| 🟢 green  | UNLOCKED (your goal)           |

---

## How to download

1. Download `crackmes.zip` (click **Code → Download ZIP**).
2. Unpack it. You will get five folders: `level-1` … `level-5`.
3. Open any `level-N/crackme.exe`.
4. Figure out how to reach the green state.

---

## Tools

- **Debugger:**      x64dbg, WinDbg, gdb, lldb
- **Disassembler:**  Ghidra, IDA Free, radare2, Cutter, objdump
- **Analysis:**      PE-bear, Detect It Easy, strings, nm
- **Exploitation:**  python3, pwntools
- **Hex editors:**   HxD, 010 Editor

---

## Rules of engagement

⚠ Run **only** in an isolated environment (VM, sandbox, your own machine)  
⚠ Do **not** use these binaries on real systems  
⚠ Do **not** attack systems you do not own  
⚠ All vulnerabilities are **intentional** and for learning only  
⚠ The author is **not responsible** for misuse of these materials

---

## Ethics

These materials are distributed for educational purposes only.  
By using them you agree to apply your knowledge legally:  
CTF competitions, your own labs, authorized security research.

> *A hacker is a researcher, not a criminal.*

---

## License

MIT — see [LICENSE](LICENSE).

---

Made for learning. Hack ethically. **Good luck!**
