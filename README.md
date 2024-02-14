# filesignature

Tool to obtain the file type by searching the `magic numbers`.


# Bytes Offsets

El "byte offset" (desplazamiento en bytes) se refiere a la posición de un byte específico dentro de un archivo o en una secuencia de bytes.

11 bytes offsets -> indica que se debe desplazar los primeros 11 bytes para obtener la marca bytes deseada.


# Cambiar de hex a str y viceversa

```python
>>> x = hex(ord('P'))
>>> x
'0x50'
>>> x.lstrip('0x')
'50'
>>> x[2:]
'50'
>>> bytes.fromhex(x[2:])
b'P'
>>> bytes.fromhex(x[2:]).decode('utf-8')
'P'

int('0x120', 16)
```
