---

jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3

---

(sec-MenM)=

# Geomorfología de Movimientos en Masa

Los movimientos en masa son uno de los procesos geodinámicos más activos y peligrosos en ambientes de montaña como los Andes. Su estudio combina la geomorfología con la geotecnia para entender el comportamiento de las laderas. Muchos de estos procesos son el resultado directo de la descomposición química de la roca, proceso que detallamos en {ref}`sec-meteorizacion`.

:::{important}

**Objetivos de aprendizaje:**

* Comprender los conceptos de estabilidad de laderas y el Factor de Seguridad (FS).

* Diferenciar entre variables condicionantes y detonantes de la inestabilidad.

* Identificar los diferentes tipos de movimientos en masa según la clasificación de Cruden y Varnes (1996).

* Analizar la morfología y las partes de un movimiento en masa para su diagnóstico en campo.

:::

## 1. Términos Comunes

En el lenguaje común y técnico, existe una variedad de términos para describir los procesos de inestabilidad de laderas:

* **Movimiento en Masa (Mass Movement):** Es el término geomorfológico y técnico más inclusivo. Describe cualquier movimiento de suelo, detritos o roca pendiente abajo, principalmente bajo la influencia de la gravedad.

* **Deslizamiento (Landslide):** Es el término más popular y a menudo se usa como sinónimo de "movimiento en masa". Sin embargo, en la clasificación de {cite:t}`varnes_landslides_1978`, "deslizamiento" se refiere a un tipo específico de movimiento (Slide) donde una masa se desplaza sobre una superficie de falla definida.

* **Proceso de Ladera (Slope Process):** Un término aún más amplio que incluye la reptación (creep) y la erosión superficial.

* **Derrumbe:** Término popular en español, usualmente reservado para **Caídas (Falls)**, que son movimientos extremadamente rápidos y desprendimientos de bloques.

* **Alud:** A menudo se asocia con flujos rápidos de nieve, pero también se usa para flujos de detritos (ej. alud torrencial).

---

## 2. Definiciones de Movimientos en Masa

* **{cite:t}`varnes_landslides_1978` - (Enfoque de Ingeniería):** "El movimiento pendiente abajo de una masa de suelo, roca o detritos... cuando el esfuerzo cortante supera la resistencia al cortante del material". Esta definición es la base de la clasificación moderna y pone el énfasis en el balance de fuerzas.

* **{cite:t}`scheidegger_physical_1975` - (Enfoque Geomorfológico):** Define los movimientos en masa como parte del proceso general de denudación del paisaje. Se enfoca en el transporte de material por gravedad como un agente escultor del relieve.

* **{cite:t}`soeters_slope_1996` - (Enfoque de Amenaza):** En el contexto de la evaluación de amenazas, los definen como el resultado de las condiciones naturales del terreno, tales como geomorfología, hidrología y geología, y las modificaciones de estas condiciones por procesos geodinámicos, vegetación, usos del suelo y actividades humanas. Dichas modificaciones activan movimientos lentos, generalmente imperceptibles debido a que las propiedades mecánicas del material o condiciones de equilibrio decrecen gradualmente, y posteriormente, factores como precipitación, sismicidad o cortes de origen antrópico detonan dichos movimientos lentos en rápidos movimientos en masa.

---

## 3. Concepto de Estabilidad de Ladera (Geotecnia)

El análisis de estabilidad cuantifica la relación entre las fuerzas que impulsan el movimiento (resistencia) y las que se resisten a él (fuerzas).

### Factor de Seguridad (FS)

Es el concepto central. Es la relación entre la resistencia al cortante disponible ($\tau_f$) y los esfuerzos cortantes ($\tau$) que actúan sobre una superficie de falla potencial.

$FS = \frac{\text{Fuerzas Resistentes}}{\text{Fuerzas Impulsoras}} = \frac{\text{Resistencia al Cortante}}{\text{Esfuerzo Cortante}}$

* **FS > 1:** La ladera es estable.

* **FS = 1:** La ladera está en equilibrio límite (falla inminente).

* **FS < 1:** La ladera es inestable y fallará.

```{figure} https://i.pinimg.com/736x/1c/c8/09/1cc809f613f08b9c519068007cc7c007.jpg
:name: fig-2138
:width: 500
```

