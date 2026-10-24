(sec-cuencas)=
# Geomorfología de Cuencas Hidrográficas

Este documento explora la cuenca hidrográfica como la unidad fundamental del paisaje, analizando su estructura, los procesos hidrológicos que la gobiernan y cómo su morfología controla la respuesta en caudales.

:::{important}
**Objetivos de aprendizaje:**
* Definir la cuenca hidrográfica y sus divisorias de aguas como la unidad de gestión del territorio.
* Jerarquizar la red de drenaje mediante el método de Strahler.
* Diferenciar los procesos de erosión, transporte y deposición en las diferentes partes de la cuenca.
* Analizar el impacto de la urbanización en la respuesta hidrológica (hidrogramas) y el riesgo de inundación.
:::

---
## 1. ¿Qué es una Cuenca Hidrográfica?
Una **cuenca hidrográfica** es la unidad geomorfológica fundamental. Se define como la superficie total de terreno que drena el agua de la precipitación hacia un punto común de salida (llamado *outlet*), que puede ser un río, un lago o el mar.

```{figure} https://i.pinimg.com/736x/48/a7/4b/48a74b7df6e5629486c66003d392e9b8.jpg
:name: fig-2982
:width: 200
```

El límite de la cuenca está definido por la **divisoria de aguas** (o *watershed divide*), una línea imaginaria que sigue las cimas y crestas topográficas y separa los flujos de agua que van en direcciones opuestas.

```{figure} https://i.pinimg.com/736x/e1/5d/da/e15dda02972d286bebc4ad290c87cb61.jpg
:name: fig-341
:width: 400
```

---
## 2. Partes de una Cuenca
Una cuenca se zonifica longitudinalmente en tres partes, cada una dominada por diferentes procesos:

* **Cuenca Alta (Recepción):** Es la cabecera.
    * **Características:** Pendientes fuertes, valles en "V" estrechos.
    * **Procesos:** Alta energía. Domina la **erosión** y los movimientos en masa. Producción de sedimentos.
* **Cuenca Media (Transferencia):**
    * **Características:** Pendientes moderadas, el valle se ensancha.
    * **Procesos:** Equilibrio entre erosión y deposición. Domina el **transporte** de sedimentos. Aparecen las primeras llanuras de inundación.
* **Cuenca Baja (Deposición):**
    * **Características:** Pendientes muy bajas, valles amplios, ríos meándricos, llanuras de inundación extensas.
    * **Procesos:** Baja energía. Domina la **deposición** de sedimentos. Formación de deltas en la desembocadura.

```{figure} https://i.pinimg.com/1200x/09/2d/76/092d76f16db55d44623e185d459c9396.jpg
:name: fig-1370
:width: 600
```

```{figure} https://i.pinimg.com/736x/8a/dd/67/8add6778eb2beae51c8ad0e88a1c10ae.jpg
:name: fig-786
:width: 600
```

---
## 3. Órdenes de Drenaje (Strahler)
Es un método para clasificar la jerarquía de la red de drenaje, lo cual es un indicador de la complejidad y el tamaño de la cuenca. El método más común es el de {cite:t}`strahler_quantitative_1957`:

* **Orden 1:** Canales de cabecera que no tienen ningún tributario.
* **Orden 2:** Se forman por la confluencia de dos canales de Orden 1.
* **Orden 3:** Se forman por la confluencia de dos canales de Orden 2.
* **Nota:** Si un canal de orden menor (ej. Orden 1) se une a uno de orden mayor (ej. Orden 2), el canal resultante mantiene el orden mayor (Orden 2).

El orden de la cuenca se define por el orden del río en su desembocadura.

```{figure} https://i.pinimg.com/736x/f0/cc/09/f0cc09fb205fdb24a71aa2772af339b1.jpg
:name: fig-4519
:width: 400
```

---
## 4. Cambios del Canal (Nacimiento a Desembocadura)
A medida que el río avanza por las partes de la cuenca, sus características cambian de forma predecible, formando el **perfil longitudinal** (un perfil cóncavo de equilibrio):

* **Nacimiento (Orden 1):** Pendiente muy alta, descarga (caudal) baja, sustrato grueso (bloques, cantos), canal estrecho.
* **Curso Medio:** Pendiente moderada, descarga creciente (por unión de tributarios), sustrato de gravas y arenas.
* **Desembocadura (Orden alto):** Pendiente casi nula, descarga máxima, sustrato fino (limos, arcillas), canal ancho y profundo.
  

