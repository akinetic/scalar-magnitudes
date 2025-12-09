# Magnitudes Escalares

> **Las Magnitudes Escalares son magnitudes escalares invariantes que conservan su valor y forma bajo transformaciones de traslación y rotación, o cambios entre sistemas de coordenadas (Cartesianas, polares, esféricas, etc.).**

---

## I. Definiciones

### Magnitudes Vectoriales

La **posición vectorial** ($\vec{r}\_{ij}$), la **velocidad vectorial** ($\vec{v}\_{ij}$), y la **aceleración vectorial** ($\vec{a}\_{ij}$) de dos partículas $i$ y $j$ están dadas por:

| Magnitud Vectorial | Definición | Derivación |
| :--- | :--- | :--- |
| **Posición** ($\vec{r}\_{ij}$) | $\vec{r}\_{ij} = (\vec{r}\_i - \vec{r}\_j)$ | *(Definición fundamental)* |
| **Velocidad** ($\vec{v}\_{ij}$) | $\vec{v}\_{ij} = (\vec{v}\_i - \vec{v}\_j)$ | $\vec{v}\_{ij} = \frac{d(\vec{r}\_{ij})}{dt}$ |
| **Aceleración** ($\vec{a}\_{ij}$) | $\vec{a}\_{ij} = (\vec{a}\_i - \vec{a}\_j)$ | $\vec{a}\_{ij} = \frac{d^2(\vec{r}\_{ij})}{dt^2}$ |

### Magnitudes Escalares

La **posición escalar** ($\tau\_{ij}$), la **velocidad escalar** ($\dot{\tau}\_{ij}$), y la **aceleración escalar** ($\ddot{\tau}\_{ij}$) de dos partículas $i$ y $j$ están dadas por:

| Magnitud Escalar | Definición | Derivación |
| :--- | :--- | :--- |
| **Posición** ($\tau\_{ij}$) | $\tau\_{ij} = \frac{1}{2} \vec{r}\_{ij} \cdot \vec{r}\_{ij}$ | *(Definición fundamental)* |
| **Velocidad** ($\dot{\tau}\_{ij}$) | $\dot{\tau}\_{ij} = \vec{v}\_{ij} \cdot \vec{r}\_{ij}$ | $\dot{\tau}\_{ij} = \frac{d(\tau\_{ij})}{dt}$ |
| **Aceleración** ($\ddot{\tau}\_{ij}$) | $\ddot{\tau}\_{ij} = \vec{a}\_{ij} \cdot \vec{r}\_{ij} + \vec{v}\_{ij} \cdot \vec{v}\_{ij}$ | $\ddot{\tau}\_{ij} = \frac{d^2(\tau\_{ij})}{dt^2}$ |

---

## II. Demostraciones de Invarianza Escalar

### 0. Transformaciones Vectoriales (Absolutas)

La posición vectorial ($\vec{r}'\_i$), la velocidad vectorial ($\vec{v}'\_i$) y la aceleración vectorial ($\vec{a}'\_i$) de una partícula $i$ con respecto a un Sistema de Referencia $S'$, cuyo origen $O'$ está en la posición vectorial $\vec{r}\_{O'}$ con respecto a otro Sistema de Referencia $S$, están dadas por:

$\vec{r}'\_i = \vec{r}\_i - \vec{r}\_{O'}$

