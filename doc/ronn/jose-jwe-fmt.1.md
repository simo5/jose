jose-jwe-fmt(1) -- Converts a JWE between serialization formats
===============================================================

## SYNOPSIS

`jose jwe fmt` -i JWE [-I CT] [-o JWE] [-O CT] [-c]

## OVERVIEW

The `jose jwe fmt` command converts a JWE into alternative serialization
formats. For example, it can:

1. Attach ciphertext to a detached JWE.
2. Detach ciphertext from a JWE.
3. Convert JWE Compact Serialization to JWE JSON Serialization.
4. Convert JWE JSON Serialization to JWE Compact Serialization.

## OPTIONS

*  `-i` _JSON_, `--input`=_JSON_ :
  Parse JWE from JSON

*  `-i` _FILE_, `--input`=_FILE_ :
  Read JWE from FILE

*  `-i` -, `--input`=-:
  Read JWE from standard input

*  `-I` _FILE_, `--detached`=_FILE_ :
  Read decoded ciphertext from FILE

*  `-I` -, `--detached`=- :
  Read decoded ciphertext from standard input

*  `-o` _FILE_, `--output`=_FILE_ :
  Write JWE to FILE

*  `-o` -, `--output`=- :
  Write JWE to stdout (default)

*  `-O` _FILE_, `--detach`=_FILE_ :
  Detach ciphertext and decode to FILE

*  `-O` -, `--detach`=- :
  Detach ciphertext and decode to standard output

*  `-c`, `--compact` :
  Output JWE using compact serialization

## AUTHOR

Nathaniel McCallum &lt;npmccallum@redhat.com&gt;

## SEE ALSO

`jose-jwe-dec`(1),
`jose-jwe-enc`(1)