```{figure} https://i.pinimg.com/736x/0f/2c/7e/0f2c7e75a1d34441f4e567b40d81582c.jpg
:name: fig-5466
:width: 400
```

---
## 5. Respuesta de la Cuenca y Medición de Caudal

### Caudal Sólido y Líquido
* **Caudal Líquido ($Q$):** Es el volumen de agua que pasa por una sección transversal del río por unidad de tiempo. Se mide en $m^3/s$.
* **Caudal Sólido ($Q_s$):** Es la cantidad (masa o volumen) de sedimento que transporta el río por unidad de tiempo.

### Medición de Caudal (Aforo)
El **aforo** es la medición del caudal. Se realiza en una **sección** del canal. La fórmula básica es:

$$Q = A \times V$$

Donde:
* **$Q$:** Caudal ($m^3/s$)
* **$A$:** Área de la sección transversal ($m^2$). Se calcula midiendo la profundidad en varios puntos a lo ancho del canal.
* **$V$:** Velocidad promedio del flujo ($m/s$). Se mide con instrumentos como un correntómetro o molinete.
  

```{figure} https://i.pinimg.com/1200x/31/6a/93/316a93232c0b102947cdf0bb5c99f630.jpg
:name: fig-8332
:width: 300
```

---
## 6. Significado de la Respuesta de la Cuenca

La **respuesta** de una cuenca es la forma en que transforma una entrada de precipitación (lluvia) en una salida de caudal (el hidrograma).

Cuando llueve, el agua sigue varias rutas antes de llegar al canal:
1.  **Interceptación:** El agua es capturada por la vegetación y se evapora (nunca toca el suelo).
2.  **Infiltración:** El agua penetra en el suelo.
3.  **Escorrentía Superficial (Flujo *Overland*):** Si la lluvia es más intensa que la capacidad de infiltración, el agua fluye sobre la superficie.
4.  **Flujo Subsuperficial (*Throughflow*):** El agua se mueve lateralmente dentro del suelo.
5.  **Flujo Profundo (Agua Subterránea):** El agua percola profundamente, recarga el acuífero y se mueve muy lentamente hacia el río.
   

```{figure} https://i.pinimg.com/736x/9a/5a/dc/9a5adcaebff1ed6dd88495cf94d1581a.jpg
:name: fig-8307
:width: 700
```

---
## 7. Respuesta Lenta vs. Respuesta Rápida

El hidrograma (gráfico de caudal vs. tiempo) muestra dos componentes:

* **Respuesta Rápida (Flujo Pico):**
    * **Definición:** El aumento rápido del caudal durante e inmediatamente después de una tormenta.
    * **Flujo Dominante:** Principalmente la **Escorrentía Superficial**. También incluye el flujo subsuperficial rápido (ver Q9).
    * **Causa:** La precipitación supera la capacidad de infiltración. Genera crecidas súbitas.

* **Respuesta Lenta (Flujo Base):**
    * **Definición:** El caudal sostenido del río que existe antes y mucho después de la tormenta.
    * **Flujo Dominante:** **Flujo Profundo** (agua subterránea).
    * **Causa:** Liberación lenta y constante del agua almacenada en los acuíferos.

---
## 8. Variables que Afectan la Respuesta de la Cuenca
* **Geología:** Rocas permeables (calizas, areniscas) fomentan la infiltración y una respuesta **lenta**. Rocas impermeables (granitos, arcillolitas) fomentan la escorrentía y una respuesta **rápida**.
* **Suelos:** Suelos gruesos y profundos = respuesta lenta. Suelos delgados o arcillosos = respuesta rápida.
* **Cobertura Vegetal:** Los bosques interceptan la lluvia, protegen el suelo y sus raíces facilitan la infiltración. Una alta cobertura vegetal genera una respuesta **lenta**.
* **Pendiente:** Pendientes fuertes = respuesta rápida.

