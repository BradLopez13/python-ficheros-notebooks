# python-ficheros-notebooks

Cuadernos Jupyter de clase del ciclo de DAM (2023) sobre ficheros, SQLite y validación de datos en Python.

## Qué hay

| Cuaderno | Contenido |
| --- | --- |
| `Ficheros 1/Ficheros.ipynb` | Lectura y escritura de ficheros de texto: modos `w`, `r` y `a`, `readlines`, `with` y acceso aleatorio con `seek`. |
| `Bases de Datos.ipynb` | SQLite con el módulo `sqlite3`: crear una tabla, insertar con `execute` y `executemany`, y consultar. |
| `Validaciones Brad Lopez.ipynb` | Validación de dígitos de control de NIF/NIE, número de afiliación a la Seguridad Social (NAF) y cuenta bancaria. |

El de validaciones es el más interesante: cada documento tiene su propio algoritmo de control (módulo 23 con tabla de letras para el NIF, módulo 97 para el NAF y pesos por posición módulo 11 para la cuenta).

## Cómo ejecutarlo

```bash
pip install notebook
jupyter notebook
```

No hay dependencias externas: `sqlite3` viene con Python.

## Limitaciones conocidas

- Son cuadernos de clase: las celdas se ejecutan en orden y no hay tests.
