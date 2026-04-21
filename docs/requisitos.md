# Requisitos Funcionales y No Funcionales 

## Requisitos Funcionales (Lo que hace el sistema)
* **Gestión de Perfiles**: El sistema debe permitir el alta y baja de conductores, verificando la vigencia de su carnet de conducir.
* **Control de Flota**: Registro técnico de vehículos y vinculación con dispositivos de sensor.
* **Monitorización en Tiempo Real**: Seguimiento de rutas activas con actualización constante de la ubicación y estado de la carga.
* **Protocolo de Alerta Térmica**: Generación automática de avisos críticos si los sensores detectan temperaturas fuera del rango de seguridad para mercancías críticas.

## Requisitos No Funcionales (Cómo es el sistema)
* **Seguridad**: Solo el Administrador tiene permisos para modificar rutas y asignar conductores.
* **Disponibilidad**: El sistema de control debe estar activo y funcionando durante todo el trayecto sin interrupciones para no perder el rastro de la cadena de frío.
* **Escalabilidad**: La arquitectura debe permitir añadir nuevos sensores sin tumbar el sistema principal.