### Resistencia al Cortante ($\tau_f$)

Es la resistencia interna del material a fallar por cizalla. Se describe por el **Criterio de Falla de Mohr-Coulomb**:

$$\tau_f = c' + \sigma_n' \tan(\phi')$$

```{figure} https://i.pinimg.com/736x/4b/5f/98/4b5f98d405de99fb3572a69482af4ae2.jpg
:name: fig-2448
:width: 500
```

* **$c'$ (Cohesión Efectiva):** La "pegajosidad" o resistencia intrínseca del material, independiente del esfuerzo normal. Es alta en arcillas consolidadas o rocas cementadas.

* **$\phi'$ (Ángulo de Fricción Interna Efectivo):** Representa la fricción entre las partículas del suelo o la roca.

* **$\sigma_n'$ (Esfuerzo Normal Efectivo):** El esfuerzo que realmente mantiene unidas las partículas.

### Esfuerzo Efectivo y Presión de Poros

El concepto de esfuerzo efectivo (Terzaghi) es la clave para entender la inestabilidad.

```{figure} https://i.pinimg.com/1200x/cb/29/e9/cb29e9e5ec22c439fca08d736c31a556.jpg
:name: fig-3273
:width: 500
```

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

```{figure} https://i.pinimg.com/736x/e3/76/eb/e376eb0c202f698226d54e70fa059895.jpg
:name: fig-margen-estabilidad
:width: 600

Evolución del margen de estabilidad de una ladera en el tiempo: los factores predisponentes y preparatorios reducen progresivamente el margen de estabilidad, hasta que un detonante produce un pico de esfuerzo que supera el umbral de inestabilidad (Steger, 2017).
```

---

## 5. Clasificación de Cruden y Varnes (1996)

Es la clasificación más utilizada a nivel mundial {cite:p}`cruden_landslide_1996`. Se basa en dos criterios fundamentales:

1.  **Tipo de Material:**

    * **Roca (Rock):** Material intacto y consolidado.

    * **Detritos (Debris):** Material grueso no consolidado (suelos de grano grueso, coluvión).

    * **Tierra (Earth):** Material fino no consolidado (suelos de grano fino, arcillas, limos).

2.  **Tipo de Movimiento (Cinemática):** Se describen en la siguiente sección.

    

```{figure} https://i.pinimg.com/1200x/ba/9b/80/ba9b801acae182bf28b6e2da874e6e91.jpg
:name: fig-322
:width: 700
```

| Tipo de Movimiento | Roca (Rock) | Detritos (Debris) | Tierra (Earth) |
| :--- | :--- | :--- | :--- |
| **Caída (Fall)** | Caída de Rocas | Caída de Detritos | Caída de Tierra |
| **Volcamiento (Topple)** | Volcamiento de Rocas | Volcamiento de Detritos | Volcamiento de Tierra |
| **Deslizamiento (Slide)** | Desliz. de Rocas | Desliz. de Detritos | Desliz. de Tierra |
| **Flujo (Flow)** | (Flujo de Rocas) | Flujo de Detritos | Flujo de Tierra |
| **Propagación (Spread)** | Propag. de Rocas | Propag. de Detritos | Propag. de Tierra |
| **Complejo (Complex)** | Combinación de los anteriores (ej. Deslizamiento-Flujo) | - | - |

---

## 6. Tipos de Movimiento (Cinemática)

* **Caídas (Falls):** Desprendimiento de material de un talud casi vertical. El movimiento es predominantemente por el aire (caída libre, rebote, rodamiento). Son extremadamente rápidos.

    * *Geoforma resultante:* **Talud** o cono de derrubios.

  

```{figure} https://i.pinimg.com/736x/fb/34/a9/fb34a9b6d733bfc541554674056856c2.jpg
:name: fig-6591
:width: 500
```

* **Volcamiento (Topples):** Rotación hacia adelante de una masa de roca o detritos alrededor de un punto de pivote en la base. Ocurre en macizos con discontinuidades (diaclasas, estratos) que buzan fuertemente hacia adentro de la ladera.

  

```{figure} https://i.pinimg.com/736x/b6/ed/50/b6ed50db91d7037d1a961480f844221c.jpg
:name: fig-2016
:width: 300
```

* **Deslizamiento (Slides):** Movimiento de cizalla de una masa coherente a lo largo de una o varias superficies de ruptura definidas.

    * **Deslizamiento Rotacional:** La superficie de falla es cóncava (forma de cuchara). El movimiento rota alrededor de un eje. Típico de materiales homogéneos como suelos residuales (saprolito) o arcillas.

    * **Deslizamiento Traslacional:** La superficie de falla es plana o ligeramente ondulada. El movimiento sigue discontinuidades geológicas (estratos, fallas, diaclasas).

  

  

```{figure} https://i.pinimg.com/736x/6c/96/91/6c96914cf86e33fa9dd5600b111519a7.jpg
:name: fig-7342
:width: 500
```

* **Flujo (Flows):** Movimiento internamente deformado, similar al de un fluido viscoso. Las partículas se mueven a diferentes velocidades dentro de la masa.

    * **Flujo de Detritos (Debris Flow):** Un flujo rápido y canalizado de una mezcla de agua y detritos. Son comunes en cuencas de alta pendiente (Quebradas) y son altamente destructivos.

    * **Flujo de Tierra (Earth Flow):** Típicos en materiales arcillosos, más lentos, a menudo con una cabecera rotacional y un lóbulo estrecho (forma de reloj de arena).

    * **Reptación (Creep):** El flujo imperceptiblemente lento del suelo. Evidenciado por árboles inclinados, postes corridos, etc.

  

  
```{figure} https://i.pinimg.com/1200x/62/28/3a/62283a9708b7af24606949964a493053.jpg
:width: 500
```

* **Propagación Lateral (Lateral Spreads):** Movimiento extensional de bloques coherentes (roca o suelo) que se deslizan sobre una capa subyacente que ha perdido su resistencia (usualmente por licuefacción sísmica).

---

## 7. Partes de un Movimiento en Masa

La morfología de un deslizamiento (especialmente rotacional) tiene partes características {cite:p}`cruden_landslide_1996`:

```{figure} https://i.pinimg.com/1200x/ff/f7/44/fff74482762297853ff366e4cfe54e3a.jpg
:name: fig-2642
:width: 700
```

* **Corona (Crown):** La superficie intacta por encima del escarpe principal.

* **Escarpe Principal (Main Scarp):** La superficie vertical o muy empinada expuesta por el desprendimiento inicial. Es la "cicatriz".

* **Escarpes Secundarios:** Pequeñas cicatrices dentro del cuerpo del deslizamiento.

* **Cabeza (Head):** La parte superior de la masa desplazada.

* **Cuerpo (Body):** La masa principal de material que se ha movido. A menudo presenta una morfología caótica o de bloques.

* **Flancos (Flanks):** Los lados del deslizamiento.

* **Superficie de Ruptura (Surface of Rupture):** La superficie sobre la cual se ha movido la masa.

* **Pie (Toe):** El lóbulo o borde más avanzado de la masa deslizada.

* **Pata (Foot):** El área donde el material se ha acumulado y sobresale de la pendiente original.

---

## Interactividad: Cálculo del Factor de Seguridad (FS)

Como ingenieros, es fundamental cuantificar la estabilidad de una ladera. El **Factor de Seguridad (FS)** se define como la relación entre las fuerzas resistentes y las fuerzas motoras. 

$$FS = \frac{c' + (\sigma - u) \tan \phi'}{\tau}$$

A continuación, puede utilizar esta celda interactiva para explorar cómo cambian la cohesión, el ángulo de fricción y la presión de poros en la estabilidad de un suelo:

```{code-cell} ipython3

import numpy as np

def calcular_fs(cohesion, friccion_deg, sigma, u, tau):

    friccion_rad = np.radians(friccion_deg)

    resistencia = cohesion + (sigma - u) * np.tan(friccion_rad)

    fs = resistencia / tau

    return fs

# Parámetros típicos de una ladera en los Andes

c = 15    # Cohesión (kPa)

phi = 25  # Ángulo de fricción interna (grados)

sigma = 100 # Esfuerzo normal (kPa)

tau = 45  # Esfuerzo cortante motor (kPa)

u = 10    # Presión de poros (kPa) - Aumenta con la lluvia

fs_actual = calcular_fs(c, phi, sigma, u, tau)

print(f"El Factor de Seguridad actual es: {fs_actual:.2f}")

if fs_actual > 1:

    print("La ladera es ESTABLE (FS > 1)")

else:

    print("La ladera es INESTABLE (FS <= 1) - ¡Peligro de deslizamiento!")

```

---

## Movimientos en Masa en Colombia: Desafíos Territoriales

Debido a su topografía abrupta, geología compleja y alta pluviosidad, Colombia es uno de los países más afectados por movimientos en masa en América Latina {cite:p}`aristizabal_avenidas_2020`.

* **Ejemplos Históricos:** Eventos devastadores como el de **Armero** (1985, detonado por erupción pero con gran componente de flujo de detritos) y el de **Mocoa** (2017, flujo de detritos torrencial) marcan la historia del país.

* **Deslizamientos Urbanos:** En ciudades como **Medellín**, **Bucaramanga** y **Manizales**, la expansión urbana sobre laderas empinadas y suelos residuales genera un riesgo constante.

* **Detonantes Comunes:** La lluvia es el principal detonante en Colombia (Fenómeno de La Niña), aunque sismos como el de **Páez (1994)** han generado miles de movimientos en masa simultáneos.

---

## 8. Laderas como Sistemas de Transporte: de la Reptación al Deslizamiento

Los movimientos en masa catastróficos descritos en las secciones anteriores son la expresión más visible y peligrosa de un espectro continuo de procesos de transporte de sedimento en laderas. En el extremo opuesto de ese espectro se encuentra la **reptación** (*creep*), el movimiento lento e imperceptible del regolito pendiente abajo, causado por procesos de expansión-contracción cíclicos (humedecimiento-secado, congelamiento-deshielo, actividad biológica de raíces y organismos excavadores) {cite:p}`bierman_key_2013`.

Para laderas dominadas por reptación, donde el transporte de sedimento es aproximadamente proporcional al gradiente topográfico, la geomorfología cuantitativa emplea el modelo de **difusión lineal** ya introducido en {ref}`sec-conceptos` ($q_s=kS$). Sin embargo, las observaciones de campo muestran que, a medida que la pendiente de una ladera se aproxima a un valor crítico o "ángulo límite" ($S_c$), la tasa de transporte de sedimento no crece linealmente sino que tiende asintóticamente al infinito. Esto llevó al desarrollo del modelo de **difusión no lineal** {cite:p}`bierman_key_2013`:

$$q_s=\frac{kS}{1-(S/S_c)^2}$$

Este modelo explica, en un mismo marco matemático, tanto el comportamiento suave y difusivo de laderas de baja pendiente (donde $S \ll S_c$ y el modelo se reduce a la difusión lineal) como el comportamiento catastrófico de laderas empinadas que se aproximan a su ángulo crítico de estabilidad: al acercarse $S$ a $S_c$, pequeños incrementos adicionales de pendiente (por ejemplo, por socavación basal de un río o un corte antrópico) provocan aumentos desproporcionados en la tasa de transporte de sedimento, lo cual es consistente con el concepto de **umbral geomorfológico** discutido en {ref}`sec-conceptos` y con la mecánica de rotura por Factor de Seguridad descrita arriba: el ángulo crítico $S_c$ del modelo de difusión no lineal es, en esencia, el correlato morfológico del ángulo de fricción efectivo ($\phi'$) del criterio de Mohr-Coulomb {cite:p}`bierman_key_2013`.

## 9. Tiempo de Residencia del Sedimento en la Ladera

Otro concepto cuantitativo útil es el **tiempo de residencia del sedimento** (*sediment residence time*): el periodo promedio durante el cual una partícula de suelo permanece almacenada en una posición de la ladera antes de ser movilizada definitivamente hacia el sistema fluvial {cite:p}`bierman_key_2013`. Este tiempo varía en órdenes de magnitud según el proceso dominante:

| Posición / Proceso en la Ladera | Tiempo de Residencia Típico del Sedimento |
| :--- | :--- |
| Regolito superficial en reptación lenta | 10² – 10⁴ años |
| Depósito coluvial en la base de una ladera estable | 10³ – 10⁵ años |
| Material removilizado por un deslizamiento traslacional | Minutos a horas (removilización súbita) |
| Depósito de un flujo de detritos en un cono aluvial (ver {ref}`sec-torrencial`) | 10¹ – 10³ años (hasta el próximo evento o incisión) |

*Órdenes de magnitud de referencia según {cite:t}`bierman_key_2013`; varían fuertemente con el clima, la litología y la actividad sísmica local.*

Este concepto es relevante para la gestión del riesgo: un depósito coluvial que ha permanecido "almacenado" en una ladera durante miles de años sin movimiento no es intrínsecamente estable de forma permanente, sino que se encuentra en un estado de **equilibrio metaestable**, susceptible de ser removilizado abruptamente si un detonante (lluvia extrema, sismo, corte antrópico) reduce su Factor de Seguridad por debajo de 1, como se describió en la Sección 3.

---

## 10. Geoinformática y Teledetección para el Monitoreo de Movimientos en Masa

La caracterización de un movimiento en masa individual (Secciones 5 a 7) se ha visto transformada en las últimas décadas por el desarrollo de las **tecnologías de geoinformación**: sensores remotos, sistemas de información geográfica (SIG) y técnicas de procesamiento digital que permiten detectar, mapear y monitorear la inestabilidad de laderas a escalas que van desde un talud individual hasta regiones enteras {cite:p}`pirasteh_global_2017`.

| Tecnología | Qué Permite Medir/Detectar | Aplicación en Movimientos en Masa |
| :--- | :--- | :--- |
| Interferometría de Radar de Apertura Sintética (InSAR) | Desplazamientos milimétricos de la superficie del terreno entre pasadas satelitales | Detección de movimientos lentos (reptación acelerada, deslizamientos activos de baja velocidad) previos a una falla catastrófica |
| LiDAR (Laser Imaging Detection and Ranging), aéreo o terrestre | Modelos digitales de elevación (DEM) de muy alta resolución, capaces de "ver" a través de la cobertura vegetal | Identificación de cicatrices de deslizamientos antiguos ocultos por bosque; cálculo preciso de volúmenes movilizados |
| Fotogrametría con Drones (UAV) | Ortomosaicos y modelos 3D de alta resolución de un evento reciente | Monitoreo repetido de la evolución de un deslizamiento activo; cálculo de volúmenes de erosión/depósito |
| Sensores Ópticos Multiespectrales (satelitales) | Cambios en la cobertura del suelo y la vegetación a escala regional | Inventarios multitemporales de movimientos en masa tras un evento sísmico o una temporada de lluvias extrema |

*Compilado a partir de {cite:t}`pirasteh_global_2017`.*

Estas tecnologías son particularmente valiosas para superar dos limitaciones históricas de los inventarios de movimientos en masa en países como Colombia: la dificultad de acceso a zonas de alta montaña con topografía abrupta y cobertura vegetal densa, y la necesidad de generar inventarios multitemporales (antes/después de un evento detonante) para calibrar modelos de amenaza a escala regional {cite:p}`pirasteh_global_2017,aristizabal_avenidas_2020`. La integración de estas fuentes de datos dentro de un SIG permite, además, combinar las variables condicionantes (Sección 4) en modelos estadísticos o de aprendizaje automático de susceptibilidad a movimientos en masa, una aproximación cada vez más estándar en la gestión del riesgo geomorfológico.

---

## Taller de Autoevaluación

1. **Mecánica de Suelos:** Explique cómo el aumento de la presión de poros ($u$) durante una temporada de lluvias reduce el Factor de Seguridad de una ladera.

2. **Condicionantes vs Detonantes:** Clasifique las siguientes variables: pendiente del terreno, sismo de magnitud 7.0, deforestación, lluvia de 100 mm en 24h, presencia de una falla geológica.

3. **Cinemática:** ¿Cuál es la diferencia principal entre un deslizamiento rotacional y uno traslacional? ¿En qué tipo de material es más común cada uno?

4. **Identificación de Campo:** Si observa un arco de escarpe fresco en la parte alta de una ladera y un abultamiento o lóbulo en la base, ¿qué partes de un movimiento en masa está identificando?

5. **Riesgo en Colombia:** ¿Por qué se dice que el Valle de Aburrá (Medellín) es una de las zonas con mayor susceptibilidad a movimientos en masa en el país?