---
## 9. Agua en el Suelo y Permeabilidad Secundaria
* **Agua Higroscópica:** Agua adherida fuertemente a las partículas del suelo; no disponible para las plantas.
* **Punto de Marchitez Permanente (PMP):** Nivel de humedad donde solo queda agua higroscópica.
* **Agua Capilar:** Agua retenida en los microporos por tensión superficial. Es el agua disponible para las plantas.
* **Capacidad de Campo (CC):** Humedad que queda en el suelo después de que el agua gravitacional ha drenado.
* **Agua Gravitacional:** Agua en los macroporos que drena por gravedad. Esta es el agua que se convierte en flujo subsuperficial y profundo.
* **Permeabilidad Secundaria:** Se refiere a la infiltración y flujo que no ocurre a través de los poros del suelo (matriz), sino a través de **macroporos** (fracturas, grietas de desecación, canales de raíces, madrigueras). Esta permeabilidad tiene un efecto dual: permite que el agua se infiltre *rápidamente* (reduciendo la escorrentía superficial) pero también le permite moverse *rápidamente* como flujo subsuperficial, contribuyendo a la respuesta rápida del hidrograma.
  
  
```{figure} https://i.pinimg.com/736x/db/d6/58/dbd658e9049f882148da51be58eb5aa2.jpg
:name: fig-3295
:width: 600
```

---
## 10. Forma de la Cuenca y su Respuesta

* **Cuenca Ovalada (o Redondeada):** Los tributarios tienen longitudes similares. El agua de todas las partes de la cuenca llega al punto de salida casi al mismo tiempo.
    * **Respuesta:** Muy **rápida** y **picuda**. Alto riesgo de crecidas.
* **Cuenca Alargada:** Los tributarios están escalonados. El agua de las cabeceras tarda mucho más en llegar a la salida que el agua de la parte baja.
    * **Respuesta:** Más **lenta** y **atenuada** (el pico es más bajo y se extiende por más tiempo).
  
  
```{figure} https://i.pinimg.com/1200x/5b/b7/46/5bb746ebf650e27663fd8e64b25ea642.jpg
:name: fig-382
:width: 400
```

---
## 11. Efecto de la Urbanización en la Respuesta

La urbanización (impermeabilización de suelos con concreto y asfalto) altera drásticamente la hidrología.

1.  **Reduce la Infiltración:** Casi a cero en áreas pavimentadas.
2.  **Reduce la Interceptación:** Se elimina la cobertura vegetal.
3.  **Aumenta la Escorrentía:** Todo lo que no se infiltra, se convierte en escorrentía superficial.

**Resultado en el Hidrograma:**
* La respuesta es **extremadamente rápida**.
* El **caudal pico es mucho mayor** (más volumen de agua en menos tiempo).
* El flujo base desaparece (no hay recarga de acuíferos).

**Efecto en los Periodos de Retorno:**
La urbanización **aumenta la magnitud del caudal pico para un mismo periodo de retorno**. Por ejemplo, una tormenta que antes (sin urbanizar) causaba una inundación con periodo de retorno de 10 años, ahora (urbanizada) puede causar un caudal pico que antes solo se veía cada 50 o 100 años. El sistema se vuelve mucho más propenso a inundaciones frecuentes y severas.

```{figure} https://i.pinimg.com/736x/b8/a9/60/b8a9603575787606d8caff50ed0deb49.jpg
:name: fig-7885
:width: 700
```
---
## Cuencas Hidrográficas en Colombia

Colombia cuenta con cinco grandes regiones hidrográficas (Amazonas, Orinoco, Caribe, Pacífico y Catatumbo).

* **Cuenca del Magdalena-Cauca:** Es la más importante desde el punto de vista socioeconómico, drenando el 24% del territorio nacional. Es una cuenca de gran complejidad tectónica y climática.
* **Cuencas del Pacífico:** Caracterizadas por longitudes cortas, pendientes extremas y una de las pluviosidades más altas del mundo (ej. cuenca del río Atrato), lo que genera caudales específicos altísimos y gran transporte de sedimentos.
* **Gestión de Cuencas:** En Colombia, las **POMCA** (Planes de Ordenación y Manejo de Cuencas Hidrográficas) son el instrumento legal para la gestión del riesgo y el recurso hídrico.

---
## 12. Morfometría de Cuencas: Más Allá del Orden de Strahler

La jerarquización de Strahler (Sección 3) es solo el punto de partida de la **morfometría de cuencas**, el análisis cuantitativo sistemático de la geometría de las redes de drenaje. Robert Horton, precursor de este enfoque, observó que ciertas proporciones entre variables de la red de drenaje se mantienen notablemente constantes de una cuenca a otra, lo que sugiere que las redes fluviales no son aleatorias sino el resultado de procesos físicos que producen una organización jerárquica predecible {cite:p}`strahler_quantitative_1957,bierman_key_2013`.

