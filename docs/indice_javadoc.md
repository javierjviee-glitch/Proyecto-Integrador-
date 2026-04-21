# Índice de Documentación Técnica (Javadoc) 

## Paquete: `com.logistica.model`
* **Vehiculo**: Representación de la unidad de transporte y su capacidad de carga.
* **Conductor**: Gestión de credenciales y disponibilidad del personal.
* **Ruta**: Lógica de trayectos, tiempos estimados y estados (activa/finalizada).

## Paquete: `com.logistica.sensors`
* **Sensor**: Clase base para la captura de datos térmicos.
* **Alerta**: Lógica de disparo de eventos cuando se detectan cambios perjudiciales por la temperatura en la mercancía.

## Paquete: `com.logistica.core`
* **ValidadorRuta**: Contiene el método `validarRuta()` para asegurar que todos los parámetros de seguridad se cumplen antes de salir.