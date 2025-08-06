# Ejercicios Finales:

1. Explica, en tus propias palabras, por qué es necesario que las computadoras representen los datos en binario.

2. Convierte el número binario 10011011 a decimal y a hexadecimal.

3. Investiga y describe cómo se representa una imagen en formato PNG en el disco.

4. Analiza la siguiente situación: ¿Qué sucede si intentas almacenar un número mayor al que puede representar un byte (por ejemplo, 300)? ¿Cómo lo maneja Python?

---

1. Las computadoras representan los datos en binario porque es la forma más simple, confiable y eficiente de procesar y almacenar información usando circuitos electrónicos, porque solo hay dos posibilidades 1 o 0, encendido o apagado, si o no, bueno o malo. Ya la cantidades de combinaciones que se puedem hacer con esas respuestas es mayor pero en si el nucleo no cambia. Y para un camputadora es mucho mas facil procesar datos asi de especificos y faciles que un monton de datos más complejos.


2. Para convertir el numero binario 10011011 a decimal primero se ordena el numero y de derecha a izquierda se le asignan numeros: 

| Numero| Potencia de 2 | Resultado |
|-----|-----------------|-----------|
| 1   | 2<sup>7</sup>  | 128       |
| 0   | 2<sup>6</sup>  | 0         |
| 0   | 2<sup>5</sup>  | 0         |
| 1   | 2<sup>4</sup>  | 16        |
| 1   | 2<sup>3</sup>  | 8         |
| 0   | 2<sup>2</sup>  | 0         |
| 1   | 2<sup>1</sup>  | 2         |
| 1   | 2<sup>0</sup>  | 1         |

128 + 0 + 0 + 16 + 8 + 0 + 2 + 1 = 155 

### Número en decimal: 155

Para convertirlo a hexadecimal:

Se agrupa de 4 en 4 desde la derecha:

1001 1011

Y se convierte cada grupo:

- 1001 = 9  
- 1011 = 11 = B

### Número hexadecimal: 9B₁₆

---

3. El formato PNG es un tipo de archivo gráfico que almacena imágenes comprimidas sin pérdida de calidad.
Cuando una imagen PNG se guarda en el disco, no se guarda como una "imagen visual", sino como una estructura de datos binarios, organizada en varias secciones llamadas "chunks" (bloques). Cada uno tiene una función específica.

La estructura básica de un archivo PNG es:
1) Firma PNG.

Son los primeros 8 bytes del archivo.
Sirven para identificar que el archivo es PNG.

2) Chunks o bloques de información.

Después de la firma, el archivo contiene una serie de bloques que siguen este formato:

- IHDR: Contiene información básica como el tamaño de la imagen, profundidad de color, tipo de compresión, etc.

- PLTE (opcional): Define una paleta de colores, si se usa.

- IDAT: Aquí están los datos de la imagen, comprimidos con el algoritmo DEFLATE.

- IEND: Indica el final del archivo PNG.

---


4. Un solo byte solo puede almacenar números hasta 255. y si se intenta guardar un número mayor, Python lanza un "ValueError".

Para representar valores mayores, se necesita usar más de un byte.
Y en python se puede hacer con los comandos de:

    .to_bytes()
    
    .from_bytes()

