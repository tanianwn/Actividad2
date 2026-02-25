# Actividad 2

## A1 → A2

### Descripción
- Rotación positiva de 90° alrededor del eje Y
- Traslación positiva en el eje Z una distancia $L_0$

### Matriz de rotación en Y (forma general)

$$
R_y(\theta)=
\begin{bmatrix}
\cos\theta & 0 & \sin\theta \\
0 & 1 & 0 \\
-\sin\theta & 0 & \cos\theta
\end{bmatrix}
$$

### Matriz de rotación en Z (forma general)

$$
R_z(\theta)=
\begin{bmatrix}
\cos\theta & -\sin\theta & 0 \\
\sin\theta & \cos\theta & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

### Multiplicación

$$
R = R_y(90^\circ) R_z(\theta)
$$

$$
R =
\begin{bmatrix}
0 & 0 & 1 \\
0 & 1 & 0 \\
-1 & 0 & 0
\end{bmatrix}
\begin{bmatrix}
\cos\theta & -\sin\theta & 0 \\
\sin\theta & \cos\theta & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

### Resultado

$$
R =
\begin{bmatrix}
0 & 0 & 1 \\
\sin\theta & \cos\theta & 0 \\
-\cos\theta & \sin\theta & 0
\end{bmatrix}
$$

### Evaluación en $90^\circ$

$$
R_y(90^\circ) =
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
\sin\theta & \cos\theta & 0 & 0 \\
-\cos\theta & \sin\theta & 0 & L_0 \\
0 & 0 & 0 & 1
\end{bmatrix}
$$

---

## A2 → A3

### Descripción
- Rotación alrededor del eje Z1 con ángulo $\theta_2$
- Traslación positiva de $L_2$ sobre el eje Z1

### Matriz de rotación

$$
R_{23}=R_z(\theta_2)
$$

$$
R_{23}=
\begin{bmatrix}
\cos\theta_2 & -\sin\theta_2 & 0 \\
\sin\theta_2 & \cos\theta_2 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

### Vector de traslación

$$
P =
\begin{bmatrix}
-L_2 \cos\theta_2 \\
-L_2 \sin\theta_2 \\
0
\end{bmatrix}
$$

### Matriz homogénea

$$
T_{23}=
\begin{bmatrix}
\cos\theta_2 & -\sin\theta_2 & 0 & -L_2\cos\theta_2 \\
\sin\theta_2 & \cos\theta_2 & 0 & -L_2\sin\theta_2 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}
$$

---

## A3 → A4

### Descripción
- Rotación alrededor del eje Z2 con ángulo $\theta_3$
- Rotación positiva de 90° alrededor del eje X2
- Traslación negativa en XY en $L_3$

### Matriz de rotación en Z (forma general)

$$
R_z(\theta)=
\begin{bmatrix}
\cos\theta & -\sin\theta & 0 \\
\sin\theta & \cos\theta & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

### Matriz de rotación en X (forma general)

$$
R_x(\theta)=
\begin{bmatrix}
1 & 0 & 0 \\
0 & \cos\theta & -\sin\theta \\
0 & \sin\theta & \cos\theta
\end{bmatrix}
$$

### Evaluación en $90^\circ$

$$
R_x(90^\circ)=
\begin{bmatrix}
1 & 0 & 0 \\
0 & 0 & -1 \\
0 & 1 & 0
\end{bmatrix}
$$

### Multiplicación

$$
R = R_z(\theta_3) R_x(90^\circ)
$$

$$
R =
\begin{bmatrix}
\cos\theta_3 & -\sin\theta_3 & 0 \\
\sin\theta_3 & \cos\theta_3 & 0 \\
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix}
1 & 0 & 0 \\
0 & 0 & -1 \\
0 & 1 & 0
\end{bmatrix}
$$

### Resultado

$$
R =
\begin{bmatrix}
\cos\theta_3 & 0 & \sin\theta_3 \\
\sin\theta_3 & 0 & -\cos\theta_3 \\
0 & 1 & 0
\end{bmatrix}
$$

### Vector de traslación

$$
P =
\begin{bmatrix}
- L_3 \sin\theta_3 \\
- L_3 \cos\theta_3 \\
0
\end{bmatrix}
$$

### Matriz de transformación homogénea

$$
T_{34} =
\begin{bmatrix}
\cos\theta_3 & 0 & \sin\theta_3 & -L_3\sin\theta_3 \\
\sin\theta_3 & 0 & -\cos\theta_3 & -L_3\cos\theta_3 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}
$$

## A4 → A5
### Descripción
- Rotación positiva de 90° alrededor del eje X3
- Rotación alrededor del eje Z3 con ángulo $\theta_4$
- Traslación positiva en el eje Z en $L_4$

### Matriz de rotación en X (forma general)
$$
R_x(\theta)=
\begin{bmatrix}
1 & 0 & 0 \\
0 & \cos\theta & -\sin\theta \\
0 & \sin\theta & \cos\theta
\end{bmatrix}
$$

### Matriz de rotación en Z (forma general)
$$
R_z(\theta)=
\begin{bmatrix}
\cos\theta & -\sin\theta & 0 \\
\sin\theta & \cos\theta & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

### Evaluación en $90^\circ$
$$
R_x(90^\circ)=
\begin{bmatrix}
1 & 0 & 0 \\
0 & 0 & -1 \\
0 & 1 & 0
\end{bmatrix}
$$

### Multiplicación
$$
R = R_x(90^\circ) R_z(\theta_4)
$$

$$
R =
\begin{bmatrix}
1 & 0 & 0 \\
0 & 0 & -1 \\
0 & 1 & 0
\end{bmatrix}
\begin{bmatrix}
\cos\theta_4 & -\sin\theta_4 & 0 \\
\sin\theta_4 & \cos\theta_4 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

### Resultado
$$
R =
\begin{bmatrix}
\cos\theta_4 & -\sin\theta_4 & 0 \\
0 & 0 & -1 \\
\sin\theta_4 & \cos\theta_4 & 0
\end{bmatrix}
$$

### Vector de traslación
$$
P =
\begin{bmatrix}
0 \\
0 \\
L_4
\end{bmatrix}
$$

### Matriz de transformación homogénea
$$
T_{45} =
\begin{bmatrix}
\cos\theta_4 & -\sin\theta_4 & 0 & 0 \\
0 & 0 & -1 & 0 \\
\sin\theta_4 & \cos\theta_4 & 0 & L_4 \\
0 & 0 & 0 & 1
\end{bmatrix}
$$
