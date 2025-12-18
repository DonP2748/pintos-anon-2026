# Pintos OS – Updated Guide for Modern Ubuntu

## Brief

This repository provides a **step-by-step guide for setting up and running the Pintos operating system on newer Ubuntu versions (e.g., Ubuntu 22.04)**.

The original Pintos project was designed for older Linux environments and requires several modifications to work correctly on modern systems. This guide documents those required changes and the correct build and run process.

This project is intended for:
- People who already know about Pintos
- Learners who are **not Stanford students**
- Self-learners who do not have access to teachers or lecturers
- Anyone who wants to study **operating system concepts** through Pintos

My **own Pintos implementation** (threads, user programs, virtual memory, file system, buffer cache, etc.) is maintained in a **separate OS repository** and is referenced only for learning purposes.

---

## Disclaimer

This repository is provided **for educational and reference purposes only**.

If you are currently enrolled in a course that uses Pintos, **do not copy this code directly**, as doing so may violate your institution’s academic integrity policy.

---

## Requirements

- Ubuntu 22.04 (recommended)
- `qemu`
- `gcc`
- `make`
- Standard Linux build tools

---

## How to Build Pintos

### 1. Install QEMU Emulator

```bash
sudo apt-get install qemu
````

---

### 2. Download Pintos Source Code

```text
https://github.com/WyldeCat/pintos-anon
```

> **Note:**
> Do **not** download older Pintos versions. They will not work correctly on modern Ubuntu without additional fixes.

---

### 3. Extract Pintos Source

Unzip the downloaded `pintos.tar.gz` file.

---

### 4. Edit `pintos-gdb`

Open the following file:

```text
/utils/pintos-gdb
```

Edit the `GDBMACROS` variable and assign it to your **absolute Pintos path**.

Example:

```bash
GDBMACROS=/home/username/pintos/src/misc/gdb-macros
```

---

### 5. Fix Makefile Variable Name

Open:

```text
/src/utils/Makefile
```

Rename:

```text
LOADLIBES → LDLIBS
```

This is required for compatibility with newer toolchains.

---

### 6. Compile Pintos Utilities

```bash
cd src/utils
make
```

> Note:
> I commented out all **System V–related implementations** to avoid build errors on modern systems.

---

### 7. Switch Emulator from Bochs to QEMU

Edit:

```text
/src/threads/Make.vars
```

Line 7:

```text
bochs → qemu
```

---

### 8. Compile Threads Project

```bash
cd src/threads
make
```

---

### 9. Update Pintos Script for QEMU

Edit:

```text
/utils/pintos
```

Make the following changes:

* Line 103: replace `bochs` with `qemu`
* Line 621: replace `qemu` with `qemu-system-x86_64`

---

### 10. Update PATH Environment Variable

Edit:

```bash
~/.bashrc
```

Add this line at the end (replace with your absolute path):

```bash
export PATH=/home/username/pintos/src/utils:$PATH
```

Apply changes:

```bash
source ~/.bashrc
```

---

## How to Run Pintos

For **each project**, you must build it once before running tests.

### Example: Project 1 (Threads)

1. Go to the project source directory:

   ```bash
   cd src/threads
   ```

2. Build the project:

   ```bash
   make
   ```

3. Enter the build directory:

   ```bash
   cd build
   ```

4. Run all tests:

   ```bash
   make check
   ```

---

### Running a Specific Test Case

You do **not** need to run all tests every time.

When running `make check`, Pintos prints the exact command for each test.
You can run a single test manually.

Example:

```bash
pintos -v -k -T 60 --qemu -- -q run alarm-single
```

I maintain a separate file listing **all test commands for each project**, so you can rerun only the failed tests instead of executing `make check` every time.

---

## License

Pintos is licensed under the original **Stanford Pintos license**.

All original copyright notices and license texts are preserved.



