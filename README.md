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

$$𝐺(𝑠) = frac{2𝑠 + 3 ⋅ 4}{𝑠 + 4} = \frac{2𝑠 + 12}{𝑠 + 4}$$
 
## 12. Sistema Térmico
Aunque el documento no incluye fórmulas detalladas, generalmente se modela como:

$$𝐶\frac{𝑑𝑇}{𝑑𝑡} = 𝑄_{in} − \frac{𝑇 − 𝑇_{amb}}{𝑅}$$

donde:

- C es la capacidad térmica
- R la resistencia térmica
- T temperatura del sistema

# 3. ALGEBRA DE BLOQUES

Bloque funcional: representa una operación matemática entre entrada y salida.

Ejemplo:
Entrada: 
𝑈
(
𝑠
)
U(s), Bloque: 
𝐺
(
𝑠
)
G(s), Salida: 
𝑌
(
𝑠
)
Y(s)
Fórmula:

𝑌
(
𝑠
)
=
𝐺
(
𝑠
)
⋅
𝑈
(
𝑠
)
Y(s)=G(s)⋅U(s)
📊 Diapositivas 3–5: Elementos del diagrama de bloques
Flechas: indican dirección de señal (entrada → salida).

Punto de suma: combina señales con signos + / −.

Ejemplo:

𝐸
(
𝑠
)
=
𝑅
(
𝑠
)
−
𝑌
(
𝑠
)
E(s)=R(s)−Y(s)
📊 Diapositiva 6: Ramificación
Una señal se dirige a múltiples bloques o puntos de suma.

Ejemplo:
𝑈
(
𝑠
)
→
𝐺
1
(
𝑠
)
U(s)→G 
1
​
 (s) y 
𝐺
2
(
𝑠
)
G 
2
​
 (s) simultáneamente.

📊 Diapositiva 7: Interpretación
La salida es el producto entre la entrada y la función del bloque.

Fórmula:

𝑌
(
𝑠
)
=
𝐺
(
𝑠
)
⋅
𝑈
(
𝑠
)
Y(s)=G(s)⋅U(s)
📊 Diapositiva 8: Bloques en cascada
Multiplicación secuencial de bloques.

Fórmula:

𝑌
(
𝑠
)
=
𝐺
1
(
𝑠
)
⋅
𝐺
2
(
𝑠
)
⋅
𝑈
(
𝑠
)
Y(s)=G 
1
​
 (s)⋅G 
2
​
 (s)⋅U(s)
📊 Diapositiva 11: Álgebra de bloques
Permite reducir diagramas complejos a una sola función de transferencia.

Se aplican reglas de simplificación.

📊 Diapositiva 13: Lazo de realimentación positiva
Fórmulas:

𝑌
(
𝑠
)
=
𝐺
1
(
𝑠
)
1
−
𝐺
1
(
𝑠
)
𝐺
2
(
𝑠
)
⋅
𝑋
(
𝑠
)
Y(s)= 
1−G 
1
​
 (s)G 
2
​
 (s)
G 
1
​
 (s)
​
 ⋅X(s)
📊 Diapositiva 14: Lazo de realimentación negativa
Caso más común en control.

Fórmula:

𝑌
(
𝑠
)
=
𝐺
1
(
𝑠
)
1
+
𝐺
1
(
𝑠
)
𝐺
2
(
𝑠
)
⋅
𝑋
(
𝑠
)
Y(s)= 
1+G 
1
​
 (s)G 
2
​
 (s)
G 
1
​
 (s)
​
 ⋅X(s)
📊 Diapositivas 16–18: Aplicación del álgebra de bloques
Ejemplo de reducción de un sistema con varias entradas:

𝑌
(
𝑠
)
𝑋
1
(
𝑠
)
=
𝐺
3
(
𝑠
)
(
𝐺
1
(
𝑠
)
−
𝐺
2
(
𝑠
)
)
,
𝑌
(
𝑠
)
𝑋
2
(
𝑠
)
=
𝐺
4
(
𝑠
)
−
1
X 
1
​
 (s)
Y(s)
​
 =G 
3
​
 (s)(G 
1
​
 (s)−G 
2
​
 (s)), 
X 
2
​
 (s)
Y(s)
​
 =G 
4
​
 (s)−1
📊 Diapositiva 19: Ejemplo práctico
Hallar 
𝐶
(
𝑠
)
𝑅
(
𝑠
)
R(s)
C(s)
​
  mediante simplificación de bloques.

📊 Diapositiva 20: Resumen
Los diagramas de bloques son clave para entender sistemas complejos.

La realimentación negativa es esencial.

El álgebra de bloques permite deducir funciones de transferencia fácilmente.

# DIAGRAMA DE FLUJO DE SEÑAL

Diapositiva 2 – Introducción
Usos: Representación de sistemas complejos.

Objetivo: Obtener la función de transferencia total de forma sistemática.

Herramienta principal: Fórmula de Mason.

Diapositivas 3–4 – Elementos del diagrama
Nodo: Representa una señal (entrada o salida).

Flecha: Representa una relación entre nodos mediante una función de transferencia (por ejemplo, 
𝐺
(
𝑠
)
G(s)).

Diapositiva 5 – Interpretación
Se sigue el flujo de las señales, como en un sistema dinámico.

Diapositiva 6 – Comparación con diagramas de bloques
Los diagramas de flujo de señal permiten un análisis más directo de sistemas complejos que los diagramas de bloques tradicionales.

Diapositivas 8–10 – Definiciones clave
Camino directo: Ruta desde entrada a salida sin repetir nodos.

Lazo (loop): Camino cerrado que regresa al mismo nodo.

Ganancia de camino: Producto de las funciones de transferencia en ese camino.

