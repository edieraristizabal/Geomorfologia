# Geomorfología de Movimientos en Masa

## 1. Términos Comunes
En el lenguaje común y técnico, existe una variedad de términos para describir los procesos de inestabilidad de laderas:

* **Movimiento en Masa (Mass Movement):** Es el término geomorfológico y técnico más inclusivo. Describe cualquier movimiento de suelo, detritos o roca pendiente abajo, principalmente bajo la influencia de la gravedad.
* **Deslizamiento (Landslide):** Es el término más popular y a menudo se usa como sinónimo de "movimiento en masa". Sin embargo, en la clasificación de Varnes (1978), "deslizamiento" se refiere a un tipo específico de movimiento (Slide) donde una masa se desplaza sobre una superficie de falla definida.
* **Proceso de Ladera (Slope Process):** Un término aún más amplio que incluye la reptación (creep) y la erosión superficial.
* **Derrumbe:** Término popular en español, usualmente reservado para **Caídas (Falls)**, que son movimientos extremadamente rápidos y desprendimientos de bloques.
* **Alud:** A menudo se asocia con flujos rápidos de nieve, pero también se usa para flujos de detritos (ej. alud torrencial).

---
## 2. Definiciones de Movimientos en Masa

* **Varnes (1978) - (Enfoque de Ingeniería):** "El movimiento pendiente abajo de una masa de suelo, roca o detritos... cuando el esfuerzo cortante supera la resistencia al cortante del material". Esta definición es la base de la clasificación moderna y pone el énfasis en el balance de fuerzas.
* **Scheidegger (1975) - (Enfoque Geomorfológico):** Define los movimientos en masa como parte del proceso general de denudación del paisaje. Se enfoca en el transporte de material por gravedad como un agente escultor del relieve.
* **Soeters y Van Westen (1996) - (Enfoque de Amenaza):** En el contexto de la evaluación de amenazas, los definen como el resultado de las condiciones naturales del terreno, tales como geomorfología, hidrología y geología, y las modificaciones de estas condiciones por procesos geodinámicos, vegetación, usos del suelo y actividades humanas. Dichas modificaciones activan movimientos lentos, generalmente imperceptibles debido a que las propiedades mecánicas del material o condiciones de equilibrio decrecen gradualmente, y posteriormente, factores como precipitación, sismicidad o cortes de origen antrópico detonan dichos movimientos lentos en rápidos movimientos en masa.

---
## 3. Concepto de Estabilidad de Ladera (Geotecnia)

El análisis de estabilidad cuantifica la relación entre las fuerzas que impulsan el movimiento (resistencia) y las que se resisten a él (fuerzas).

### Factor de Seguridad (FS)
Es el concepto central. Es la relación entre la resistencia al cortante disponible ($\tau_f$) y los esfuerzos cortantes ($\tau$) que actúan sobre una superficie de falla potencial.

$FS = \frac{\text{Fuerzas Resistentes}}{\text{Fuerzas Impulsoras}} = \frac{\text{Resistencia al Cortante}}{\text{Esfuerzo Cortante}}$

* **FS > 1:** La ladera es estable.
* **FS = 1:** La ladera está en equilibrio límite (falla inminente).
* **FS < 1:** La ladera es inestable y fallará.
* 
<image src=https://i.pinimg.com/736x/1c/c8/09/1cc809f613f08b9c519068007cc7c007.jpg width="500">

### Resistencia al Cortante ($\tau_f$)
Es la resistencia interna del material a fallar por cizalla. Se describe por el **Criterio de Falla de Mohr-Coulomb**:

