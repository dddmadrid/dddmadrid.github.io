---
layout: post
title:  "Crónicas de DDD eXchange 2017 - Episodio I"
date:   2017-05-03 22:54:34 +0200
author: "Javier Fernández"
categories: ddd conferencias
comments: true
---

El 27 y 28 de abril tuve la suerte de asistir como ponente a la conferencia [DDD eXchange 2017][ddd-exchange-2017] que tuvo lugar en Londres. A pesar de que todas las charlas están disponibles en la web del organizador, [Skills Matter][skills-matter-talks], creo que puede ser interesante hacer un resumen de las charlas a las que asistí para aquellos que no queráis dedicar los 40 minutos completos a ver cada una.

Nota: para visualizar las charlas es necesario registrarse.

## Buen diseño es diseño imperfecto - Eric Evans
[Good Design is Imperfect Design - Eric Evans][good-design-imperfect-design-evans]

En la charla inicial, Eric Evans nos pide a los desarrolladores de software que __dejemos de utilizar DDD como una excusa para ser perfeccionistas__. Siempre estamos buscando recursos, como principios y reglas, para hacer el camino del desarrollo de software más fácil. No hay una bala de plata: cada uno sabe lo que funciona y lo que no... es un proceso de aprendizaje y como tal, no debebemos obsesionarnos con hacerlo todo bien a la primera. De hecho menciona que los _bounded contexts_ son mecanismos para contener 'el desastre'.

Más adelante nos propone un ejemplo de la suma de tiempo utilizando la librería java.time (antiguamente JodaTime). Utiliza el método ```plus()``` de esta librería para demostrar que un software imperfecto puede ser buen software.

Enlaza esta demostración con una búsqueda de nombres más adecuados para este método ```plus()``` y nos deja una frase interesante: 

> Pon nombres raros a conceptos raros

Por último, Eric nos sugiere que "ampliemos la estética". Deberíamos buscar soluciones alternativas que puede que no cuadren con nuestro concepto de estado del arte. En definitiva, debemos intentar huir del perfeccionismo que parece que nos causa DDD.

## Escenarios de BDD como Modelos de Dominio - Ciaran McNulty
[BDD Scenarios as Domain Models - Ciaran McNulty][bdd-scenarios-as-domain-models-mcnulty]

¿Cómo combinar DDD y BDD? Ciaran propone centrarnos en un problema de negocio, establecer unas soluciones de negocio, priorizarlas y, a continuación, buscar algunas soluciones técnicas para poder resolver estos problemas de negocio. Este flujo pertenece a BDD. ¿Y cuál es la forma de explicar las reglas de negocio? mediante ejemlos. __Debemos incorporporar ejemplos en las conversaciones (o calaboraciones) que busca DDD__. Uno de las puntos en los que Ciaran hace más hincapié es el de dar contexto (DDD) a las reglas de negocio establecidas (BDD).

A continuación Ciaran hace un repaso bastante interesante sobre diferentes herramientas , que yo desconocía por completo, y que parecen muy interesantes, como los [Mapas de ejemplos][example-mapping] de Matt Wynne o los [Mapas de funcionalidades][feature-mapping] de John Ferguson Smart.

Con estas herramientas introduce el modelado mediante ejemplos:

> Al introducir el lenguage ubícuo en tus escenarios, tus escenarios se convierten en tu modelo de dominio de manera natural

Finalmente, Ciaran muestra un ejemplo de este modelado mediante ejemplos.

## Cruzar el rio sintiendo las piedras - Simon Wardley
[Crossing the river by feeling the stones - Simon Wardley][crossing-the-river-wardley]

Esta ha sido una de las mejores charlas que he visto últimamente. Muy amena y divertida a pesar de la advertencia que hizo Wardley acerca del número de diapositivas: ¡168!

Para ponernos en contexto, Wardley nos muestra varios ejemplos de cómo tratamos la información en la empresa: cuadrantes, secuencias de datos, etc... A continuación les añade contexto mediante mapas. Los mapas ofrecen una navegabilidad: tienen un punto de partida y permiten visualizar el contexto. Pregunta en voz alta cuáles son los mecanismos que se utilizan en las empresas... y no suelen ser los mapas.