Ganancia de lazo: Producto de funciones de transferencia de un lazo.

📐 Diapositiva 12 – Fórmula de Mason
𝐶
(
𝑠
)
𝑅
(
𝑠
)
=
∑
𝑃
𝑘
Δ
𝑘
Δ
R(s)
C(s)
​
 = 
Δ
∑P 
k
​
 Δ 
k
​
 
​
 
𝑃
𝑘
P 
k
​
 : Ganancia de cada camino directo.

Δ
Δ: Determinante total del sistema:

Δ
=
1
−
∑
𝐿
𝑖
+
∑
𝐿
𝑖
𝐿
𝑗
−
∑
𝐿
𝑖
𝐿
𝑗
𝐿
𝑘
+
⋯
Δ=1−∑L 
i
​
 +∑L 
i
​
 L 
j
​
 −∑L 
i
​
 L 
j
​
 L 
k
​
 +⋯
Δ
𝑘
Δ 
k
​
 : Determinante sin los lazos que tocan el camino 
𝑃
𝑘
P 
k
​
 .

🧮 Ejemplos resueltos
Ejemplo 1 – Diapositiva 13
Camino directo:

𝑃
1
=
𝐺
1
𝐺
2
𝐺
3
P 
1
​
 =G 
1
​
 G 
2
​
 G 
3
​
 
Lazos:

𝐿
1
=
𝐺
1
𝐺
2
𝐻
1
L 
1
​
 =G 
1
​
 G 
2
​
 H 
1
​
 

𝐿
2
=
−
𝐺
2
𝐺
3
𝐻
2
L 
2
​
 =−G 
2
​
 G 
3
​
 H 
2
​
 

𝐿
3
=
−
𝐺
1
𝐺
2
𝐺
3
L 
3
​
 =−G 
1
​
 G 
2
​
 G 
3
​
 

Determinante:

Δ
=
1
−
(
𝐿
1
+
𝐿
2
+
𝐿
3
)
Δ=1−(L 
1
​
 +L 
2
​
 +L 
3
​
 )
Resultado:

𝐶
(
𝑠
)
𝑅
(
𝑠
)
=
𝐺
1
𝐺
2
𝐺
3
Δ
R(s)
C(s)
​
 = 
Δ
G 
1
​
 G 
2
​
 G 
3
​
 
​
 
Ejemplo 2 – Diapositiva 14
3 caminos directos:

𝑃
1
=
𝐺
1
𝐺
2
𝐺
3
𝐺
4
𝐺
5
,
𝑃
2
=
𝐺
1
𝐺
6
𝐺
4
𝐺
5
,
𝑃
3
=
𝐺
1
𝐺
2
𝐺
7
P 
1
​
 =G 
1
​
 G 
2
​
 G 
3
​
 G 
4
​
 G 
5
​
 ,P 
2
​
 =G 
1
​
 G 
6
​
 G 
4
​
 G 
5
​
 ,P 
3
​
 =G 
1
​
 G 
2
​
 G 
7
​
 
Lazos:

𝐿
1
=
−
𝐺
4
𝐻
1
,
𝐿
2
=
−
𝐺
2
𝐺
7
𝐻
2
,
𝐿
3
=
−
𝐺
6
𝐺
4
𝐺
5
𝐻
2
,
𝐿
4
=
−
𝐺
2
𝐺
3
𝐺
4
𝐺
5
𝐻
2
L 
1
​
 =−G 
4
​
 H 
1
​
 ,L 
2
​
 =−G 
2
​
 G 
7
​
 H 
2
​
 ,L 
3
​
 =−G 
6
​
 G 
4
​
 G 
5
​
 H 
2
​
 ,L 
4
​
 =−G 
2
​
 G 
3
​
 G 
4
​
 G 
5
​
 H 
2
​
 
Determinante:

Δ
=
1
−
𝐿
1
+
𝐿
2
+
𝐿
3
+
𝐿
4
+
𝐿
1
𝐿
2
Δ=1−L 
1
​
 +L 
2
​
 +L 
3
​
 +L 
4
​
 +L 
1
​
 L 
2
​
 
Cofactores:

Δ
1
=
1
,
Δ
2
=
1
,
Δ
3
=
1
−
𝐿
1
Δ 
1
​
 =1,Δ 
2
​
 =1,Δ 
3
​
 =1−L 
1
​
 
Resultado:

𝐶
(
𝑠
)
𝑅
(
𝑠
)
=
𝑃
1
Δ
1
+
𝑃
2
Δ
2
+
𝑃
3
Δ
3
Δ
R(s)
C(s)
​
 = 
Δ
P 
1
​
 Δ 
1
​
 +P 
2
​
 Δ 
2
​
 +P 
3
​
 Δ 
3
​
 
​
 
🧩 Cómo resolver un problema con Mason paso a paso
Identificar los caminos directos 
𝑃
𝑘
P 
k
​
  y calcular su ganancia.

Identificar los lazos 
𝐿
𝑖
L 
i
​
  y su ganancia.

Calcular Δ: considerar la combinación de lazos que no se tocan entre sí.

Para cada camino directo 
𝑃
𝑘
P 
k
​
 , calcular su cofactor 
Δ
𝑘
Δ 
k
​
  ignorando los lazos que lo tocan.

Aplicar la fórmula de Mason:

𝐶
(
𝑠
)
𝑅
(
𝑠
)
=
∑
𝑃
𝑘
Δ
𝑘
Δ
R(s)
C(s)
​
 = 
Δ
∑P 
k
​
 Δ 
k
​
 
​
 
📘 Actividades (Diapositivas 16–17)
Reducir por álgebra de bloques una función de transferencia.

Convertir a diagrama de flujo de señal y resolver con Mason.
