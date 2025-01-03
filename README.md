# Análisis de datos experimentales de absorción de radiación gamma

Este repositorio contiene un análisis de datos experimentales de absorción de radiación gamma para diferentes isotopos (Cs-137, Na-22 y Ba-133), utilizando técnicas de integración numérica y ajuste de modelos. El proyecto se centra en el estudio de la variación de la absorbancia con el espesor de materiales absorbentes y la comparación de diferentes métodos de integración, como la regla del trapecio y la de Simpson.

## Descripción del Proyecto

El análisis se realiza sobre los espectros de radiación provenientes de los siguientes isotopos radiactivos:

- **Cs-137 (661 keV)**  
- **Na-22 (1275 keV y 511 keV)**  
- **Ba-133 (160 keV)**

Se procesaron varios archivos de datos de espectros de radiación para diferentes anchos de absorbente. El análisis incluye:

1. **Carga de los Datos**: Los archivos de datos espectrales se cargan y procesan desde un directorio de Google Drive.
2. **Procesamiento de Datos**: Se extraen las cuentas de cada espectro y se calculan las áreas bajo la curva utilizando los métodos de integración numérica (Trapecio y Simpson).
3. **Análisis Comparativo**: Se compara la absorbancia a diferentes espesores de material utilizando los métodos mencionados. Se ajusta un modelo lineal a los logaritmos de los cocientes de las áreas integradas.
4. **Gráficas**: Se generan gráficos de absorbancia versus espesor del material, junto con los ajustes teóricos.

## Requisitos

Para ejecutar este notebook, necesitas las siguientes librerías de Python:

- `numpy`
- `matplotlib`
- `scipy`

Puedes instalar las dependencias con:

```bash
pip install numpy matplotlib scipy
```
## Resultados

El proyecto incluye gráficos y modelos ajustados que muestran la relación entre el espesor del absorbente y la absorbancia para cada isotopo. Estos resultados son útiles para entender el comportamiento de los materiales frente a la radiación en diferentes configuraciones experimentales.

![Gráfico final](https://github.com/ffborgo/coef-de-absorcion/blob/main/grafico.png|300)

## Cómo Ejecutar

1. Clona este repositorio en tu máquina local:
   ```bash
   git clone https://github.com/ffborgo/coef-de-absorcion.git
   ```

## Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar este proyecto, por favor crea una nueva rama y asegurate de que tus cambios sean coherentes con el estilo del proyecto y que no rompan la funcionalidad existente.