$$\tau_f = c' + \sigma_n' \tan(\phi')$$

<image src=https://i.pinimg.com/736x/4b/5f/98/4b5f98d405de99fb3572a69482af4ae2.jpg width="500">

* **$c'$ (Cohesión Efectiva):** La "pegajosidad" o resistencia intrínseca del material, independiente del esfuerzo normal. Es alta en arcillas consolidadas o rocas cementadas.
* **$\phi'$ (Ángulo de Fricción Interna Efectivo):** Representa la fricción entre las partículas del suelo o la roca.
* **$\sigma_n'$ (Esfuerzo Normal Efectivo):** El esfuerzo que realmente mantiene unidas las partículas.

### Esfuerzo Efectivo y Presión de Poros
El concepto de esfuerzo efectivo (Terzaghi) es la clave para entender la inestabilidad.

<image src=https://i.pinimg.com/1200x/cb/29/e9/cb29e9e5ec22c439fca08d736c31a556.jpg width="500">

* **Esfuerzo Normal Total ($\sigma_n$):** El peso total (sólidos + agua) por unidad de área que actúa perpendicular a la superficie de falla.
* **Presión de Poros ($u$):** La presión del agua en los poros del suelo. Esta presión actúa "empujando" las partículas y separándolas, contrarrestando el esfuerzo normal.
* **Esfuerzo Normal Efectivo ($\sigma_n'$):** Es el esfuerzo total menos la presión de poros: $\sigma_n' = \sigma_n - u$. Este es el esfuerzo que controla la resistencia al cortante.

### ¿Por qué fallan las laderas?

* **Por Lluvia (Aumento de Presión de Poros):**
    1.  La lluvia intensa se infiltra en el suelo.
    2.  El nivel freático sube, aumentando la presión de poros ($u$).
    3.  Al aumentar $u$, el esfuerzo efectivo ($\sigma_n'$) disminuye drásticamente.
    4.  Al disminuir $\sigma_n'$, la resistencia al cortante ($\tau_f$) colapsa.
    5.  El $FS$ cae por debajo de 1.
* **Por Sismos (Aumento de Esfuerzos Cortantes):**
    1.  La aceleración sísmica introduce un nuevo **esfuerzo cortante cíclico** ($\tau_s$) en la ladera.
    2.  Este esfuerzo se suma al esfuerzo cortante gravitacional, aumentando las "Fuerzas Impulsoras".
    3.  En suelos granulares saturados, el sismo también puede causar **licuefacción**, que es un aumento súbito de la presión de poros ($u$), llevando la resistencia a cero.

---
## 4. Variables Condicionantes y Detonantes

* **Variables Condicionantes:** Son las características estáticas o de largo plazo que hacen que una ladera sea **susceptible** a fallar. Responden al "Por qué aquí".
    * *Ejemplos:* Pendiente del terreno, geología (rocas débiles, fallas), uso del suelo (deforestación), aspecto (orientación de la ladera), geometría de la ladera (curvatura).
* **Variables Detonantes (Disparadores):** Son los eventos dinámicos y de corta duración que **inician** el movimiento. Responden al "Por qué ahora".
    * *Ejemplos:* Lluvias intensas o prolongadas (el detonante más común en climas tropicales), sismos, actividad humana (cortes en la base, sobrecarga en la corona), erupciones volcánicas (sismicidad, sobrecarga de ceniza, lahares).

---
## 5. Clasificación de Cruden y Varnes (1996)
Es la clasificación más utilizada a nivel mundial. Se basa en dos criterios fundamentales:

1.  **Tipo de Material:**
    * **Roca (Rock):** Material intacto y consolidado.
    * **Detritos (Debris):** Material grueso no consolidado (suelos de grano grueso, coluvión).
    * **Tierra (Earth):** Material fino no consolidado (suelos de grano fino, arcillas, limos).
2.  **Tipo de Movimiento (Cinemática):** Se describen en la siguiente sección.
    
<image src=https://i.pinimg.com/1200x/ba/9b/80/ba9b801acae182bf28b6e2da874e6e91.jpg width="700">

| Tipo de Movimiento | Roca (Rock) | Detritos (Debris) | Tierra (Earth) |
| :--- | :--- | :--- | :--- |
| **Caída (Fall)** | Caída de Rocas | Caída de Detritos | Caída de Tierra |
| **Volcamiento (Topple)** | Volcamiento de Rocas | Volcamiento de Detritos | Volcamiento de Tierra |
| **Deslizamiento (Slide)** | Desliz. de Rocas | Desliz. de Detritos | Desliz. de Tierra |
| **Flujo (Flow)** | (Flujo de Rocas) | Flujo de Detritos | Flujo de Tierra |
| **Propagación (Spread)** | Propag. de Rocas | Propag. de Detritos | Propag. de Tierra |
| **Complejo (Complex)** | \multicolumn{3}{c|}{Combinación de los anteriores (ej. Deslizamiento-Flujo)} |

---
## 6. Tipos de Movimiento (Cinemática)

* **Caídas (Falls):** Desprendimiento de material de un talud casi vertical. El movimiento es predominantemente por el aire (caída libre, rebote, rodamiento). Son extremadamente rápidos.
    * *Geoforma resultante:* **Talud** o cono de derrubios.

  <image src=https://i.pinimg.com/736x/fb/34/a9/fb34a9b6d733bfc541554674056856c2.jpg width="500">

* **Volcamiento (Topples):** Rotación hacia adelante de una masa de roca o detritos alrededor de un punto de pivote en la base. Ocurre en macizos con discontinuidades (diaclasas, estratos) que buzan fuertemente hacia adentro de la ladera.

  <image src=https://i.pinimg.com/736x/b6/ed/50/b6ed50db91d7037d1a961480f844221c.jpg width="300">

* **Deslizamiento (Slides):** Movimiento de cizalla de una masa coherente a lo largo de una o varias superficies de ruptura definidas.
    * **Deslizamiento Rotacional:** La superficie de falla es cóncava (forma de cuchara). El movimiento rota alrededor de un eje. Típico de materiales homogéneos como suelos residuales (saprolito) o arcillas.
    * **Deslizamiento Traslacional:** La superficie de falla es plana o ligeramente ondulada. El movimiento sigue discontinuidades geológicas (estratos, fallas, diaclasas).
  
  <image src=https://i.pinimg.com/736x/6c/96/91/6c96914cf86e33fa9dd5600b111519a7.jpg width="500">

* **Flujo (Flows):** Movimiento internamente deformado, similar al de un fluido viscoso. Las partículas se mueven a diferentes velocidades dentro de la masa.
    * **Flujo de Detritos (Debris Flow):** Un flujo rápido y canalizado de una mezcla de agua y detritos. Son comunes en cuencas de alta pendiente (Quebradas) y son altamente destructivos.
    * **Flujo de Tierra (Earth Flow):** Típicos en materiales arcillosos, más lentos, a menudo con una cabecera rotacional y un lóbulo estrecho (forma de reloj de arena).
    * **Reptación (Creep):** El flujo imperceptiblemente lento del suelo. Evidenciado por árboles inclinados, postes corridos, etc.
  
  <image src= https://i.pinimg.com/1200x/62/28/3a/62283a9708b7af24606949964a493053.jpg
   width="500">

* **Propagación Lateral (Lateral Spreads):** Movimiento extensional de bloques coherentes (roca o suelo) que se deslizan sobre una capa subyacente que ha perdido su resistencia (usualmente por licuefacción sísmica).

---
## 7. Partes de un Movimiento en Masa

La morfología de un deslizamiento (especialmente rotacional) tiene partes características:

<image src=https://i.pinimg.com/1200x/ff/f7/44/fff74482762297853ff366e4cfe54e3a.jpg width="700">

* **Corona (Crown):** La superficie intacta por encima del escarpe principal.
* **Escarpe Principal (Main Scarp):** La superficie vertical o muy empinada expuesta por el desprendimiento inicial. Es la "cicatriz".
* **Escarpes Secundarios:** Pequeñas cicatrices dentro del cuerpo del deslizamiento.
* **Cabeza (Head):** La parte superior de la masa desplazada.
* **Cuerpo (Body):** La masa principal de material que se ha movido. A menudo presenta una morfología caótica o de bloques.
* **Flancos (Flanks):** Los lados del deslizamiento.
* **Superficie de Ruptura (Surface of Rupture):** La superficie sobre la cual se ha movido la masa.
* **Pie (Toe):** El lóbulo o borde más avanzado de la masa deslizada.
* **Pata (Foot):** El área donde el material se ha acumulado y sobresale de la pendiente original.

