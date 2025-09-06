# Laboratorio 2 Convolución y correlación
## Resumen 
En este laboratorio se abordarán los conceptos fundamentales de convolución y correlación. Asimismo, se realizará el procesamiento de una señal biológica mediante la Transformada de Fourier, complementado con un análisis estadístico de la tranformada y de la señal.

## Parte A 
Para iniciar, se seleccionaron dos señales distintas, generadas a partir de los dígitos del código estudiantil y de la cédula de cada integrante del grupo. Una vez definidas, se procedió a aplicar la operación de convolución entre ellas, con el objetivo de analizar su comportamiento combinado. Este proceso se realizó tanto manualmente como digitalmente por medio de python.
Se realizó el diagrama de flujo que se muestra a continuación:

![Diagramas de flujo lab 2_page-0001](https://github.com/user-attachments/assets/5d4a701f-3407-4b2e-b77a-cda77da48e17)

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

Para esta sección se realizó el siguiente diagrama de flujo:

![Diagramas de flujo lab 2_page-0002](https://github.com/user-attachments/assets/54bb142f-054b-47a5-a809-b676e1d4c451)


En la parte B del laboratorio se definieron dos señales. A continuación se presentan:

<img width="416" height="43" alt="image" src="https://github.com/user-attachments/assets/31ed6cc7-1b3b-4593-a9ec-053b9bfba405" />

Dado que el período de muestreo es de 1.25 ms, se requería calcular la correlación cruzada entre ambas funciones. Para ello, se utilizo el siguiente código:

```python
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd

Ts = 1.25e-3 
f = 100       
n = np.arange(0, 10)  
x1 = np.cos(2 * np.pi * f * n * Ts)
x2 = np.sin(2 * np.pi * f * n * Ts)

corr = np.correlate(x1, x2, mode='full')
lags = np.arange(-len(x1) + 1, len(x1))

plt.figure(figsize=(12, 6))
```

Luego, se graficaron ambas señales con el siguiente código:

```python
plt.subplot(2, 1, 1)
plt.stem(n, x1, linefmt='mediumorchid', markerfmt='o', basefmt='gray', label='x1[n] = cos(...)')
plt.stem(n, x2, linefmt='turquoise', markerfmt='o', basefmt='gray', label='x2[n] = sin(...)')
plt.title('Señales x1[n] y x2[n]')
plt.xlabel('n')
plt.ylabel('Amplitud')
plt.legend()
plt.grid(True)
```
El resultado se muestra en la siguiente gráfica:

<img width="1544" height="382" alt="image" src="https://github.com/user-attachments/assets/c9fa8c23-5e02-4fd5-aaf0-34132723ca7c" />

La correlación se muestra en la siguiente gráfica, obtenida con el siguiente código:

```python
plt.subplot(2, 1, 2)
plt.stem(lags, corr, linefmt='lightcoral', markerfmt='o', basefmt='gray')
plt.title('Correlación cruzada entre x1[n] y x2[n]')
plt.xlabel('Desfase (lags)')
plt.ylabel('Amplitud')
plt.grid(True)

plt.tight_layout()
plt.show()
```
Esta es la gráfica obtenida:

<img width="1544" height="382" alt="image" src="https://github.com/user-attachments/assets/d6307c17-0425-4956-8fa5-cee2d60092e5" />

A continuación se responde la pregunta: ¿En qué casos es útil aplicar la correlación cruzada en el procesamiento digital de señales?







## Parte C 

En este apartado se tiene el siguiente diagrama de flujo:

![Diagramas de flujo lab 2_page-0003](https://github.com/user-attachments/assets/5171ca10-df48-4843-82f4-62d57617e890)

![Diagramas de flujo lab 2_page-0004](https://github.com/user-attachments/assets/aa34b769-a817-4195-a43f-8b6fc4623e11)

Para el desarrollo de la parte C del laboratorio de captura una señal EOG del generador de señales biológicas implementando el entorno spyder de el programa ANACONDA. Para la captura y almacenamiento de la señal se desarrolló el siguiente código:
```python
Import nidaqmx                     # Librería daq. Requiere haber instalado el driver nidaqmx
from nidaqmx.constants import AcquisitionType # Para definir que adquiera datos de manera consecutiva
import matplotlib.pyplot as plt    # Librería para graficar
import numpy as np                 # Librería de funciones matemáticas

#%% Adquisición de la señal por tiempo definido

fs = 16           # Frecuencia de muestreo en Hz. Recordar cumplir el criterio de Nyquist
duracion = 5       # Periodo por el cual desea medir en segundos
senal = []          # Vector vacío en el que se guardará la señal
dispositivo = 'Dev2/ai0' # Nombre del dispositivo/canal (se puede cambiar el nombre en NI max)

total_muestras = int(fs * duracion)

with nidaqmx.Task() as task:
    # Configuración del canal
    task.ai_channels.add_ai_voltage_chan(dispositivo)
    # Configuración del reloj de muestreo
    task.timing.cfg_samp_clk_timing(
        fs,
        sample_mode=AcquisitionType.FINITE,   # Adquisición finita
        samps_per_chan=total_muestras        # Total de muestras que quiero
    )

    # Lectura de todas las muestras de una vez
    senal = task.read(number_of_samples_per_channel=total_muestras)

t = np.arange(len(senal))/fs # Crea el vector de tiempo
plt.plot(t,senal)
plt.axis([0,duracion,-2.5,2.5])
plt.grid()
plt.title(f"fs={fs}Hz, duración={duracion}s, muestras={len(senal)}")
plt.show()
#%%
np.savetxt(f"labo fs{fs}.txt", [t,senal])
```

Con el anterior código se guarda la señal en un archivo .txt para posteriormente realizar la lectura de la señal y realizar el gráfico de esta, para esto empleamos el siguiente código:
```python
import numpy as np
import matplotlib.pyplot as plt


data = np.loadtxt("/content/labo fs16 (1).txt")

#Transponer filas a columnas
data = data.T

# 3) Separar columnas
t = data[:,0]
x = data[:,1]


# 5) Graficar
plt.figure(figsize=(8,5))
plt.plot(t, x)
plt.xlabel("Tiempo (s)")
plt.ylabel("Amplitud")
plt.axis([0,5,-2.5,2.5])
plt.title("blabla")
plt.grid(True)
plt.show()

```
Obteniendo la siguiente señal:


