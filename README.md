# SimulacroRedes2

### Pregunta 1

#### a) Explica brevemente el funcionamiento del Algoritmo de Dijkstra para encontrar la ruta más corta entre dos nodos en un grafo ponderado.  
El Algoritmo de Dijkstra usa vértices, con los nodos no visitados teniendo un valor infinito, y el nodo fuente teniendo un valor de 0. Luego va al nodo con distancia mínima, asignándolo como nodo actual. Sigue con este método, acumulando los valores de distancia, hasta llegar al nodo objetivo de manera óptima.

#### b) Describe el método de Enrutamiento por Inundación (Flooding) y discute sus ventajas y desventajas comparándolo con Dijkstra.  
El método por Inundación manda el paquete por todas las rutas disponibles, y escoge la más corta. Sus ventajas son que es un método simple y que siempre encuentra la ruta mas corta. La desventaja es que crea mucho tráfico en la red, y el volumen de paquetes puede crear errores.

### Pregunta 2

#### a) Para la subred 172.29.152.0 con máscara 255.255.248.0, determina la dirección de broadcast. Explica el proceso de conversión de la máscara a binario y cómo se obtiene el resultado.
Esta máscara se puede representar como /21, lo que significa que 21 de los 32 bits de la dirección simbolizan la red, y el resto se usan para asignar direcciones en la red (ej. 11111111.11111111.11111000.00000000). El valor más bajo se usa para simbolizar la red completa (10101100.00011101.10011000.00000000 o 172.29.152.0) y el más alto se usa para Broadcast (10101100.00011101.10011111.11111111 o 172.29.159.255)

#### b) Dado el bloque 172.18.26.0/23, calcula la dirección de broadcast y justifica el proceso.
Primero, se convierte a binario: 10101100.00010010.00011010.00000000. 32 - 23 = 9, hay 9 bits disponibles para la red. Se convierten los bits disponibles a 1 para encontrar el valor máximo de la red, que es el Broadcast: 10101100.00010010.00011011.11111111 o 172.18.27.255.

### Pregunta 3

#### a) Con la subred 172.30.67.192 y máscara 255.255.255.192, determina cuál es la última dirección de host válida (excluyendo la dirección de broadcast).
Convierte a binario: 10101100.00011110.01000011.11000000. Los últimos ceros son direcciones disponibles. Encuentra el segundo valor más grande: 10101100.00011110.01000011.11111110 o 172.30.67.254.

#### b) Para el host 172.22.53.199 con máscara 255.255.252.0, determina el rango de direcciones válidas (primera y última dirección de host) de la subred.
Convierte a binario: 10101100.00010110.00110101.11000111, la subred a la que pertenece este host debe tener 10 ceros disponibles: 10101100.00010110.00110100.00000000 o 172.22.52.0. La primera dirección utilizable para un host es 172.22.52.1, y la última es 10101100.00010110.00110111.11111110 o 172.22.55.254.

### Pregunta 4

#### a) Calcula el número de equipos (hosts) que pueden conectarse en la red 172.26.0.0 con máscara 255.255.255.192.
Máscara en binario: 11111111.11111111.11111111.11000000. 6 ceros disponibles. 2^6 - 2 (red y broadcast) = 62.

#### b) Dado el host 172.18.171.190/23, identifica a qué subred pertenece, explicando cómo se determina el bloque correspondiente.
Binario: 10101100.00010010.10101011.10111110. 9 ceros disponibles: 10101100.00010010.10101010.00000000 o subred 172.18.170.0/23. 

### Pregunta 5

#### Explica cómo se determina el número de subredes disponibles utilizando la fórmula: Nº de subredes = 2^s. donde s es el número de bits prestados al identificador de subred. Aplica este concepto a un escenario en el que se requieren al menos 4 subredes para segmentar una red.



### Pregunta 6

### Pregunta 7

### Pregunta 8

### Pregunta 9

### Pregunta 10

### Pregunta 11

### Pregunta 12

### Pregunta 13

### Pregunta 14

### Pregunta 15

### Pregunta 16

### Pregunta 17

### Pregunta 18

### Pregunta 19

### Pregunta 20

### Pregunta 21
