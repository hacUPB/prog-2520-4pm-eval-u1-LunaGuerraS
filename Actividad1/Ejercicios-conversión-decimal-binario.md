# Ejercicios de conversión entre sistemas decimal y binario:

### Ejercicios:

1. Convierte el número decimal 22 a binario.

2. ¿Cuál es el resultado en decimal del número binario 10110?


---

1. Para convertir de decimal a binario de divide entre 2 y vamos anotando el residuo.

| División | Cociente | Residuo |
|---|---|---|
| 22 / 2 | 11 | 0 |
| 11/2 | 5 | 1 |
| 5/2 | 2 | 1 |
| 2/2 | 1 | 0 |
| 1/2 | 0 | 1 |

Para tener el binario se toma entonces los numeros de residuo en orden acendente (de abajo a arriba).

### Número en binario: 10110

---

2. Para convertir de binario a decimal se enumeran los números de derecha a isquierda: 

  |  |  |  |  |  |
|---|---|---|---|---|
| 1| 0 | 1 | 1 | 0 |
| **4** | **3** | **2** | **1** | **0** |

Luego se multiplica el cada número por 2 elevado al numero de la enumeración que hicimos:

0 * 2<sup>0</sup> + 1 * 2<sup>1</sup> + 1 * 2<sup>2</sup> + 0 * 2<sup>3</sup> + 1 * 2<sup>4</sup>

Total: 0 + 2 + 4 + 0 + 16 = 22

### Número decimal: 22