$\vec{v}'\_i = \vec{v}\_i - \vec{v}\_{O'} - \vec{\omega} \times (\vec{r}\_i - \vec{r}\_{O'})$

$\vec{a}'\_i = \vec{a}\_i - \vec{a}\_{O'} - 2 \vec{\omega} \times (\vec{v}\_i - \vec{v}\_{O'}) + \vec{\omega} \times (\vec{\omega} \times (\vec{r}\_i - \vec{r}\_{O'})) - \vec{\alpha} \times (\vec{r}\_i - \vec{r}\_{O'})$

Donde $\vec{r}\_i$, $\vec{v}\_i$, y $\vec{a}\_i$ son la posición, velocidad y aceleración vectoriales de la partícula $i$ con respecto al Sistema $S$; y $\vec{\omega}$ y $\vec{\alpha}$ son la velocidad angular y la aceleración angular del Sistema $S'$ con respecto al Sistema $S$.

**Nota**

Si $\vec{m}'\_i = \vec{n}\_i$ entonces:

$\dfrac{d(\vec{m}'\_i)}{dt} = \dfrac{d(\vec{n}\_i)}{dt} - \vec{\omega} \times \vec{n}\_i$

---

### 1. Invarianza de la Posición Escalar ($\tau\_{ij}$)

La Posición Escalar $\tau\_{ij}$ es invariante bajo rotación y traslación porque la magnitud del vector relativo se preserva.

$\tau\_{ij} = \frac{1}{2} (\vec{r}\_i - \vec{r}\_j) \cdot (\vec{r}\_i - \vec{r}\_j)$

$\tau'\_{ij} = \frac{1}{2} (\vec{r}'\_i - \vec{r}'\_j) \cdot (\vec{r}'\_i - \vec{r}'\_j)$

$\text{Dado que } (\vec{r}\_i - \vec{r}\_j) = (\vec{r}'\_i - \vec{r}'\_j)$

$\text{Porque } \vec{r}'\_i = \vec{r}\_i - \vec{r}\_{O'} \text{ y } \vec{r}'\_j = \vec{r}\_j - \vec{r}\_{O'} \text{ (El vector de posición relativa es independiente del origen del Sistema.)}$

$\tau'\_{ij} = \frac{1}{2} (\vec{r}\_i - \vec{r}\_j) \cdot (\vec{r}\_i - \vec{r}\_j)$

$\therefore \tau'\_{ij} = \tau\_{ij}$

---

### 2. Invarianza de la Velocidad Escalar ($\dot{\tau}\_{ij}$)

La Velocidad Escalar $\dot{\tau}\_{ij}$ es invariante porque el producto cruz generado por la velocidad angular ($\vec{\omega}$) es perpendicular al vector de posición relativa, resultando en un producto escalar cero.

$\dot{\tau}\_{ij} = (\vec{v}\_i - \vec{v}\_j) \cdot (\vec{r}\_i - \vec{r}\_j)$

$\dot{\tau}'\_{ij} = (\vec{v}'\_i - \vec{v}'\_j) \cdot (\vec{r}'\_i - \vec{r}'\_j)$

$\dot{\tau}'\_{ij} = \left( (\vec{v}\_i - \vec{v}\_j) - \vec{\omega} \times (\vec{r}\_i - \vec{r}\_j) \right) \cdot (\vec{r}\_i - \vec{r}\_j)$

$\text{Dado que } (- \vec{\omega} \times (\vec{r}\_i - \vec{r}\_j)) \cdot (\vec{r}\_i - \vec{r}\_j) = 0 \text{ (El término rotacional es ortogonal al vector de posición relativa.)}$

$\text{Porque } (\vec{A} \times \vec{B}) \cdot \vec{B} = 0 \text{ (Propiedad del Triple Producto Escalar)}$

$\dot{\tau}'\_{ij} = (\vec{v}\_i - \vec{v}\_j) \cdot (\vec{r}\_i - \vec{r}\_j)$

$\therefore \dot{\tau}'\_{ij} = \dot{\tau}\_{ij}$

---

### 3. Invarianza de la Aceleración Escalar ($\ddot{\tau}\_{ij}$)

La Aceleración Escalar $\ddot{\tau}\_{ij}$ es invariante porque todos los términos inerciales (Aceleración Angular, Coriolis y Centrífuga) se anulan mutuamente debido a las propiedades de los productos vectoriales y escalares.

$\ddot{\tau}\_{ij} = (\vec{a}\_i - \vec{a}\_j) \cdot (\vec{r}\_i - \vec{r}\_j) + (\vec{v}\_i - \vec{v}\_j) \cdot (\vec{v}\_i - \vec{v}\_j)$

$\ddot{\tau}'\_{ij} = (\vec{a}'\_i - \vec{a}'\_j) \cdot (\vec{r}'\_i - \vec{r}'\_j) + (\vec{v}'\_i - \vec{v}'\_j) \cdot (\vec{v}'\_i - \vec{v}'\_j)$

$\ddot{\tau}'\_{ij} = \left[ (\vec{a}\_i - \vec{a}\_j) - 2 \vec{\omega} \times (\vec{v}\_i - \vec{v}\_j) + \vec{\omega} \times (\vec{\omega} \times (\vec{r}\_i - \vec{r}\_j)) - \vec{\alpha} \times (\vec{r}\_i - \vec{r}\_j) \right] \cdot (\vec{r}\_i - \vec{r}\_j) + \left[ (\vec{v}\_i - \vec{v}\_j) - \vec{\omega} \times (\vec{r}\_i - \vec{r}\_j) \right] \cdot \left[ (\vec{v}\_i - \vec{v}\_j) - \vec{\omega} \times (\vec{r}\_i - \vec{r}\_j) \right]$

$\text{Dado que } - (\vec{\alpha} \times (\vec{r}\_i - \vec{r}\_j)) \cdot (\vec{r}\_i - \vec{r}\_j) = 0 \text{ (El término de aceleración angular se anula)}$

$\text{Porque } (\vec{A} \times \vec{B}) \cdot \vec{B} = 0 \text{ (Propiedad del Triple Producto Escalar)}$

$\text{Dado que } - 2 (\vec{\omega} \times (\vec{v}\_i - \vec{v}\_j)) \cdot (\vec{r}\_i - \vec{r}\_j) - 2 (\vec{v}\_i - \vec{v}\_j) \cdot (\vec{\omega} \times (\vec{r}\_i - \vec{r}\_j)) = 0 \text{ (Los términos de Coriolis se anulan)}$

$\text{Porque } (\vec{A} \times \vec{B}) \cdot \vec{C} = \vec{A} \cdot (\vec{B} \times \vec{C}) \text{ (Propiedad de Permutación Cíclica del Triple Producto Escalar)}$

$\text{Dado que } + (\vec{\omega} \times (\vec{\omega} \times (\vec{r}\_i - \vec{r}\_j))) \cdot (\vec{r}\_i - \vec{r}\_j) + (\vec{\omega} \times (\vec{r}\_i - \vec{r}\_j)) \cdot (\vec{\omega} \times (\vec{r}\_i - \vec{r}\_j)) = 0 \text{ (Los términos centrífugos se anulan)}$

$\text{Dado que } + \vec{P} \cdot (\vec{r}\_i - \vec{r}\_j) + E = 0$

$\text{Porque } \vec{P} = \vec{A} \times (\vec{B} \times \vec{C}) = (\vec{A} \cdot \vec{C}) \ \vec{B} - (\vec{A} \cdot \vec{B}) \ \vec{C} \text{ (Triple Producto Vectorial)}$

$\text{Porque } E = (\vec{A} \times \vec{B}) \cdot (\vec{A} \times \vec{B}) = (\vec{A} \cdot \vec{A}) \ (\vec{B} \cdot \vec{B}) - (\vec{A} \cdot \vec{B})^2 \text{ (Identidad de Lagrange)}$

$\ddot{\tau}'\_{ij} = (\vec{a}\_i - \vec{a}\_j) \cdot (\vec{r}\_i - \vec{r}\_j) + (\vec{v}\_i - \vec{v}\_j) \cdot (\vec{v}\_i - \vec{v}\_j)$

$\therefore \ddot{\tau}'\_{ij} = \ddot{\tau}\_{ij}$

---

## III. Relaciones Fundamentales

### Relaciones de Magnitudes Radiales

Las magnitudes escalares ($\tau\_{ij}, \dot{\tau}\_{ij}, \ddot{\tau}\_{ij}$) expresadas usando **magnitudes radiales** ($r\_{ij}$) están dadas por:

| Magnitud Escalar | Relación con Magnitudes Radiales |
| :--- | :--- |
| $\tau\_{ij}$ | $\tau\_{ij} = \frac{1}{2} r\_{ij}^2$ |
| $\dot{\tau}\_{ij}$ | $\dot{\tau}\_{ij} = r\_{ij} \dot{r}\_{ij}$ |
| $\ddot{\tau}\_{ij}$ | $\ddot{\tau}\_{ij} = r\_{ij} \ddot{r}\_{ij} + \dot{r}\_{ij}^2$ |

### Relaciones de Magnitudes Polares

Las magnitudes escalares ($\tau\_{ij}, \dot{\tau}\_{ij}, \ddot{\tau}\_{ij}$) expresadas usando **magnitudes polares** ($r\_{ij}$) están dadas por:

| Magnitud Escalar | Relación con Magnitudes Polares |
| :--- | :--- |
| $\tau\_{ij}$ | $\tau\_{ij} = \frac{1}{2} r\_{ij}^2$ |
| $\dot{\tau}\_{ij}$ | $\dot{\tau}\_{ij} = r\_{ij} \dot{r}\_{ij}$ |
| $\ddot{\tau}\_{ij}$ | $\ddot{\tau}\_{ij} = r\_{ij} \ddot{r}\_{ij} + \dot{r}\_{ij}^2$ |

### Relaciones de Magnitudes Cilíndricas

Las magnitudes escalares ($\tau\_{ij}, \dot{\tau}\_{ij}, \ddot{\tau}\_{ij}$) expresadas usando **magnitudes cilíndricas** ($r\_{ij}$) están dadas por:

| Magnitud Escalar | Relación con Magnitudes Cilíndricas |
| :--- | :--- |
| $\tau\_{ij}$ | $\tau\_{ij} = \frac{1}{2} r\_{ij}^2$ |
| $\dot{\tau}\_{ij}$ | $\dot{\tau}\_{ij} = r\_{ij} \dot{r}\_{ij}$ |
| $\ddot{\tau}\_{ij}$ | $\ddot{\tau}\_{ij} = r\_{ij} \ddot{r}\_{ij} + \dot{r}\_{ij}^2$ |

### Relaciones de Magnitudes Circulares

Las magnitudes escalares ($\tau\_{ij}, \dot{\tau}\_{ij}, \ddot{\tau}\_{ij}$) expresadas usando **magnitudes circulares** ($r\_{ij}$) están dadas por:

| Magnitud Escalar | Relación con Magnitudes Circulares |
| :--- | :--- |
| $\tau\_{ij}$ | $\tau\_{ij} = \frac{1}{2} r\_{ij}^2$ |
| $\dot{\tau}\_{ij}$ | $\dot{\tau}\_{ij} = r\_{ij} \dot{r}\_{ij}$ |
| $\ddot{\tau}\_{ij}$ | $\ddot{\tau}\_{ij} = r\_{ij} \ddot{r}\_{ij} + \dot{r}\_{ij}^2$ |

### Relaciones de Magnitudes Esféricas

Las magnitudes escalares ($\tau\_{ij}, \dot{\tau}\_{ij}, \ddot{\tau}\_{ij}$) expresadas usando **magnitudes esféricas** ($r\_{ij}$) están dadas por:

| Magnitud Escalar | Relación con Magnitudes Esféricas |
| :--- | :--- |
| $\tau\_{ij}$ | $\tau\_{ij} = \frac{1}{2} r\_{ij}^2$ |
| $\dot{\tau}\_{ij}$ | $\dot{\tau}\_{ij} = r\_{ij} \dot{r}\_{ij}$ |
| $\ddot{\tau}\_{ij}$ | $\ddot{\tau}\_{ij} = r\_{ij} \ddot{r}\_{ij} + \dot{r}\_{ij}^2$ |

---

## IV. Bibliografía

1. A. Torassa, *Una Terna de Ecuaciones Invariantes* (2014). [PDF](https://atorassa.github.io/physics-authors/torassa/spanish/pdf/34.pdf)
2. A. Torassa, *Una Reformulación de la Mecánica Clásica* (2014). [PDF](https://atorassa.github.io/physics-authors/torassa/spanish/pdf/45.pdf)
3. A. Tobla, *Magnitudes Lineales, Radiales & Escalares* (2015). [PDF](https://atorassa.github.io/physics-authors/tobla/spanish/pdf/01.pdf)
4. A. Tobla, *Una Reformulación de la Mecánica Clásica* (2024). [PDF](https://atorassa.github.io/physics-authors/tobla/spanish/pdf/02.pdf)
