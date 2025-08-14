# Ejercicios

1. **Verificación de peso de despegue**
    
    En una pista de pruebas de aeronaves, el sistema debe verificar si el peso total de la aeronave, incluyendo combustible y carga, supera el límite máximo permitido para el despegue. Dependiendo del resultado, el sistema deberá indicar si la aeronave está lista para despegar o si debe reducir carga o combustible.
    
## Analisis

| Variables de entrada| Descripción |
|---------------------|-------------|
| Combustible | Peso del combustible de la aeronave |
| Carga | Peso de la carga de la aeronave |

| Variable intermedia | Descripción |
|--------------------|-------------|
| Peso_total | El peso total del avión |
|  |  |

| Constante | Descripción |
|--------------------|-------------|
| 5000 | Peso limite de la aeronave (kg)|


## Pseudocódigo:
```
Inicio
Leer combustible, carga
Peso_total = Carga + Combustible

Si Peso_total > 5000
    Mostrar "Aeronave no lista para despegar"
Si no
    Mostrar "Aeronave lista para despegar"
Fin Si
FIN

```
---

2. **Control de temperatura del motor**
    
    Durante una inspección de rutina, se mide la temperatura de un motor de turbina. Si la temperatura es mayor a un valor crítico, se debe indicar "Peligro: sobrecalentamiento". Si está dentro del rango seguro, indicar "Operación normal". Si es demasiado baja, indicar "Motor frío – Calentar antes de operar".

## Análisis
 
 | Variables de entrada| Descripción |
|---------------------|-------------|
| Temperatura |  Peso total de la aeronave |

| Variable de salida | Descripción |
|--------------------|-------------|
|  |  |

| Constante | Descripción |
|--------------------|-------------|
| 15000 | Temperatura critica maxima del motor (C°)|
| 400 | Temperatura critica minima del motor (C°)|

## Pseudocódigo:
```
Inicio
Leer temperatura

Si Temperatura > 15000
    Mostrar "Peligro: sobrecalentamiento"
Si no
    Si temperatura < 1500 y temperatura > 400
    Mostrar "Operación normal"
    Si no
        Mostrar "Motor frío – Calentar antes de operar"
Fin Si
FIN
```

---

1. **Registro de altitudes de vuelo**
    
    Un sistema debe registrar la altitud de vuelo cada 10 minutos durante una hora y mostrar todas las mediciones al final.

## Análisis
 
| Variables de entrada| Descripción |
|---------------------|-------------|
| Altitud | Peso total de la aeronave |

| Variable de salida | Descripción |
|--------------------|-------------|
| Altitud |  |

| Control | Descripción |
|--------------------|-------------|
| i | Temperatura critica maxima del motor (C°)|

| Constante | Descripción |
|--------------------|-------------|
| 6 | Las veces que se repita  |


## Pseudocódigo:

```
Inicio
i = 0
Mientras i = 7
    Leer dato
    Estatura [i]
    i = i + 1
Fin Mientras
```
---

2. **Control de combustible en pruebas**
    
    Durante un ensayo en banco de un motor a reacción, se mide el nivel de combustible cada minuto y se detiene el registro cuando el combustible baja del 10%. Mostrar el tiempo total de operación antes de llegar a ese punto.