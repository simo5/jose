AC_PREREQ(2.59)
AC_INIT(jose, 7)
AC_CANONICAL_SYSTEM
AC_PROG_CC_C99

AM_INIT_AUTOMAKE([subdir-objects foreign no-dist-gzip dist-bzip2 parallel-tests])
AM_SILENT_RULES([yes])
AM_PROG_CC_C_O

LT_INIT([disable-static])

PKG_PROG_PKG_CONFIG([0.25])

PKG_CHECK_MODULES([zlib], [zlib])
PKG_CHECK_MODULES([jansson], [jansson >= 2.10])
PKG_CHECK_MODULES([libcrypto], [libcrypto >= 1.0.2])

JOSE_CFLAGS="\
-Wall \
-Wextra \
-Werror \
-Wstrict-aliasing \
-Wchar-subscripts \
-Wformat-security \
-Wmissing-declarations \
-Wmissing-prototypes \
-Wnested-externs \
-Wpointer-arith \
-Wshadow \
-Wsign-compare \
-Wstrict-prototypes \
-Wtype-limits \
-Wunused-function \
-Wno-missing-field-initializers \
-Wno-unused-parameter \
"
AC_SUBST([JOSE_CFLAGS])

AC_CONFIG_FILES([jose/jose.h jose.pc jose/Makefile lib/Makefile cmd/Makefile tests/Makefile doc/Makefile Makefile])
AC_OUTPUT
