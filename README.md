# Simulación de quema de gas en mecheros de pozos petroleros

Esta aplicación web proporciona una simulación interactiva del proceso de quema de gas en un mechero (flare stack) utilizado en pozos petroleros. La simulación permite visualizar cómo diferentes parámetros afectan a la combustión del gas, la formación de la llama, y la dispersión de contaminantes en el ambiente.

## Características principales

- **Simulación en tiempo real** de la quema de gas y dispersión de contaminantes
- **Controles interactivos** para modificar parámetros clave:
  - Caudal de gas
  - Velocidad y dirección del viento
  - Condiciones ambientales (temperatura, humedad)
  - Características del mechero (altura, diámetro)
- **Visualización dual**:
  - Vista lateral: muestra la altura de la llama y dispersión vertical de contaminantes
  - Vista superior: muestra el área de dispersión horizontal y alcance de los contaminantes
- **Cálculo de emisiones** de contaminantes (CO₂, CO, NOx, SOx, partículas, metano, VOCs) en kg/día y kg/año
- **Información en tiempo real** sobre la altura de la llama, inclinación y área afectada

## Uso de la aplicación

1. Abra el archivo `index.html` en cualquier navegador web moderno
2. Utilice los controles deslizantes para ajustar los diferentes parámetros
3. Observe cómo los cambios afectan a las visualizaciones y a los valores calculados

## Parámetros de simulación

| Parámetro | Rango | Descripción |
|-----------|-------|-------------|
| Caudal de gas | 10,000 - 2,000,000 ft³/día | Volumen de gas quemado diariamente |
| Velocidad del viento | 0 - 50 km/h | Velocidad del viento en el área del mechero |
| Dirección del viento | 0 - 359° | Dirección desde donde sopla el viento (0=Norte, 90=Este) |
| Temperatura ambiente | -20 - 50 °C | Temperatura del aire circundante |
| Humedad relativa | 0 - 100 % | Porcentaje de humedad en el aire |
| Altura del mechero | 5 - 30 m | Altura de la torre del mechero |
| Diámetro del mechero | 0.1 - 2 m | Diámetro de la salida del mechero |

## Modelo de cálculo

La simulación utiliza modelos simplificados para estimar:

- **Altura de la llama**: Basada en el caudal de gas y diámetro del mechero
- **Inclinación de la llama**: Proporcional a la velocidad del viento
- **Dispersión de contaminantes**: Basada en dirección y velocidad del viento, características de la llama
- **Emisiones de contaminantes**: Calculadas utilizando factores de emisión estándar para la industria petrolera

## Contaminantes calculados

- Dióxido de carbono (CO₂)
- Monóxido de carbono (CO)
- Óxidos de nitrógeno (NOx)
- Óxidos de azufre (SOx)
- Material particulado
- Metano (CH₄)
- Compuestos orgánicos volátiles (VOC)

## Consideraciones técnicas

Esta aplicación es una simulación educativa que utiliza aproximaciones y modelos simplificados. Las visualizaciones y cálculos ofrecen una representación conceptual del fenómeno, pero no deben utilizarse para análisis profesionales de impacto ambiental. Para estudios detallados, se recomienda el uso de software especializado y modelos más complejos que consideren condiciones meteorológicas locales, composición específica del gas, y otros factores relevantes.

## Tecnologías utilizadas

- HTML5
- CSS3
- JavaScript (Vanilla)
- Animaciones mediante requestAnimationFrame

## Instalación

No se requiere instalación. Simplemente descargue los archivos del repositorio y abra `index.html` en su navegador.

## Contribuciones

Las contribuciones son bienvenidas. Si desea mejorar esta simulación, por favor:

1. Haga un fork del repositorio
2. Cree una rama para su funcionalidad (`git checkout -b nueva-funcionalidad`)
3. Realice sus cambios y haga commit (`git commit -am 'Añadir nueva funcionalidad'`)
4. Haga push a la rama (`git push origin nueva-funcionalidad`)
5. Cree un nuevo Pull Request

## Licencia

Este proyecto está licenciado bajo la Licencia MIT - vea el archivo LICENSE para más detalles.

## Contacto

Si tiene preguntas o sugerencias sobre esta simulación, no dude en abrir un issue en este repositorio.

---

*Nota: Esta simulación es un recurso educativo y no representa con exactitud completa la complejidad de los procesos reales de quema de gas en pozos petroleros.*
