# Linux kernel code reading using gdb and qemu

## Tips

### GDB

Setting PATH for Linux kernel source code like as:
`(gdb) directory $cwd:/work/build-linux`

Using TUI mode: `(gdb) la src`

Connecting to target: `(gdb) target remote :10000`

Command list for Linux: `(gdb) apropos lx`

### QEMU

Setting GDB option like as:
`-gdb tcp::10000 -S`

Disable KASLR(Kernel Address Space Layout Randomization) for using symbol:
`-append "nokaslr ..."`

## Reference

### The Linux Kernel: Debugging kernel and modules via gdb

https://www.kernel.org/doc/html/v4.18/dev-tools/gdb-kernel-debugging.html
