# Ejercicios:

1. ¿Qué número binario representa el carácter 'C' en ASCII?
2. Convierte el número flotante 5.75 a binario (explica los pasos).

---

1. El carácter 'C' en ASCII se representa con el número binario 01000011. Este número corresponde al valor decimal 67.

---

2. Para convertir el número flotante 5.75 a binario se necesita separar la parte entera y la parte decimal y convertir cada una por separado.


### Paso 1:

Se convierte e 5 a binario.

| División | Cociente | Residuo |
|--------- |----------|---------|
| 5 ÷ 2    | 2        | 1       |
| 2 ÷ 2    | 1        | 0       |
| 1 ÷ 2    | 0        | 1       |

5 = 101

### Paso 2:

Se multplica por 2 y se toma la parte entera del resultado en cada paso:

1. 0.75 × 2 = 1.5 → parte entera: 1, parte decimal: 0.5  
2. 0.5 × 2 = 1.0 → parte entera: 1, parte decimal: 0.0  

0.75 = 0.11


### Paso 3:
Se combinan la parte entera y la decimal para hacer el resultado final:

- Parte entera: 101 
- Parte decimal: 0.11  

**Resultado final:**  101.11₂

El subindice 2 es para indicar que estamos trabajando con sistema binario.