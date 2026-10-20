# Examen virtual: pilas, colas y listas

SD1004 Estructura de Datos, Institución Universitaria Pascual Bravo. Docente: Juan Duque.

## Equipo

**Número de equipo:** 3

| Integrante | Nombre |
|:---:|---|
| A | Anderson Gil Arenas |

Equipo de un solo integrante: Anderson Gil Arenas realizó todas las partes.

## Partes grupales

| Parte | Archivo | Contenido |
|---|---|---|
| 1 | [01-movimientos.pdf](01-movimientos.pdf) | Secuencia R, M, N; estados de P y Q en cada paso; pseudocódigo; justificación; revisión de la propuesta M, N, R |
| 2 | [02-reparar-listas.pdf](02-reparar-listas.pdf) | Diagnóstico, recorrido y reparación de las listas 2.1 a 2.4 |
| 3 | [03-eleccion-estructuras.pdf](03-eleccion-estructuras.pdf) | Cola para solicitudes, pila para deshacer, lista circular simple y luego doble circular para técnicos |

Las versiones HTML de los mismos diagramas están en la carpeta [`html/`](html/).

## Respuesta individual (Parte 4)

| Integrante | Variante | Archivo |
|:---:|---|---|
| A | Retirar el nodo B; solo se ejecutó `A.siguiente = C` | [individuales/GilArenasAnderson-1.pdf](individuales/GilArenasAnderson-1.pdf) |

## Roles por parte

| Parte | Propuso | Dibujó | Verificó |
|:---:|---|---|---|
| 1 | Anderson Gil Arenas | Anderson Gil Arenas | Anderson Gil Arenas |
| 2 | Anderson Gil Arenas | Anderson Gil Arenas | Anderson Gil Arenas |
| 3 | Anderson Gil Arenas | Anderson Gil Arenas | Anderson Gil Arenas |

## Resumen de resultados

- **Parte 1:** secuencia R, M, N (3 movimientos). La propuesta M, N, R no logra el objetivo: al ejecutar N se retira el 6 y termina con P = 6, 4 y Q = 9, 2.
- **Parte 2:**
  - 2.1: `C.siguiente = B` se repara con `C.siguiente = nulo`.
  - 2.2: `B.siguiente = nulo` se repara con `B.siguiente = C`.
  - 2.3: `B.anterior = C` se repara con `B.anterior = A`.
  - 2.4: `A.anterior = B` se repara con `A.anterior = C`.
- **Parte 3:** cola (FIFO) para solicitudes; pila (LIFO) para deshacer; técnicos en lista circular simple que pasa a doble circular agregando la referencia `anterior`.
- **Parte 4 (integrante A):** falta `C.anterior = A`. Recorrido por anterior desde C: C, B, A.

## Herramientas consultadas

- Apuntes del curso SD1004 Estructura de Datos.
- IA: Claude (Anthropic).
  - **Consulta:** resolución de las cuatro partes del examen a partir del enunciado y elaboración de los diagramas en HTML y PDF.
  - **Verificación:** simulación paso a paso de cada movimiento de pila y cola, comparando el estado final con el objetivo posición por posición; recorrido manual de cada lista en su estado defectuoso y reparado, contando las visitas hasta llegar a nulo o a la quinta visita; revisión de cada referencia contra la tabla de enlaces esperados y de la simetría `x.siguiente.anterior = x` en las listas dobles.

## Registro en el repositorio

| Momento | Commit |
|---|---|
| Minuto 25 | Avance 1: movimientos de pila y cola (`01-movimientos.pdf`) |
| Minuto 50 | Avance 2: diagnóstico y reparación de listas (`02-reparar-listas.pdf`) |
| Antes del minuto 90 | Entrega final: elección de estructuras, respuesta individual y README |
