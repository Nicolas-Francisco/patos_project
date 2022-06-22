# Accidentes de tránsito en Estados Unidos, 
### Proyecto del curso de Procesamiento Masivo de Datos
Integrantes: 
- Javier Lavados Jillbert, 
- Jorge Barraza, 
- Nicolás García Ríos

## How to run
El proyecto parte con el mismo set-up del Laboratorio 5 (Spark).
El dataset se encuentra en la siguiente dirección del servidor de uhadoop:

```
hdfs://cm:9000/uhadoop2022/blackfiregroup/data.csv
```

Por otro lado, el archivo .jar del proyecto se encuentra en la siguiente dirección:

```
hdfs://cm:9000/uhadoop2022/blackfiregroup/mdp-spark.jar
```

Para ejecutar alguna de las dos clases, debe ejecutarse el siguiente código (sin saltos de línea)
```
spark-submit --master spark://cluster-01:7077 /data/2022/uhadoop/blackfiregroup/mdp-spark.jar 
<CLASS> hdfs://cm:9000/uhadoop2022/blackfiregroup/data.csv 
hdfs://cm:9000/uhadoop2022/blackfiregroup/accidents-count/
```

Donde `<CLASS>` puede ser a la primera querie `AccidentsByWeekdayRating` o la segunda `SeverityByWeekday`
