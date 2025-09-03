# Laboratorio 2 Convolución y correlación
## Resumen 
En este laboratorio se abordarán los conceptos fundamentales de convolución y correlación. Asimismo, se realizará el procesamiento de una señal biológica mediante la Transformada de Fourier, complementado con un análisis estadístico de la tranformada y de la señal.

## Parte A 
Para iniciar, se seleccionaron dos señales distintas, generadas a partir de los dígitos del código estudiantil y de la cédula de cada integrante del grupo. Una vez definidas, se procedió a aplicar la operación de convolución entre ellas, con el objetivo de analizar su comportamiento combinado. Este proceso se realizó tanto manualmente como digitalmente por medio de python.

### Convolución Primera señal 
A continuacion la convulución manual de la primera estudiante:

<img width="521" height="831" alt="image" src="https://github.com/user-attachments/assets/73e03190-4348-4ba8-b584-30931a92c142" />

El resultado de esta convolución:

<img width="606" height="286" alt="image" src="https://github.com/user-attachments/assets/e0aeb183-aee6-4479-9642-41d3a3062885" />

Su respectivo grafico:

<img width="628" height="710" alt="image" src="https://github.com/user-attachments/assets/ab8fd9dc-81e0-43bd-9986-2397e7081d67" />

Por otro lado el codigo de la convolución de la primera estudiante:

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

### Convolución Segunda señal 
Posteriormente la convolución manual de la segunda estudiante:

<img width="521" height="831" alt="image" src="https://github.com/user-attachments/assets/2e51caea-1ef0-474b-b776-7ee4949fa0de" />

El resultado de esta convolución:

<img width="606" height="286" alt="image" src="https://github.com/user-attachments/assets/e10764e5-51c1-4b9f-8020-840d26622f81" />

Su respectivo grafico:

<img width="628" height="710" alt="image" src="https://github.com/user-attachments/assets/49bfdfee-cd42-4e3b-9d2f-ab6c05b14733" />

Seguidamente el codigo en python para la convolución:

```python
import numpy as np
import matplotlib.pyplot as plt

xe=(1,0,7,6,2,4,2,9,9,8)
he=(5,6,0,0,8,4,8)

ye=np.convolve(xe,he)
print(f"y(n) ={ye}")

```

Resultado de la convolución:

<img width="611" height="39" alt="image" src="https://github.com/user-attachments/assets/353c6dbc-845f-489e-b776-0f4da21814c5" />

El codigo para el grafico:

```python
me= np.array([0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15])
plt.stem(me, ye)
plt.title("Gráfico de Evelyn")
plt.xlabel("Eje X")
plt.ylabel("Eje Y")
plt.show()
```

El grafico por medio de python:

<img width="704" height="586" alt="image" src="https://github.com/user-attachments/assets/2c44dcaa-61cb-437e-b96e-c26cb5844467" />

### Convolución Tercera señal 

Por ultimo la convolución manual de la tercera estudiante:

<img width="500" height="277" alt="image" src="https://github.com/user-attachments/assets/1e37e646-98aa-4604-8c29-8215089ba31e" />

<img width="521" height="554" alt="image" src="https://github.com/user-attachments/assets/48e5ac0c-90f8-41db-a790-97d71201a4f4" />

El resultado de la ultima convolución:

<img width="606" height="286" alt="image" src="https://github.com/user-attachments/assets/bc824ac4-d29a-4d12-a7e0-baea87502844" />

Su respectivo grafico:

<img width="628" height="710" alt="image" src="https://github.com/user-attachments/assets/495e95a4-bd49-4280-b52d-2211e937935d" />

Por otro ultimo el codigo de la convolución de la tercera estudiante:

```python
import numpy as np
import matplotlib.pyplot as plt

xm=(1,1,3,7,9,7,6,5,2,4)
hm=(5,6,0,0,8,5,2)

ym=np.convolve(xm,hm)
print(f"y(n) ={ym}")
```

Resultado de la convolución:

<img width="611" height="39" alt="image" src="https://github.com/user-attachments/assets/d56b4bc5-fe79-4a8f-8523-830e9c6a35c9" />

El codigo para el grafico:

```python
mm= np.array([0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15])

plt.stem(mm, ym)

plt.title("Gráfico de Maria")
plt.xlabel("Eje X")
plt.ylabel("Eje Y")

plt.show()
```

El grafico por medio de python:

<img width="704" height="586" alt="image" src="https://github.com/user-attachments/assets/b87b47f7-c0cc-4744-aa13-b184cb025cf0" />

## Parte B 


## Parte C 