Más adelante muestra el resultado de la investigación que lleva realizando durante años: se trata de un mapa que relaciona el tipo de software o sistemas (por ejemplo, hecho a medida, un producto existente, etc...). La visualización mediante este tipo de mapas permite ver hacia dónde se dirige la tecnología para tomar decisiones acerca dejar de invertir en sistemas anticuados, detectar la inercia de partes de nuestros sistemas, etc... 

No sabría decir por qué pero esta charla me puso en modo _brainstorming_... no tengo muy claro cómo puedo aplicar el contenido que expuso Wardley pero es una herramienta con mucho potencial, sobre todo para la porte estratégica de la compañía. Esta charla es totalmente recomendable para todo el mundo, especialmente para CEOs y otros perfiles de alto nivel.

Además de que el contenido es realmente bueno, Wardley tiene un modo de presentar la charla realmente ameno y divertido... podría haber estado horas escuchándole.

## Procesos de larga duración en DDD - Bernd Rücker
[Long running processes in DDD - Bernd Rücker][long-running-processes-ddd-rucker]

Bernd comienza con una introducción sobre los procesos de larga duración y su implementación donde habla de patrones como gestores de procesos o Sagas. También habla sobre la problemática acerca del contexto de los mensajes/eventos/comandos que gestionan estos procesos.

Más tarde plantea el uso de herramientas visuales para la configuración de flujos, y lo resume con la siguiente frase:

> El poder de los gráficos

No obstante menciona cómo se asemeja su charla con BPM y como, por norma general, los desarrolladores de software huímos de estas siglas.

Por último habla de los siete pecados de los flujos de trabajo y Java. Se centra en la poblemática de no utilizar ningún motor, comenzar con uno hecho en casa y darle de comer hasta que se convierte en un monstruo o bien utilizar una herramienta pensada para gente de negocio pero que acaban utilizando los desarrolladores, muy a su pesar.

## Black Ops DDD utilizando el Business Model Canvas - Javier Fernández
[Black Ops DDD using the Business Model Canvas - Javier Fernández][black-ops-ddd-fernandez]

Voy a traducir el abstract de mi charla, os dejo que la echéis un vistazo y saquéis vuestras propias conclusiones :)

Si estás intentada adoptar DDD en tu organización necesitarás arrastrar a la gente de negocio y si, debes esperar resistencia. Tendrás que utilizar técnicas poco convencionales para que esto pueda ocurrir.

Por suerte puedes utilizar el _Business Model Canvas_: un _framework_ popular entre gente de negacio que se utiliza para generar modelos de negocio. Esta herramienta ayuda a que la gente de negocio perciba DDD de manera menos agresiva: si conseguimos que nuestros compañeros estén más cómodos, tendremos un ambiente propenso a cambios.

Me encantaría recibir vuestros comentarios acerca de la charla, si alguien tiene tiempo y ganas, me puede encontrar en twitter: [@javierfdezg][twitter-javier-fernandez].

Esto fue todo para el primer día. En cuanto tenga lista la crónica del segundo día publicaré otro post.


[ddd-exchange-2017]: https://skillsmatter.com/conferences/8231-ddd-exchange-2017#program 
[skills-matter-talks]: https://skillsmatter.com/conferences/8231-ddd-exchange-2017#program 
[good-design-imperfect-design-evans]: https://skillsmatter.com/skillscasts/9171-good-design-is-imperfect-design

[bdd-scenarios-as-domain-models-mcnulty]: https://skillsmatter.com/skillscasts/9841-bdd-scenarios-as-domain-models

[example-mapping]: https://cucumber.io/blog/2015/12/08/example-mapping-introduction

[feature-mapping]: https://johnfergusonsmart.com/feature-mapping-a-simpler-path-from-stories-to-executable-acceptance-criteria

[crossing-the-river-wardley]: https://skillsmatter.com/skillscasts/9665-crossing-the-river-by-feeling-the-stones

[long-running-processes-ddd-rucker]: https://skillsmatter.com/skillscasts/9853-long-running-processes-in-ddd

[black-ops-ddd-fernandez]: https://skillsmatter.com/skillscasts/9935-black-ops-ddd-using-the-business-model-canvas

[twitter-javier-fernandez]: http://twitter.com/javierfdezg
