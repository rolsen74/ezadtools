# GCC Cross Compiler for AmigaOS 4 (with SDK)

This repository provides a simple Makefile to **build a GCC cross-compiler for AmigaOS 4**, including SDK headers.

If you just want to compile the cross-compiler with the AmigaOS 4 SDK — this Makefile will do exactly that.

If you’re looking to **fix bugs**, **build a native version**, or work on **runtime libraries**, please refer to:
- [adtools](https://github.com/AmigaLabs/adtools)
- [clib2](https://github.com/sodero/clib2)
- [clib4](https://github.com/AmigaLabs/clib4)

---

## 🔧 What This Builds

This setup compiles **GCC 11.5.0** along with its required dependencies:

| Package | Version |
|----------|----------|
| GMP | 5.1.3 |
| MPFR | 3.1.6 |
| MPC | 1.0.3 |
| Binutils | 2.23.2 |
| GCC | 11.5.0 |

It also:
- Applies **patches from [adtools](https://github.com/AmigaLabs/adtools)**  
- Builds and installs **include files** from:
  - **clib2**
  - **clib4**
  - **AmigaOS 4 SDK v54.16**

---

## 🧰 Usage

Just run:

```bash
make -f makefile_cross
