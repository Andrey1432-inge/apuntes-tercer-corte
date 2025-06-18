# FUNCION DE TRASNFERENCIA

## 1. Introducción a la Función de Transferencia

- Herramienta en el análisis de sistemas dinámicos.

- Derivada de la ecuación diferencial usando la transformada de Laplace.

## 2. Ejemplo de Transformada de Laplace

- Ecuación: $$𝑦̈ + 3𝑦̇ + 2𝑦 = 3𝑢̇ + 3𝑢$$

- Se transforma y despeja $$Y(s)/U(s)$$ para obtener la función de transferencia.

## 3. Definición de Función de Transferencia

- Es el cociente $$Y(s)/U(s)$$

- Solo válido si condiciones iniciales son cero.

## 4. Clasificación

- n > m: Impropia

- n < m: Estrictamente propia

- n = m: Bipropia

## 5. Zeros

- Se hallan igualando el numerador a cero: 

$$N(s) = 0$$

## 6. Polos

- Se hallan igualando el denominador a cero: 

$$D(s) = 0$$

## 7. Teorema del valor final

- Permite hallar el valor en

  $$lim(t→∞) = f(t) = lim(s→0) sF(s)$$

## 8. Entradas de prueba

- Escalón: 

$$\frac{A}{s}$$

- Rampa: 
 
$$\frac{A}{s^2}$$

- Parábola: 

$$\frac{A}{s^3}$$

## 9. Ejemplos resueltos

- Ejemplo 1: Hallar la función de transferencia

Ecuación:

$$𝑦¨ + 3𝑦˙ + 2𝑦 = 3𝑢˙ + 3𝑢$$

Transformada de Laplace (condiciones iniciales = 0):

$$𝑠^2𝑌(𝑠) + 3𝑠𝑌(𝑠) + 2𝑌(𝑠) = 3𝑠𝑈(𝑠) + 3𝑈(𝑠)$$

Despejamos $$\frac{𝑌(𝑠)}{𝑈(𝑠)}:

$$\frac{𝑌(𝑠)}{𝑈(𝑠)} = \frac{3𝑠 + 3}{𝑠^2 + 3𝑠 + 2}

- Ejemplo 2: Encontrar Zeros y Polos

Función de transferencia:

$$𝐺(𝑠) = \frac{3𝑠 − 1}{𝑠^2 + 3𝑠 + 2}
 
Zeros:

Numerador = 0 → 3𝑠 − 1 = 0 → 𝑠 = \frac{1}{3}
​
Polos:

Denominador = 0 → 𝑠^2 + 3𝑠 + 2 = 0 → 𝑠 = −1 , −2

## 10. Actividad final resuelta

- Ecuación diferencial:

