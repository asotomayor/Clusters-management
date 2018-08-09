# Clusters-management
YARN capacity-scheduler configuration
Actividad correspondiente al módulo 5 del Máster de Big Data y Business Analytics.
La actividad consiste en configurar las colas desde Ambari (distribución de Hadoop Hortonworks) y obtener el archivo capacity.scheduler.xml con las propiedades configuradas de acuerod al suigiente caso supuesto:

La estructura de colas a implementar es:
1. Todas las colas estarán activas excepto la cola redessociales que se encontrará parada.
2. El número máximo de aplicaciones concurrentes en el cluster son 950.
3. Todos los trabajos del grupo direccion irán siempre a la cola online y no se les permitirá que los envíen a otra cola.

root
- desarrollo: Capacidad:20; Máxima Capacidad:50; User-limit:2; Administrador cola y jobs : javier; Usuarios cola: javier y el grupo programadores.
- marketing: Capacidad:70; Máxima Capacidad:100
    - online: Capacidad:50; Máxima Capacidad:70; Límite capacidad usuario: La capacidad de la cola; Administrador cola: maria;         Administrador jobs: susana e isabel;Usuarios cola: grupo online
    - redessociales: Capacidad:30; Máxima Capacidad: 50; Administrador cola y jobs: grupo redes; Usuarios cola: grupo redes.
    - otros: Capacidad:20; Máxima Capacidad: La misma que la capacidad; Máximo aplicaciones:40; Administrador cola: juan; Administrador jobs: miguel; Usuarios_cola: miguel y juan y grupo marketing.
- default: Capacidad:10; Máxima Capacidad:30; Límite capacidad usuario:El doble de la capacidad de la cola; Porcentaje mínimo usuario:25;
