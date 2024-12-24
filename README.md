# Caidas y periodos de recuperacion en el precio de Bitcoin

<p style="text-align:center">
    <img src="https://media.slovoidilo.ua/media/publications/21/209648/209648-1_large.jpg" width="830" height="180" alt="Bitcoin Logo">
</p>





<h1>Contenidos</h1>
<div class="alert alert-block alert-info" style="margin-top: 20px">
    <ul>
        <li>
            <a href="#Introducción">Introducción</a>
        </li>
        <li>
            <a href="#Exploración">Exploración</a>
        </li>
         <li>
            <a href="#Función">Función central</a>
        </li>
        <li>
            <a href="#Visualización">Visualización</a>
            <ul>
                <li><a href="#Caidas del 10%">Caidas del 10%</a></li>
                <li><a href="#Caidas del 30%">Caidas del 30%</a></li>
                <li><a href="#Caidas del 50%">Caidas del 50%</a></li>
            </ul>
        </li>
    </ul>

</div>

<hr>


# **Introducción**

Este análisis centrado en los precios históricos de Bitcoin ofrece una perspectiva sobre los ciclos de este mercado y las dinámicas de recuperación tras grandes caídas. El objetivo es identificar y estudiar las caídas significativas en el precio de Bitcoin desde 2010 hasta 2024, así como el tiempo que tarda en recuperarse a niveles previos. 
Los gráficos generados en este análisis permiten:

1. **Visualizar caídas significativas:** Identificar momentos en los que el precio de Bitcoin experimentó disminuciones mayores a un cierto porcentaje predefinido, como un 10%.
2. **Rastrear períodos de recuperación:** Medir el número de días que el precio tarda en superar su máximo histórico previo, proporcionando una métrica clara del impacto de las caídas en el mercado.
3. **Analizar patrones históricos:** Observar si existen tendencias en la duración y frecuencia de los períodos de caída y recuperación a lo largo del tiempo.

Estos resultados son útiles para:
- Inversionistas que desean comprender la resiliencia histórica del mercado de Bitcoin frente a caídas significativas.
- Analistas interesados en estudiar patrones de recuperación en mercados volátiles.
- Personas curiosas por explorar el comportamiento del mercado de Bitcoin a lo largo de su historia.




# Exploración
### Librerías utilizadas

<img src="images/librerias_importadas.png" alt="Librerías importadas" width="364" height="190">

### Dataset utilizado
El dataset proviene de Kaggle y contiene datos históricos del precio de Bitcoin y de otras criptomonedas, organizados por fecha. La fuente original del dataset es: https://www.kaggle.com/datasets/svaningelgem/crypto-currencies-daily-prices/data

### Estructura del dataset original
A continuación se muestra una vista inicial de cómo era el dataset original:

<img src="images/estructura_dataSet.png" alt="estructura_dataSet.png" width="590" height="452">

Explicación de cada columna del dataset:
1. ticker
-	Representa el símbolo del activo que se está analizando. En este caso, BTC se refiere a Bitcoin.
2. date
-	La fecha de los datos registrados. Cada fila representa la información del precio de Bitcoin para un día específico.
3. open
-	Es el precio de apertura del día.
-	Este es el precio al que se realizó la primera transacción de Bitcoin al inicio del día (generalmente a la medianoche UTC).
4. high
-	Es el precio máximo alcanzado durante ese día.
-	Refleja el valor más alto al que Bitcoin fue negociado durante las 24 horas del día.
5. low
-	Es el precio mínimo alcanzado durante ese día.
•	Indica el valor más bajo al que Bitcoin fue negociado durante las 24 horas del día.
6. close
-	Es el precio de cierre del día.
-	Este es el precio al que se realizó la última transacción del día (normalmente justo antes de la medianoche UTC).