$$𝑦¨¨ + 5𝑦''' + 13.5𝑦¨ + 3.75𝑦 = 7.5𝑢˙ + 3.75𝑢$$

Función de transferencia (condiciones iniciales = 0)

Transformamos:

$$(𝑠^3 + 5𝑠^2 + 13.5𝑠 + 3.75)𝑌(𝑠) = (7.5𝑠 + 3.75)𝑈(𝑠)$$

$$𝐺(𝑠) = \frac{𝑌(𝑠)}{𝑈(𝑠)} = \frac{7.5𝑠 + 3.75}{𝑠^3 + 5𝑠^2 + 13.5𝑠 + 3.75}$$
 
Zeros:

Numerador = 0 → 7.5𝑠 + 3.75 = 0 → 𝑠 = −0.5

Polos:

Resolvemos 

$$𝑠^3 + 5𝑠^2 + 13.5𝑠 + 3.75 = 0$$ 

(Usamos factorización o método numérico; aproximado)
Raíces (estimadas): Una real y dos complejas conjugadas.

$$𝑠_1 ≈ −0.293$$ (real)
$$𝑠_2 ≈ −2.354 + 1.797𝑖$$ (complejo)
$$𝑠_3 ≈ − 2.354 − 1.797𝑖$$ (complejo conjugado)

Valor final frente a entrada escalón unitario:

Entrada escalón: 

$$𝑈(𝑠) = \frac{1}{𝑠}$$

$$𝑌(𝑠) = \frac{7.5𝑠 + 3.75}{𝑠(𝑠^3 + 5𝑠^2 + 13.5𝑠 + 3.75)}
 
$$lim_{𝑠 → 0}𝑠𝑌(𝑠) = lim_{⁡𝑠 → 0}\frac{7.5𝑠 + 3.75}{𝑠^3 + 5𝑠^2 + 13.5𝑠 + 3.75} = \frac{3.75}{3.75} = 1

# 2. Modelamiento por diagramas

## 1. Modelos de sistemas complejos

Se pueden construir a partir de:

 -Funciones de transferencia individuales.

 -Modelos existentes para componentes comunes.

## 2. Solenoide

**Partes:**

1. Circuito eléctrico

2. Transductor electromecánico

3. Sistema mecánico

- **Fórmulas clave:**

Fuerza del electroimán:

$$F(t)∝i(t)$$

- Donde $$i(t)$$ es la corriente en la bobina.

Dinámica mecánica (con resorte y amortiguador):

$$Mx¨(t) + Bx˙(t)+Kx(t)=F(t)$$

- Ejemplo: Un solenoide que mueve una válvula proporcionalmente al voltaje aplicado.

## 3. Motor DC (Corriente de campo constante)

**Ecuaciones clave:**

1. Flujo magnético:

$$𝜙∝𝑖_𝑓$$
 
2. Torque:

$$𝑇=𝐾_𝑇𝜙𝑖_𝑎$$
 
3. Voltaje inducido:

$$𝑒_𝑎=K_𝑒𝜔$$

4. Ecuación eléctrica:

$$𝑉_𝑎=𝑅_𝑎𝑖_𝑎 + 𝐿_𝑎\frac{𝑑𝑖_𝑎}{𝑑𝑡} + 𝑒_𝑎$$
 
5. Dinámica mecánica:

$$𝐽\frac{𝑑𝜔}{𝑑𝑡} + 𝐵𝜔 = 𝑇$$

## 4. Motor DC (Corriente de armadura)

Asumiendo $$𝑖_𝑓 = cte ⇒ 𝜙 = cte$$, se simplifica:

1. Torque:

$$𝑇 = 𝐾𝑖_𝑎$$

2. Ecuación completa:

$$𝑉_𝑎 = 𝑅_𝑎𝑖_𝑎 + 𝐿_𝑎\frac{𝑑𝑖_𝑎}{𝑑𝑡} + 𝐾𝜔$$

3. Mecánica:

$$𝐽\frac{𝑑𝜔}{𝑑𝑡} + 𝐵𝜔 = 𝐾𝑖_𝑎$$

## 5. Engranajes y Poleas

- Relación de transformación:

$$𝜃_2 = \frac{𝑁_1}{𝑁_2}𝜃_1$$
 
$$𝜏_1 = \frac{𝑁_2}{𝑁_1}𝜏_2$$
 
- Efecto sobre parámetros:

$$𝐽_{eq} =(\frac{𝑁_1}{𝑁_2})^2*𝐽_{carga}$$
 
## 6. Transmisión rotacional a lineal

- Relación:

$$𝑥 = 𝑟𝜃$$

$$𝐹 = \frac{𝜏}{𝑟}$$ 
 
## 7. Palancas

- Principio de momentos:

$$𝐹_1𝐿_1 = 𝐹_2𝐿_2$$
 
## 8. Potenciómetros

- Rotación:

$$𝑉_{salida} = (\frac{𝜃}{𝜃_{max}})𝑉_{ref}$$

- Traslación:

$$𝑉_{salida} = (\frac{𝑥}{𝑥_{max}})𝑉_{ref}$$
 
## 9. Tacómetros

- Conversión de velocidad angular a voltaje:

$$𝑉 = 𝐾𝜔$$

## 10. Sensores transmisores

- Lineales:

$$𝐻(𝑠) = \frac{TO}{PV} = 𝐾$$

- No lineales: requieren linealización (no se da fórmula explícita).

## 11. Mezcla de sustancias

- Modelo de mezcla continua:

$$𝐺(𝑠) = \frac{𝑄(𝑠)}{𝑄_𝑖(𝑠)} = \frac{𝜌_{inicial}𝑠 + 𝜌_{in}𝑣_{in}}{𝑠 + 𝑣_{out}}$$
 
**Ejemplo:**

$$𝐺(𝑠) = \frac{2𝑠 + 3 ⋅ 4}{𝑠 + 4} = \frac{2𝑠 + 12}{𝑠 + 4}$$
 
## 12. Sistema Térmico
Aunque el documento no incluye fórmulas detalladas, generalmente se modela como:

$$𝐶\frac{𝑑𝑇}{𝑑𝑡} = 𝑄_{in} − \frac{𝑇 − 𝑇_{amb}}{𝑅}$$

donde:

- C es la capacidad térmica
- R la resistencia térmica
- T temperatura del sistema

# 3. ALGEBRA DE BLOQUES

## 1. Definicion:

- Bloque funcional: representa una operación matemática entre entrada y salida.

**Ejemplo:**

- Entrada: $$𝑈(𝑠)$$, Bloque: $$𝐺(𝑠)$$, Salida: $$𝑌(𝑠)$$

**Fórmula:**

$$𝑌(𝑠) = 𝐺(𝑠) ⋅ 𝑈(𝑠)$$

## 2. Elementos del diagrama de bloques

- Flechas: indican dirección de señal (entrada → salida).

- Punto de suma: combina señales con signos + / −.

**Ejemplo:**

$$𝐸(𝑠) = 𝑅(𝑠) − 𝑌(𝑠)$$

## 3. Ramificación

- Una señal se dirige a múltiples bloques o puntos de suma.

**Ejemplo:**

$$𝑈(𝑠) → 𝐺_1(𝑠) y 𝐺_2(𝑠)$$ simultáneamente.

## 4. Interpretación

- La salida es el producto entre la entrada y la función del bloque.

**Fórmula:**

$$𝑌(𝑠) = 𝐺(𝑠) ⋅ 𝑈(𝑠)$$

## 5. Bloques en cascada

- Multiplicación secuencial de bloques.

**Fórmula:**

$$𝑌(𝑠) = 𝐺_1(𝑠) ⋅ 𝐺_2(𝑠) ⋅ 𝑈(𝑠)$$
​
## 6. Álgebra de bloques

- Permite reducir diagramas complejos a una sola función de transferencia.

- Se aplican reglas de simplificación.

## 7. Lazo de realimentación positiva

**Fórmulas:**

$$𝑌(𝑠) = \frac{𝐺_1(𝑠)}{1 − 𝐺_1(𝑠)𝐺_2(𝑠)} ⋅ 𝑋(𝑠)$$

## 8. Lazo de realimentación negativa

- Caso más común en control.

**Fórmula:**

$$𝑌(𝑠) = \frac{𝐺_1(𝑠)}{1 + 𝐺_1(𝑠)𝐺_2(𝑠)} ⋅ 𝑋(𝑠)$$

## 9. Aplicación del álgebra de bloques

- Ejemplo de reducción de un sistema con varias entradas:

$$\frac{𝑌(𝑠)}{𝑋_1(𝑠)} = 𝐺_3(𝑠)((𝐺_1(𝑠) − 𝐺_2(𝑠)), \frac{𝑌(𝑠)}{𝑋_2(𝑠)} = 𝐺_4(𝑠) − 1$$

## 10. Ejemplo práctico

- Hallar $$\\frac{𝐶(𝑠)}{𝑅(𝑠)}$$ mediante simplificación de bloques.

## 11. Resumen

- Los diagramas de bloques son clave para entender sistemas complejos.

- La realimentación negativa es esencial.

- El álgebra de bloques permite deducir funciones de transferencia fácilmente.

# DIAGRAMA DE FLUJO DE SEÑAL

## 1. Introducción

- Usos: Representación de sistemas complejos.

- Objetivo: Obtener la función de transferencia total de forma sistemática.

- Herramienta principal: Fórmula de Mason.

## 2. Elementos del diagrama

- Nodo: Representa una señal (entrada o salida).

- Flecha: Representa una relación entre nodos mediante una función de transferencia (por ejemplo, $$𝐺(𝑠)$$).

## 3. Interpretación

- Se sigue el flujo de las señales, como en un sistema dinámico.

## 4. Comparación con diagramas de bloques

- Los diagramas de flujo de señal permiten un análisis más directo de sistemas complejos que los diagramas de bloques tradicionales.

## 5. Definiciones clave

- Camino directo: Ruta desde entrada a salida sin repetir nodos.

- Lazo (loop): Camino cerrado que regresa al mismo nodo.

- Ganancia de camino: Producto de las funciones de transferencia en ese camino.

- Ganancia de lazo: Producto de funciones de transferencia de un lazo.

## 6. Fórmula de Mason

$$\frac{𝐶(𝑠)}{𝑅(𝑠)} = \frac{∑𝑃_𝑘Δ_𝑘}{Δ}$$
 
- 𝑃_𝑘: Ganancia de cada camino directo.

- Δ: Determinante total del sistema:

$$Δ = 1 − ∑𝐿_𝑖 + ∑𝐿_𝑖𝐿_𝑗 − ∑𝐿_𝑖𝐿_𝑗𝐿_𝑘 + ⋯$$

- Δ_𝑘: Determinante sin los lazos que tocan el camino 𝑃_𝑘.

## 7. Ejemplos resueltos

- **Ejemplo 1**

- Camino directo:

$$𝑃_1 = 𝐺_1𝐺_2𝐺_3$$
 
- Lazos:
  - $$𝐿_1 = 𝐺_1𝐺_2𝐻_1$$
  
  - $$𝐿_2 = −𝐺_2𝐺_3𝐻_2$$

  - $$𝐿_3 = −𝐺_1𝐺_2𝐺_3$$

- Determinante:

$$Δ = 1 − (𝐿_1 + 𝐿_2 + 𝐿_3)$$

- Resultado:

$$\frac{𝐶(𝑠)}{𝑅(𝑠)} = \frac{𝐺_1𝐺_2𝐺_3}{Δ}$$
 
- **Ejemplo 2**

- 3 caminos directos:

  - $$𝑃_1 = 𝐺_1𝐺_2𝐺_3𝐺_4𝐺_5$$ 
  - $$𝑃_2 = 𝐺_1𝐺_6𝐺_4𝐺_5$$
  - $$𝑃_3 = 𝐺_1𝐺_2𝐺_7$$

- Lazos:

  - $$𝐿_1 = −𝐺_4𝐻_1$$
  - $$𝐿_2 = −𝐺_2𝐺_7𝐻_2$$
  - $$𝐿_3 = −𝐺_6𝐺_4𝐺_5𝐻_2$$
  - $$𝐿_4 = −𝐺_2𝐺_3𝐺_4𝐺_5𝐻_2$$
 
- Determinante:

  - $$Δ = 1 − 𝐿_1 + 𝐿_2 + 𝐿_3 + 𝐿_4 + 𝐿_1𝐿_2$$
 
- Cofactores:
  
  - $$Δ_1 = 1$$
  - $$Δ_2 = 1$$
  - $$Δ_3 = 1 − 𝐿_1$$
 
- Resultado:

$$\frac{𝐶(𝑠)}{𝑅(𝑠)} = \frac{𝑃_1Δ_1 + 𝑃_2Δ_2 + 𝑃_3Δ_3}{Δ}$$
​
## 8. Cómo resolver un problema con Mason paso a paso

1. Identificar los caminos directos $$𝑃_𝑘$$ y calcular su ganancia.
2. Identificar los lazos $$𝐿_𝑖$$ y su ganancia.
3. Calcular Δ: considerar la combinación de lazos que no se tocan entre sí.
4. Para cada camino directo $$𝑃_𝑘$$, calcular su cofactor $$Δ_𝑘$$ ignorando los lazos que lo tocan.
5. Aplicar la fórmula de Mason:

$$\frac{𝐶(𝑠)}{𝑅(𝑠)} = \frac{∑𝑃_𝑘Δ_𝑘}{Δ}$$
