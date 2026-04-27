### Plan de Pruebas de Caja Negra (Fase III)


Este documento detalla la estrategia de validación para el sistema de Logística Crítica, asegurando que los requisitos de negocio se cumplan sin fallos.

## 1. Pruebas de Caja Negra (Funcionales)
Estas pruebas se centran en las entradas y salidas del sistema, sin analizar el código interno, para asegurar que las reglas de negocio funcionan.

| ID | Escenario de Prueba | Entrada (Input) | Resultado Esperado |
|:---|:---|:---|:---|
| **TC-01** | Validación de Seguridad | Asignar conductor con carnet caducado. | El sistema bloquea la asignación y muestra "Carnet Invalido". |
| **TC-02** | Rango de Sensores | Lectura de sensor de temperatura a -90°C. | El sistema descarta la lectura por estar fuera del rango físico. |
| **TC-03** | Integridad de Ruta | Iniciar ruta crítica sin sensores vinculados. | Error: "No se puede iniciar ruta crítica sin monitoreo térmico". |
| **TC-04** | Capacidad de Carga | Cargar 5000kg en vehículo de 3500kg. | Alerta de sobrepeso y bloqueo del despacho de mercancía. |
| **TC-05** | Alerta de Emergencia | Temperatura sube de 5°C a 12°C en ruta. | Notificación push inmediata al Conductor y Administrador. |

## 2. Diseño de Pruebas Unitarias (Lógica)
Representación de la lógica que se implementará para validar los métodos críticos.

### Test: `validarCapacidadVehiculo()`
**Objetivo:** Verificar que el peso no exceda el límite técnico.
```pseudo
INICIO TEST_CAPACIDAD
    peso_mercancia = 4000
    limite_vehiculo = 3500
    SI (peso_mercancia > limite_vehiculo)
        RESULTADO = "FALLO_VALIDACION" (Correcto)
    SINO
        RESULTADO = "EXITO"
FIN TEST