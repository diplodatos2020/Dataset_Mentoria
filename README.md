Análisis de Red de Telecomunicaciones
=====================================

### **Mentor**: Mario Ferreyra


### Descripción

Se propone analizar los datos provenientes de una de las Áreas de Negocio de la Empresa para la cual trabajo. Hablamos de su Red de Telecomunicaciones a nivel provincial. La misma, está compuesta por la Infraestructura de la Red de Telecomunicaciones propiamente dicha, la cual abarca la Red Teleoperación e Interconexión de Estaciones Eléctricas, la Red de Telemedición y Transporte de Datos, Red de Infraestructura de TI, Red de Protección del Tendido Eléctrico y la Red para Provisión/Comercialización de Internet Corporativo.

Cabe aclarar que físicamente se trata de la misma Red. La Fibra Óptica instalada permite todos estas aplicaciones y usos, al igual que sus radioenlaces de alta capacidad. Dicha fibra nos brinda mayor fiabilidad, alta resistencia a las inclemencias del tiempo, dimensiones y pesos reducidos, velocidad en la transmisión ilimitada, pero su despliegue es más lento y costoso. Los enlaces de radiofrecuencia son más económicos, su despliegue es más dinámico, pero sus alcances en cuanto a anchos de banda son limitados. Cualquiera fuere el medio, esta red debe estar bajo estudio constante a fin de evitar fallas o anomalías.

En esta mentoría se propone:
* Análisis de Tráfico de la red, para detectar comportamientos sospechosos en función de garantizar la seguridad de los Sistemas que la usan y de la propia Red.
* Utilización y capacidad de la Red.
* Predicción de consumo, cortes, saturación y desperfectos en la Red para analizar ampliaciones y/o modificaciones en la Infraestructura actual.

### Lo interesante del tema

Los resultados del Proyecto se pueden implementar para mejorar la Calidad del Servicio brindado actualmente por la Red.

El análisis y sus resultados nos permitirán tener una acabada idea de su capacidad, utilización, eficiencia, control y seguridad.

### Trataremos de responder algunas de las siguientes preguntas

* ¿Es posible predecir cortes o desperfectos en la Red?
* ¿Podemos predecir el uso de la Red en las próximas 24 horas? ¿En la próxima semana?
* ¿Es posible detectar anomalías o comportamientos sospechosos en el tráfico de la Red?
* ¿La actividad de la Red varía según el día de la semana o mes? 
* ¿Los cortes en la Red están asociados con alguna otra/s variable/s del set de datos?

---

Dataset
=======

* Archivo: `dataset_inf_telec.csv`

* Consta de +16K registros (filas) y 11 features (columnas)

| Feature                   | Descripción                                        |
|:-------------------------:|:---------------------------------------------------|
| **ID_EQUIPO**             | Switch/Router                                      |
| **PUNTO_MEDICION**        | Línea Troncal                                      |
| **CAPACIDAD_MAXIMA_GBS**  | Capacidad maxima [Gigabit/seg]                     |
| **FECHA_INICIO_MEDICION** | Fecha y hora inicio medicion                       |
| **FECHA_HORA**            | Fecha y hora efectiva de la medida                 |
| **FECHA_FIN_MEDICION**    | Fecha y hora fin de medicion                       |
| **PASO**                  | -                                                  |
| **LATENCIA_MS**           | Latencia (tiempo de espera de la respuesta) [mseg] |
| **PORCENTAJE_PACK_LOSS**  | % de paquetes perdidos (pings configurados en diferentes momentos del dia) |
| **INBOUND_GBPS**          | Trafico de entrada [Gigabit/seg]                   |
| **OUTBOUND_GBPS**         | Trafico de salida  [Gigabit/seg]                   |

---

Entorno Virtual
===============

1. Para crear y activar nuestro virtualenv:

        $ conda create --name dd20 python=3.6
        $ conda activate dd20

2. Instalar dependencias:

        $ pip install -r requirements.txt
