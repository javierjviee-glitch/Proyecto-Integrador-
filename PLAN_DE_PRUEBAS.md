### Plan de Pruebas de Caja Negra (Fase III)

| ID | Acción (Entrada) | Resultado Esperado |
| :--- | :--- | :--- |
| **01** | Intentar asignar un conductor con carnet caducado a una ruta. | El sistema bloquea la asignación y lanza una alerta. |
| **02** | Registrar un sensor con temperatura de -90°C (fuera de rango físico). | El sistema descarta la lectura y marca el sensor como "Requiere Revisión". |
| **03** | Iniciar una ruta de mercancía crítica sin sensores de temperatura vinculados. | El sistema impide el despacho del vehículo por falta de monitorización obligatoria. |
| **04** | Simular una pérdida de señal GPS del vehículo por más de 10 minutos. | El sistema genera automáticamente una alerta de "Vehículo No Localizado". |
| **05** | Introducir una temperatura superior al límite máximo permitido para la carga. | El sistema dispara el protocolo de emergencia y notifica al conductor y administrador. |