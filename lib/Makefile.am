AM_CFLAGS = @JOSE_CFLAGS@ @jansson_CFLAGS@ @zlib_CFLAGS@ @libcrypto_CFLAGS@ -pthread -I $(top_srcdir)
LDFLAGS += @jansson_LIBS@ @zlib_LIBS@ @libcrypto_LIBS@ -export-symbols-regex '^jose_' -version-info 1:0:0

lib_LTLIBRARIES = libjose.la
libjose_la_SOURCES = \
    misc.c misc.h \
    cfg.c \
    io.c \
    b64.c \
    hsh.c hsh.h \
    hooks.c hooks.h \
    jwk.c \
    jws.c \
    jwe.c \
    zlib/deflate.c \
    openssl/aescbch.c \
    openssl/aesgcm.c \
    openssl/aesgcmkw.c \
    openssl/aeskw.c \
    openssl/compat.c openssl/compat.h \
    openssl/dir.c \
    openssl/ec.c \
    openssl/ecdh.c \
    openssl/ecdhes.c \
    openssl/ecdsa.c \
    openssl/hash.c \
    openssl/hmac.c \
    openssl/jwk.c \
    openssl/lock.c \
    openssl/misc.c openssl/misc.h \
    openssl/oct.c \
    openssl/pbes2.c \
    openssl/rsa.c \
    openssl/rsaes.c \
    openssl/rsassa.c
