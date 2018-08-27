# lua-nuttx

## Abstract

This is Lua 5.3.5 ported to NuttX.

The following platforms are currently supported.
* Sony Spresense (CXD56)
* STM32F4Discovery

## NuttX Configuration

Required configs:
* `CONFIG_SYSTEM_READLINE=y`
* `CONFIG_READLINE_ECHO=y`
* `CONFIG_LIBC_WCHAR=y`
* `CONFIG_LIBC_LOCALE=y`
* `CONFIG_TIME_EXTENDED=y`
* `CONFIG_LIBM=y`

Optional features:
* `os.tmpname` and `io.tmpfile` requires `/tmp` mountpoint
