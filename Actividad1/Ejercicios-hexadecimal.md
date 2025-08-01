# Ejercicios:

1. Convierte el número decimal 255 a hexadecimal.
2. ¿Cuál es el valor hexadecimal de la secuencia binaria 11010110?

---

1. Para pasar un numero a hexadeciaml primero de divide el número entre 16 sucesivamente.

| División | Cociente | Residuo |
|----------|----------|---------|
| 255 ÷ 16 |    15    | 15      |
| 15 ÷ 16  |    0     | 15      |

Y luego se convierten los residuos a hexadecimal:

- 15 = F

### Resultado final: FF

---

2.  Primero se grupan los bits en bloques de 4:

1101 0110

Se convierte cada grupito

- 1101 = 13 → **D**
- 0110 = 6 → **6**


### Resultado final: 11010110₂ = D6₁₆



