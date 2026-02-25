# Actividad2
## A1 → A2

### Descripción
- Rotación positiva de 90° alrededor del eje Y  
- Traslación positiva en el eje Z una distancia \( L_0 \)

### Matriz de rotación en Y (forma general)

$$
R_y(\theta)=
\begin{bmatrix}
\cos\theta & 0 & \sin\theta \\
0 & 1 & 0 \\
-\sin\theta & 0 & \cos\theta
\end{bmatrix}
$$

### Evaluación en \( 90^\circ \)

$$
R_y(90^\circ\) =
\begin{bmatrix}
0 & 0 & 1 \\
0 & 1 & 0 \\
-1 & 0 & 0
\end{bmatrix}
$$


### Vector de traslación

$$
P =
\begin{bmatrix}
0 \\
0 \\
L_0
\end{bmatrix}
$$


### Matriz de transformación homogénea

$$
T_{12} =
\begin{bmatrix}
0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0 \\
-1 & 0 & 0 & L_0 \\
0 & 0 & 0 & 1
\end{bmatrix}
$$
