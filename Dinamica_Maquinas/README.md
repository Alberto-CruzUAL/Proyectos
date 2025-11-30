# ⚙️ Análisis Dinámico y Cinemático de Mecanismos

![Estado](https://img.shields.io/badge/Estado-Finalizado-success)
![Software](https://img.shields.io/badge/Simulación-MATLAB%20%7C%20Simulink%20%7C%20SolidWorks-blue)

Proyecto de cálculo y simulación desarrollado para la asignatura de Dinámica de Máquinas.
El objetivo es el análisis completo del movimiento, fuerzas y equilibrado de un sistema mecánico complejo bajo condiciones de operación reales.

## 🎯 Objetivo del Proyecto

Analizar el comportamiento cinemático y dinámico de un **[NOMBRE DEL MECANISMO, EJ: Mecanismo de 4 Barras / Biela-Manivela / Leva]**.

Se busca determinar:
1.  **Posición, Velocidad y Aceleración** de todos los eslabones en función del tiempo.
2.  **Fuerzas dinámicas** en los pares cinemáticos (reacciones en los apoyos).
3.  **Par motor necesario** para mantener el movimiento bajo carga externa.

## 📐 Descripción del Mecanismo

* **Grados de Libertad (GDL):** [Ej: 1 GDL].
* **Tipo de Movimiento:** [Ej: Plano General].
* **Entrada:** Motor con velocidad angular constante $\omega = [XX]$ rad/s.
* **Cargas Externas:** [Ej: Fuerza de corte en el eslabón 3 / Par resistente].

![Esquema Cinemático](https://via.placeholder.com/600x350?text=Sube+tu+Diagrama+Cinemático+Aqui)
*(Aquí debes subir una imagen del esquema vectorial o diagrama de cuerpo libre de tu mecanismo)*

## 🛠️ Metodología de Análisis

### 1. Análisis Cinemático (Vectorial)
Resolución de las ecuaciones de lazo cerrado mediante **Números Complejos** o **Método Matricial**:
* $\vec{r}_2 + \vec{r}_3 = \vec{r}_1 + \vec{r}_4$
* Derivación temporal para obtención de velocidades y aceleraciones (Coriolis y relativas).

### 2. Análisis Dinámico (Cinético)
Aplicación del **Principio de D'Alembert** o **Método de Newton-Euler**:
* Cálculo de fuerzas de inercia ($F = m \cdot a_G$).
* Planteamiento de sistemas de ecuaciones lineales para resolver las incógnitas de reacción.

### 3. Simulación Computacional
Validación de los cálculos manuales mediante software:
* **Código:** [Python / MATLAB] para iterar el movimiento de 0° a 360°.
* **Validación:** Comparación con [SolidWorks Motion / MSC Adams].

## 📊 Resultados Obtenidos

Se presentan las gráficas de evolución durante un ciclo completo:

| Velocidad del Eslabón de Salida | Par Motor Requerido |
| :---: | :---: |
| ![Grafica Velocidad](https://via.placeholder.com/400x300?text=Grafica+Omega+vs+Tiempo) | ![Grafica Torque](https://via.placeholder.com/400x300?text=Grafica+Torque+vs+Angulo) |

> **Conclusión:** Se observa que el par máximo ocurre a $\theta = [XX]^\circ$, coincidiendo con la máxima aceleración del eslabón conducido. Se propone añadir un **volante de inercia** para reducir las fluctuaciones de par en un [XX]%.

## 📄 Recursos

* **[Ver Memoria de Cálculo (PDF)](./Memoria-Calculo.pdf)**
* **[Ver Código de Simulación](./codigo/)**

---
**Autor:** [Tu Nombre]
*Ingeniería Mecánica - UAL*
