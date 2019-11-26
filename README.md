# SD-SentimentTwitterAnalysis

Analizador de sentimientos a partir de una recolección de tweets sobre el término indicado.

-Realizado como Práctica 3 para la asignatura de Sistemas Distribuidos (Universidad de Cádiz - 2017/2018)-


### Autores

* **Miguel Ángel Álvarez García** - [GitHub](https://github.com/IamMiguelAA)
* **Ana Gómez González** - [GitHub](https://github.com/angoglez)


### Tecnologías utilizadas

* [Anypoint Platform](https://anypoint.mulesoft.com/home/)


### Funcionamiento

Se recomienda la instalación a través de pip de todos los paquetes necesarios relacionados con las tencologías empleadas expresadas en el apartado anterior.

1.En la terminal, ejecute:
```
python server.py
```

2.En otra instancia de la terminal, ejecute ahora:
```
celery -A celery_tasks worker -l=info
```
Con ésto ya debemos tener nuestra cola de tareas asíncronas lista y el pequeño servidor web levantado.

3.En su navegador, escriba la dirección:
```
localhost:5000/home
```

4.Escriba en el cuadro de texto el término sobre el que quiere realizar el análisis de sentimiento.
**Nota!** La cadena que introduzca puede usar cualquier de las opciones de [búsqueda avanzada](https://help.twitter.com/es/using-twitter/twitter-advanced-search) ofrecidas por Twitter.
