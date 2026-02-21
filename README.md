# Analisis-HomicidiosDolosos-Narcotrafico-Argentina
Aquí se puede ver el Análisis que realice de la muerte por Homicidios Dolosos por Narcotráfico en Argentina, se analizaran las variables y modelos adecuados a la realidad, teniendo en cuenta que la tasa de mortalidad nunca es menor a 0 o negativa 

PRESENTACIÓN DE LA PROBLEMATICA

El presente informe tiene el objetivo de hacer una evaluación basado en la Tasa de Mortalidad de Homicidios Dolosos en Argentina. Se selecciono esta problemática por un interés en el planteado en la tasa de mortalidad, y factores sociales en Argentina. Los homicidios dolosos por narcotráfico es una importante indicador o factor clave de violencia criminal en Argentina. El propósito del proyecto es analizar el presente problema, se observa que gracias a esto surgió una baja en la tasa de Homicidios en los últimos 7 años, con lo datos adquiridos antes de 2024, por esto se usara en 2025 para una proyección en los próximos 5 años. 

DATOS
Los datos se extrajeron de fuentes oficiales del Sistema Nacional de Información Criminal (SNIC), del informe especifico de lo que analice, este fue publicado por el Ministerio de Seguridad Nacional. Los datos venían acompañados de Tasa de Homicidios de cada 100.000 habitantes. Se trabajo con la tasa en vez de cantidades porque hace el grafico más legible que hacerlo de numero que se alejan de 0 y dañan el grafico a la hora de analizar.  
    • Informe del Sistema de Alerta Temprana (SAT) - Homicidios Dolosos 2024- https://drive.google.com/uc?export=download&id=1-c3T6o1WAkbMif8I1Byj37PyTfFiCYR_
    
TABLA DE DATOS HISTORICOS
  Para el modelo se realizo un cambio en las variables por año porque facilita en análisis en números mas pequeños porque como mencionamos no se alejan de 0. Donde el año 2018 se intercambió en la variable 𝑥 = 1. Pude hacerlo gracias que la guía de estudio lo recomienda lo cual facilita el ajuste de modelo a elegir. También se elegio trabajar por cada 100.000 habitantes porque anteriormente dicho es inimaginable trabajar con datos tan pequeños o muy grandes en cantidades. 
  <img width="932" height="281" alt="Captura de pantalla 2026-02-21 164025" src="https://github.com/user-attachments/assets/2449d4e7-b616-4009-867b-b5c1a63d2aa1" />
    • Fuente de Datos Estadísticos: Ministerio de Seguridad Nacional (2025). Informe SNIC SAT HD 2024, Tabla 2, pág. 15. 
    
METODOLOGIA Y HERRAMIENTAS
Para el análisis se usó GeoGebra Classic 5, para la construcción del modelo y predicción de los datos y ver la tendencia a la que tenían si subida o bajada (Regresión). Permitió que al usarlo ver los puntos donde se marcaban las tasas en el gráfico y el modelo que mayor se adecuaba a ello, también ayudo a obtener los coeficientes de determinación (𝑅2) de manera precisa para ver que modelo funcional se adecuaba más al análisis, teniendo en cuenta lo que planteamos para este proyecto y las tecnologías usadas. 

REPRESENTACIÓN GRAFICA Y SELECCION DE MODELO
<img width="1464" height="668" alt="Captura de pantalla 2026-02-19 140333" src="https://github.com/user-attachments/assets/7e50a388-7674-417f-9cf0-22623c6c3082" />
  Justificación de Selección de Modelo: Se uso dos modelos principales para el descenso de la tasa de homicidios. Por contexto de la realidad la tasa de mortalidad nunca es menor a 0, se inicio con modelado lineal porque es el modelo mas sencillo de trabajar, pero al hacerlo también con modelo polinómico daba a una tasa negativa a 0. Al hacerlo con modelo exponencial se observo que era el único que no daba un decrecimiento menor a 0. Se la diferenció con colores para una mejor lectura. 
      • Modelo Lineal (Recta Rosa): Presento un coeficiente de det. 𝑅2 ≈ 0,88 
      • Modelo Exponencial (Curva Naranja): Presento un coeficiente de det. 𝑅12 ≈ 0,87 
      
  Si bien se ve que matemáticamente gana el Lineal por muy poco, pero a pesar de eso se seleccionó el Modelo Exponencial solo por validación lógica y consistencia con la realidad. El modelo lineal, decrece debajo de 0 anteriormente dicho, lo mismo el modelo polinómico. El modelo exponencial (𝑦 = 𝑘 ∙ 𝑒𝑎𝑥) plantea que es infinita o más conocida como asíntota lo cual nunca toca o se aproxima infinitamente, lo cual 𝑦 = 0, lo cual implica que la violencia disminuye acercándose a 0, el comportamiento de ser decreciente no presenta una pendiente constante (como el lineal), sino una disminución acorde a como se mide la mortalidad. 
      • Función de Modelo Seleccionado: La función exponencial obtenida mediante GeoGebra 
          es: 
                                g(𝑥) = 5,83∙𝑒−0,06𝑥 

  Donde 𝒙 representa el tiempo en años (por eso 𝑥 = 1 en 2018) y 𝑔(𝑥) es la tasa a estimar de homicidios. El exponente a ser negativo (−0,06) se da a entender y confirma que la tendencia es decreciente o va en baja en el periodo analizado. 
  
  NOTA: Las estimaciones daban que en 200 años la tasa de Homicidios Dolosos por Narcotráfico, tendera a aproximarse a 0 sin alcanzarlo, lo cual hace ver que no hay una erradicación absoluta, pero si una reducción progresiva. 
  
