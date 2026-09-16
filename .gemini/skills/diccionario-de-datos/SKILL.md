---
name: Diccionario de datos
description: Describe cada columna de un CSV con su tipo, un ejemplo real y que significa en el dominio. Usela al recibir un dataset nuevo, antes de decidir que columnas sirven
version: 1.0.0
---

# Diccionario de datos

Recibe la ruta de un CSV y devuelve la descripcion de cada una de sus columnas: como se
llama, que tipo trae, un valor de ejemplo tomado del archivo y que significa en el dominio
del que salieron los datos.

Existe para no volver a explicar el dataset desde cero. Un diccionario escrito una vez
sirve para todo el semestre, y sirve tanto para una persona nueva en el equipo como para
una herramienta.

## Formato

### Ficha del archivo
Nombre, filas, columnas, de donde salio y cuando se descargo.

### Columnas
| Columna | Tipo | Ejemplo real | Que significa | Confianza |
|---------|------|--------------|---------------|-----------|

La columna Confianza dice "alta" si el significado esta documentado en la fuente, y
"deducida" si se infirio de los valores.

### Columnas que no se entienden
Las que no se pudieron describir, con lo que haria falta para describirlas.

## Reglas

- No limpie los datos, no haga gráficos y no decida qué columnas sirven.
- Use únicamente ejemplos reales tomados del CSV y verifique que cada columna del archivo aparezca en el resultado.
