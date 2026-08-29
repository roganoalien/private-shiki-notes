---
title: afectacion-paperless-20-agosto
date: 2026-08-24
tags: []
notebook: private-shiki-notes
links: []
template: null
---

# Afectación de evolución de controles de seguridad 19 Agosto

### Uso seguro de mecanismos para compartir archivos 
Aquí fue donde hubo afectacción. Con PNR y apellido se busca que exista, después de esa evaluación permite el login y con eso el uso de S3 prefirmada para subir el archivo. 

### Nueva protección para buckets de Amazon S3
Que va relacionado con el anterior

## Fechas
El ESAN fue lo que reportó el problema con los archivos con el peso. No se sabe si quitaron las políticas, no hay claridad del fallo y afectación. Hace un mes hicieron lo mismo de hacer cambios de políticas desde una cuenta externa. El 19 falló y luego volvió a funcionar sin saber realmente qué pasó o si echaron para atrás las políticas. AWS DevOps Agent les da una razón de dónde podría venir el cambio. Y dice que el cambio vino de una cuenta maestra con un ID y no se puede tener una mayor visibilidad o trazabilidad de lo que ocurrió ni si se volvió a cambiar y el viernes en la noche se solucionó pero no se sabe el por qué. Hay screenshot. Aplicaron a todas las cuentas sin seguir sus propias reglas de aplicar en un ambiente de DEV, QA y PROD. 

Este caso afectó un poco pero pasó antes otro que tumbaron el portal y afectó mucho. El equipo se dio cuenta porque estaban haciendo pruebas con SENDGRID en la noche y no se reportó nada por la hora y el jueves en la mañana dijeron que no habían subido cambios y esto en el desarrollo y después le mencionaron que si hicieron cambios. Afortunadamente no afectó un proceso crítico pero si hubiese sido hubiera generado mayor problemática. Si hubo un caso de ticket o reporte, el viernes a las 11:39am. El 20 empezó a fallar y el día viernes mandó cliente un reporte de error de ESAN. ESAN es solicitar un animal de apoyo, descargas un PDF y después de llenarlo se sube el archivo y cuando se sube se guarda en un S3. 

El otro caso de afectación de Cara a Cliente que tumbaron todo el portal y fue de un momento a otro, estaban haciendo pruebas y de repente se dejó de ver. Gracias al agente de DEVOPS de AWS que dijo quién hizo el cambio, a qué hora. Se tuvo una sesión en la que el equipo de CIBERSEGURIDAD se sorprendió que hubiesen cambios sin que el equipo de desarrollo ni los dueños de la app estuvieran al tanto. Reporte en word en mi chat sobre el error y la fecha.. del 30 de julio al 5 de agosto. Aparecía un error de acceso denegado y con eso se dieron cuenta de que alguien había modificado algo y después de investigar con el agente fue que vieron el error. El error fue provocado por una cuenta de emergencia AWSControlTowerExecution, ese rol revisa si hay algo mal y esta cuenta hizo los cambios. En la sesión NADIE SUPO QUÉ CONTESTAR, y quedó pendiente revisar quién tiene ese rol, por qué se hizo y qué más movió. Según el agente de DevOPS fue un proceso automatizado. Daba error 403, cuando ciberseguridad detecta un cambio así quitan el acceso. O sea que un proceso automatizado detectó algo QUE NADIE SABE QUÉ PASÓ, luego ciberseguridad detectó ese 403 y luego le quitó el acceso al equipo. Se solucionó con ALDO en el momento. 

El equipo de CIBERSEGURIDAD no les ha contestado, de lo que quedó pendiente de la investigación. La junta que tuvieron fue el 17 de agosto en el que se quedó pendiente la investigación. Lo que tardó del 5 de agosto al 17, fue buscar un espacio pero parte de que no se dieron cuenta fue porque ENID era quien hacia esas pruebas porque está de incapacidad. El equipo no se dio cuenta tan rápido hasta que alguien fue a hacer pruebas el portal y se dieron cuenta hasta una semana después de que sucedió el error. Este desarrollo afectado afectó en DEV porque NADA MÁS SE HIZO EN DESARROLLO, el de S3 si fue en las 3 cuentas. Si esto se hacía en producción la afectación hubiese sido gigantezca. 

Los servicios de cara a cliente, todos los modulos que terminan hacia un cliente final fueron afectados. Todo servicio que un cliente haga con Paperless se vería afectado UMR, ESAN, certificado médico. 

Ya se ha reportado muchas veces que hacen cambios sin avisar y hay afectaciones. Se debería de hacer un proceso en el que mínimo hagan cambios con un RFC y se haga listas de quiénes han sido afectado y empiecen por UN AMBIENTE. 

qPRESIONAR PARA SABER QUÉ PASÓ Y QUIÉN FUE sobre el error anterior del 5 de agosto. CIBERSEGURIDAD iba a investigar de quién es esa cuenta. Manejarlo como que no fue exactamente ellos o si fue devops o infra o quien.