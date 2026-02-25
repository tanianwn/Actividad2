# Actividad2

## A1 → A2

### Descripción
- Rotación positiva de 90° alrededor del eje Y
- Traslación positiva en el eje Z una distancia L0

### Matriz de rotación en Y (forma general)

Ry(θ) =
[ cosθ   0   sinθ
  0      1   0
 -sinθ   0   cosθ ]

### Matriz de rotación en Z (forma general)

Rz(θ) =
[ cosθ  -sinθ   0
  sinθ   cosθ   0
  0      0      1 ]

### Multiplicación

R = Ry(90°) Rz(θ)

### Resultado

R =
[ 0        0        1
  sinθ     cosθ     0
 -cosθ     sinθ     0 ]

### Vector de traslación

P =
[ 0
  0
  L0 ]

### Matriz homogénea

T12 =
[ 0        0        1      0
  sinθ     cosθ     0      0
 -cosθ     sinθ     0      L0
  0        0        0      1 ]

---

## A2 → A3

### Descripción
- Rotación alrededor del eje Z1 con ángulo θ2
- Traslación positiva de L2 sobre el eje Z1

### Matriz de rotación

R23 =
[ cosθ2  -sinθ2   0
  sinθ2   cosθ2   0
  0       0       1 ]

### Vector de traslación

P =
[ -L2 cosθ2
  -L2 sinθ2
   0 ]

### Matriz homogénea

T23 =
[ cosθ2  -sinθ2   0   -L2 cosθ2
  sinθ2   cosθ2   0   -L2 sinθ2
  0       0       1    0
  0       0       0    1 ]

---

## A3 → A4

### Descripción
- Rotación alrededor del eje Z2 con ángulo θ3
- Rotación positiva de 90° alrededor del eje X2
- Traslación negativa en XY en L3

### Matriz de rotación resultante

R =
[ cosθ3   0   sinθ3
  sinθ3   0  -cosθ3
  0       1   0 ]

### Vector de traslación

P =
[ -L3 sinθ3
  -L3 cosθ3
   0 ]

### Matriz homogénea

T34 =
[ cosθ3   0   sinθ3   -L3 sinθ3
  sinθ3   0  -cosθ3   -L3 cosθ3
  0       1   0        0
  0       0   0        1 ]
