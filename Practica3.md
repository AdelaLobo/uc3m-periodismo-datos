# Práctica 3: Gráfico con *Datawrapper*
## Justificación del tema
Este [gráfico](https://datawrapper.dwcdn.net/cO2Dk/1/) de elaboración propia representa **la evolución del volumen de tweets que deseaban una feliz Navidad**. El objetivo de esto era observar cuándo empiezan y terminan las felicitaciones. Es curioso comprobar que los usuarios de Twitter comienzan a desear una feliz Navidad en noviembre. Como vemos, hay quien considera que el periodo navideño comienza cuando termina Halloween. Evidentemente, a finales de diciembre es cuando el volumen de tweets se dispara.
## Proceso de elaboración
Lo primero que he hecho es transformar la columna de las fechas para que *OpenRefine* las considerara como tal. He realizado el mismo proceso con la columna numérica. También he eliminado las columnas de las urls. Por otra parte, he eliminado los datos de 1970 como vimos en clase. Luego he abierto una faceta de texto y he eliminado todas las tendencias que no estuvieran relacionadas con la navidad. De tal manera que las únicas tendencias que he considerado son:
- Feliz Navidad
- Feliz Día de Navidad
- Feliz y Santa Navidad

Al ordenar las fechas me he dado cuenta de que el volumen de tweets del 24 y 25 de noviembre eran desproporcionados. Al parecer, los datos de noviembre aparecerían como si correspondiesen a diciembre en el archivo. Ese ha sido el principal problema que me he encontrado a la hora de realizar este trabajo. Para solucionarlo, cambié manualmente esos datos para que se consideraran como valores de diciembre.
Por último, exporté los datos a un **.csv** y empecé a trabajar con *Datawrapper*. Una vez ahí, inserté el título y las notas correspondientes para que cualquier persona que acceda al gráfico pueda entender la información que se le presenta. 