Análisis de la Variable (Tasa vs. Cantidad real): Según como lo aclara el informe en el apartado metodológico del SNIC, se calcula de la siguiente forma: 

  T𝑎𝑠𝑎 = (𝐶𝑎𝑛𝑡𝑖𝑑𝑎𝑑/𝑃𝑜𝑏𝑙𝑎𝑐𝑖𝑜𝑛 𝑇𝑜𝑡𝑎𝑙 ∙ 100.000)
  C𝑎𝑛𝑡.𝑅𝑒𝑎𝑙 = (𝑇𝑎𝑠𝑎∙𝑃𝑜𝑏𝑙𝑎𝑐𝑖𝑜𝑛 𝑑𝑒𝑙 𝐴ñ𝑜) / 100.000

  Si ponemos la cantidad de homicidios dado en la tabla del informe del SNIC, tomando el 2024 que fueron 1802 víctimas, sobre la población aproximada de 47 millones, se obtiene probabilidad del 0,000038 de que alguien sea asesinado por estas causas. Lo cual no da en porcentaje 0,0038% de población que falleció por esto durante el 2024, la formula a usar para sacar fue:  
  
  T𝑎𝑠𝑎 𝑅𝑒𝑎𝑙 = 𝑇𝑎𝑠𝑎 / 100.000
  𝑃𝑜𝑟𝑐𝑒𝑛𝑡𝑎𝑗𝑒 = 𝑇𝑎𝑠𝑎 ∙ 100 
  
Aunque el porcentaje sea bajo o nos parezca así, en números son 1802 vidas perdidas, lo que justifica la relevancia socialmente al intentar reducirlo. 

PRONOSTICO (EXTRAPOLACIÓN A 5 AÑOS)
Usando la función dada por GeoGebra en el modelo exponencial 𝑔(𝑥) = 5,83 ∙ 𝑒−0,06𝑥, se realizó una extrapolación en los próximos 5 años (2025-2029), esto se hizo porque ya dicho se conocen datos oficiales o de estos solo del 2024 hacia atrás, por eso tomado como alternativa hacer el análisis desde 2025 en adelante, porque solo son esos los datos que conocemos, los valores de tiempo 𝑥 = 8 y 𝑥 = 12, equivalen a dichos años para hacer el pronóstico. Esto se pudo obtener gracias a poner la letra o punto en la Vista Algebraica del programa, se definió como 𝑙𝑒𝑡𝑟𝑎 𝑒𝑛 𝑀𝑎𝑦.= (𝑣𝑎𝑟.𝑑𝑒 𝑡𝑖𝑒𝑚𝑝𝑜,𝑓𝑢𝑛𝑐𝑖𝑜𝑛(𝑣𝑎𝑟.𝑑𝑒 𝑡𝑖𝑒𝑚𝑝𝑜)), y el programa automáticamente lo pone y lo calcula, lo hace ver mucho mas limpio en la Vista Algebraica, que hacerlo con la función de intersección del programa, también se puede usar una función similar llamada interseca. 
TABLA DE DATOS HISTORICOS
<img width="934" height="430" alt="Captura de pantalla 2026-02-21 164119" src="https://github.com/user-attachments/assets/e2d74b83-c7c1-4dce-88fc-f43639c67948" />

FUNDAMENTACIÓN Y LIMITACIONES DEL ANÁLISIS
Es esencial remarcar que el pronóstico está sujeto a limitaciones propias del análisis de factores sociales claves y la falta de datos del año anterior 2025, y que2026 aun no finalizo, lo cual lleva a limitaciones. 
  1. La extrapolación asume que las condiciones actuales (políticas, gubernamentales, geopolíticas, socioeconómicas, etc.) se mantendrán iguales. Si alguna cambia por ejemplo menos inversión y menos ganas de combatir el problema social y políticamente, podría alterar la curva real. 
  2. Datos faltantes de 2 años 2025 y 2026. Puede haber errores en los próximos 3 años de mi pronostico debido a que se extrapolo desde 2025, lo cual puede presentar fallas en el análisis. La falta se da porque SNIC publica en cierto desfase temporal, por eso es que mi análisis se basa en la ultima vez que se publicaron datos oficiales. 

CONCLUSIÓN: El análisis, hace ver la tendencia es decreciente. Lo cual si sigue las condiciones para el 2029 la baja será de 2,96. Los modelos son fundamental para     decisiones en contexto real

