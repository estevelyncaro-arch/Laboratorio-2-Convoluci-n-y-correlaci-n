# Laboratorio 2 Convolución y correlación
## Resumen 
En este laboratorio se abordarán los conceptos fundamentales de convolución y correlación. Asimismo, se realizará el procesamiento de una señal biológica mediante la Transformada de Fourier, complementado con un análisis estadístico de la tranformada y de la señal.

## Parte A 
Para iniciar, se seleccionaron dos señales distintas, generadas a partir de los dígitos del código estudiantil y de la cédula de cada integrante del grupo. Una vez definidas, se procedió a aplicar la operación de convolución entre ellas, con el objetivo de analizar su comportamiento combinado. Este proceso se realizó tanto manualmente como digitalmente por medio de python.

A continuacion la convulución manual de la primera estudiante:

<img width="521" height="831" alt="image" src="https://github.com/user-attachments/assets/73e03190-4348-4ba8-b584-30931a92c142" />

El resultado de esta convolución:

<img width="606" height="286" alt="image" src="https://github.com/user-attachments/assets/e0aeb183-aee6-4479-9642-41d3a3062885" />

Su respectivo grafico:

<img width="628" height="810" alt="image" src="https://github.com/user-attachments/assets/ab8fd9dc-81e0-43bd-9986-2397e7081d67" />

Por siguiente el codigo de la convulución de la primera estudiante:

```python
  import numpy as np
  import matplotlib.pyplot as plt

  xp=(1,0,7,6,2,4,1,5,9,8)
  hp=(5,6,0,0,6,0,5)

  yp=np.convolve(xp,hp)
  print(f"y(n) ={yp}")
```

El resultado de la convolución:

<img width="611" height="39" alt="image" src="https://github.com/user-attachments/assets/93cb8ad9-144a-4822-b9e6-ed6a12ce39d6" />

El codigo para el grafico:

```python
mp= np.array([0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15])
plt.stem(mp, yp)
plt.title("Gráfico de Paula")
plt.xlabel("Eje X")
plt.ylabel("Eje Y")
plt.show()

```

El grafico por medio de python:

<img width="704" height="586" alt="image" src="https://github.com/user-attachments/assets/7c940833-09b6-4af7-853f-be48aaf088b6" />





## Parte B 


## Parte C 
