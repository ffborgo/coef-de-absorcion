# Determinación del Coeficiente de Atenuación Lineal

Este repositorio contiene el código utilizado para analizar datos experimentales relacionados con la interacción de radiación γ con la materia. El objetivo principal es determinar el coeficiente de atenuación lineal $\mu$ y estudiar la variación de la absorbancia con el espesor de diferentes materiales absorbentes. Además, se comparan métodos de integración numérica, como la regla del trapecio y la de Simpson.

---

## Descripción del Proyecto

El análisis se centra en los espectros de radiación emitidos por los siguientes isótopos radiactivos:

- **Cs-137 (661 keV)**  
- **Na-22 (1275 keV y 511 keV)**  
- **Ba-133 (160 keV)**  

El proyecto incluye las siguientes etapas principales:

1. **Carga de Datos**: 
   - Los espectros de radiación son cargados desde archivos en un directorio de Google Drive.
   
2. **Procesamiento de Datos**: 
   - Se extraen las cuentas de cada espectro.
   - Se calculan las áreas bajo la curva utilizando métodos de integración numérica (Trapecio y Simpson).
   
3. **Análisis Comparativo**: 
   - Se analiza la absorbancia en función del espesor del material para cada isótopo.
   - Se ajusta un modelo lineal a los logaritmos de los cocientes de las áreas integradas.

4. **Generación de Gráficos**: 
   - Se generan gráficos de absorbancia versus espesor, junto con los ajustes lineales y teóricos.

---

## Requisitos

Para ejecutar este proyecto, necesitas tener instaladas las siguientes bibliotecas de Python:

- `numpy`
- `matplotlib`
- `scipy`

Puedes instalarlas con el siguiente comando:

```bash
pip install numpy matplotlib scipy
```

## Resultados

El código genera gráficos y modelos ajustados que muestran la relación entre el espesor del absorbente y la absorbancia para cada isótopo analizado. Estos resultados ayudan a comprender el comportamiento de los materiales frente a la radiación en diferentes configuraciones experimentales.

Ejemplo de gráfico generado:

<img src="https://github.com/ffborgo/coef-de-absorcion/blob/main/grafico.png" alt="Gráfico final" style="width: 60%; max-width: 500px;">

## Contribuciones y uso

Las contribuciones son bienvenidas. Si deseas mejorar este proyecto, por favor crea una nueva rama y sentite libre de modificarlo a tu gusto.