### Leyes de Horton

* **Ley de los Números de Canal:** La razón entre el número de canales de un orden dado ($N_u$) y el número de canales del orden inmediatamente superior ($N_{u+1}$) es aproximadamente constante para todos los órdenes de una cuenca. Esta constante se conoce como la **razón de bifurcación** ($R_b$):

$$R_b=\frac{N_u}{N_{u+1}}$$

* **Ley de las Longitudes de Canal:** De forma análoga, la longitud promedio de los canales tiende a aumentar geométricamente con el orden, según una razón de longitud ($R_L$) también aproximadamente constante entre órdenes sucesivos {cite:p}`bierman_key_2013`.

En la mayoría de las cuencas naturales, $R_b$ toma valores entre 3 y 5. Valores de $R_b$ inusualmente altos o bajos pueden indicar un fuerte control estructural o litológico sobre la red de drenaje (ver {ref}`sec-morfotectonica`), en lugar de un desarrollo puramente erosivo "libre".

### La Ley de Hack: Longitud del Cauce Principal vs. Área de la Cuenca

Otra relación morfométrica robusta, documentada por John Hack, vincula la longitud del cauce principal ($L$) con el área de la cuenca que drena ($A$) mediante una ley de potencia {cite:p}`bierman_key_2013`:

$$L=cA^{h}$$

Donde $c$ es una constante y el exponente $h$ toma típicamente valores cercanos a 0.6 en cuencas de todo el mundo, un valor notablemente consistente entre climas y litologías muy distintos. Este exponente, ligeramente mayor a 0.5 (el valor esperado si las cuencas fueran geométricamente similares en todas las escalas), implica que las cuencas grandes tienden a ser proporcionalmente más alargadas que las cuencas pequeñas, un patrón con implicaciones directas sobre la forma del hidrograma (ver Sección 10, arriba) {cite:p}`bierman_key_2013`.

| Herramienta Morfométrica | Qué Cuantifica | Aplicación Práctica |
| :--- | :--- | :--- |
| Razón de Bifurcación ($R_b$) | Grado de ramificación de la red de drenaje | Detectar control estructural/litológico anómalo |
| Razón de Longitud ($R_L$) | Tasa de crecimiento de la longitud de canal con el orden | Comparar la eficiencia de drenaje entre cuencas |
| Curva/Integral Hipsométrico (ver {ref}`sec-evolucion`) | Distribución de área con la elevación (etapa de disección) | Inferir el "estado" evolutivo relativo de una cuenca |
| Ley de Hack ($L=cA^h$) | Relación entre longitud del cauce principal y área de cuenca | Predecir la forma y el tiempo de concentración de una cuenca no instrumentada |

Estas herramientas morfométricas, calculables directamente a partir de un Modelo Digital de Elevación, permiten caracterizar objetivamente cuencas no instrumentadas —una situación común en buena parte del territorio colombiano— y son la base cuantitativa que sustenta muchos de los criterios cualitativos de forma y respuesta hidrológica discutidos en la Sección 10 {cite:p}`bierman_key_2013`.

---
## Taller de Autoevaluación

1. **Órdenes de Drenaje:** Dado un mapa de una red de drenaje, identifique los canales de orden 1, 2 y 3 según Strahler. ¿De qué orden es la cuenca si su río principal es de orden 4?
2. **Respuesta Hidrológica:** Explique por qué una cuenca ovalada tiende a producir crecidas más peligrosas que una cuenca alargada.
3. **Urbanización:** ¿Cómo afecta la pavimentación de una cuenca al tiempo de retraso (*lag time*) entre la tormenta y el pico del hidrograma?
4. **Perfil Longitudinal:** Describa cómo cambia el sustrato del lecho desde la cuenca alta hasta la desembocadura. ¿Por qué ocurre este cambio?
5. **Balance Hidráulico:** Si un río tiene un área de sección de 50 m² y una velocidad de 2 m/s, ¿cuál es su caudal? Si aguas abajo el área aumenta a 100 m² y no hay tributarios, ¿cuál será la nueva velocidad promedio?
