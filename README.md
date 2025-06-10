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

1. Modelos de sistemas complejos
Se pueden construir a partir de:

Funciones de transferencia individuales.

Modelos existentes para componentes comunes.

Sin fórmulas específicas en esta diapositiva.

2. Solenoide
Partes:

Circuito eléctrico

Transductor electromecánico

Sistema mecánico

Fórmulas clave:

Fuerza del electroimán:

𝐹
(
𝑡
)
∝
𝑖
(
𝑡
)
F(t)∝i(t)
Donde 
𝑖
(
𝑡
)
i(t) es la corriente en la bobina.

Dinámica mecánica (con resorte y amortiguador):

𝑀
𝑥
¨
(
𝑡
)
+
𝐵
𝑥
˙
(
𝑡
)
+
𝐾
𝑥
(
𝑡
)
=
𝐹
(
𝑡
)
M 
x
¨
 (t)+B 
x
˙
 (t)+Kx(t)=F(t)
Ejemplo: Un solenoide que mueve una válvula proporcionalmente al voltaje aplicado.

3. Motor DC (Corriente de campo constante)
Ecuaciones clave:

Flujo magnético:

𝜙
∝
𝑖
𝑓
ϕ∝i 
f
​
 
Torque:

𝑇
=
𝐾
𝑇
𝜙
𝑖
𝑎
T=K 
T
​
 ϕi 
a
​
 
Voltaje inducido:

𝑒
𝑎
=
𝐾
𝑒
𝜔
e 
a
​
 =K 
e
​
 ω
Ecuación eléctrica:

𝑉
𝑎
=
𝑅
𝑎
𝑖
𝑎
+
𝐿
𝑎
𝑑
𝑖
𝑎
𝑑
𝑡
+
𝑒
𝑎
V 
a
​
 =R 
a
​
 i 
a
​
 +L 
a
​
  
dt
di 
a
​
 
​
 +e 
a
​
 
Dinámica mecánica:

𝐽
𝑑
𝜔
𝑑
𝑡
+
𝐵
𝜔
=
𝑇
J 
dt
dω
​
 +Bω=T
4. Motor DC (Corriente de armadura)
Asumiendo 
𝑖
𝑓
=
cte
⇒
𝜙
=
cte
i 
f
​
 =cte⇒ϕ=cte, se simplifica:

Torque:

𝑇
=
𝐾
𝑖
𝑎
T=Ki 
a
​
 
Ecuación completa:

𝑉
𝑎
=
𝑅
𝑎
𝑖
𝑎
+
𝐿
𝑎
𝑑
𝑖
𝑎
𝑑
𝑡
+
𝐾
𝜔
V 
a
​
 =R 
a
​
 i 
a
​
 +L 
a
​
  
dt
di 
a
​
 
​
 +Kω
Mecánica:

𝐽
𝑑
𝜔
𝑑
𝑡
+
𝐵
𝜔
=
𝐾
𝑖
𝑎
J 
dt
dω
​
 +Bω=Ki 
a
​
 
5. Engranajes y Poleas
Relación de transformación:

𝜃
2
=
𝑁
1
𝑁
2
𝜃
1
θ 
2
​
 = 
N 
2
​
 
N 
1
​
 
​
 θ 
1
​
 
𝜏
1
=
𝑁
2
𝑁
1
𝜏
2
τ 
1
​
 = 
N 
1
​
 
N 
2
​
 
​
 τ 
2
​
 
Efecto sobre parámetros:

𝐽
𝑒
𝑞
=
(
𝑁
1
𝑁
2
)
2
𝐽
carga
J 
eq
​
 =( 
N 
2
​
 
N 
1
​
 
​
 ) 
2
 J 
carga
​
 
6. Transmisión rotacional a lineal
Relación:

𝑥
=
𝑟
𝜃
x=rθ
𝐹
=
𝜏
𝑟
F= 
r
τ
​
 
7. Palancas
Principio de momentos:

𝐹
1
𝐿
1
=
𝐹
2
𝐿
2
F 
1
​
 L 
1
​
 =F 
2
​
 L 
2
​
 
8. Potenciómetros
Rotación:

𝑉
salida
=
(
𝜃
𝜃
max
)
𝑉
ref
V 
salida
​
 =( 
θ 
max
​
 
θ
​
 )V 
ref
​
 
Traslación:

𝑉
salida
=
(
𝑥
𝑥
max
)
𝑉
ref
V 
salida
​
 =( 
x 
max
​
 
x
​
 )V 
ref
​
 
9. Tacómetros
Conversión de velocidad angular a voltaje:

𝑉
=
𝐾
𝜔
V=Kω
10. Sensores transmisores
Lineales:

𝐻
(
𝑠
)
=
TO
PV
=
𝐾
H(s)= 
PV
TO
​
 =K
No lineales: requieren linealización (no se da fórmula explícita).

11. Mezcla de sustancias
Modelo de mezcla continua:

𝐺
(
𝑠
)
=
𝑄
(
𝑠
)
𝑄
𝑖
(
𝑠
)
=
𝜌
inicial
𝑠
+
𝜌
in
𝑣
in
𝑠
+
𝑣
out
G(s)= 
Q 
i
​
 (s)
Q(s)
​
 = 
s+v 
out
​
 
ρ 
inicial
​
 s+ρ 
in
​
 v 
in
​
 
​
 
Ejemplo:

𝐺
(
𝑠
)
=
2
𝑠
+
3
⋅
4
𝑠
+
4
=
2
𝑠
+
12
𝑠
+
4
G(s)= 
s+4
2s+3⋅4
​
 = 
s+4
2s+12
​
 
12. Sistema Térmico
Aunque el documento no incluye fórmulas detalladas, generalmente se modela como:

𝐶
𝑑
𝑇
𝑑
𝑡
=
𝑄
in
−
𝑇
−
𝑇
amb
𝑅
C 
dt
dT
​
 =Q 
in
​
 − 
R
T−T 
amb
​
 
​
 
donde:

𝐶
C es la capacidad térmica

𝑅
R la resistencia térmica

𝑇
T temperatura del sistema

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
