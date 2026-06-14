# Estacionamiento Inteligente
Materia: Sistemas Operativos | Periodo: 2026-Ex1 | Estado: Completado

## Equipo de trabajo
- José Hidalgo ([josehidalgoc-cpu](https://github.com/josehidalgoc-cpu))
- José Viteri ([jvit04](https://github.com/jvit04))

## Capturas / Demo
![Vista principal](docs/screenshots/04.gif)

## Funcionalidad
- [x] Funcionalidad 1: Control de ingreso y salida de vehículos con validación de cupos mediante el uso de locks (Mutex) para asegurar la integridad de datos compartidos [Commit](https://github.com/jvit04/Proyecto_Sis_EstacionamientoInteligente/commit/0d9922644f809d5c602755a64e7a3b4ec128979a)
- [x] Funcionalidad 2: Registro de historial y auditoría con tiempos exactos y cálculo de estadía por vehículo [Commit](https://github.com/jvit04/Proyecto_Sis_EstacionamientoInteligente/commit/1e0a15a1dff36a2083be547930e2c3b5563da03c)
- [x] Funcionalidad 3: Simulación concurrente que evalúa múltiples hilos ("vehículos") compitiendo por los recursos del sistema simultáneamente [Commit](https://github.com/jvit04/Proyecto_Sis_EstacionamientoInteligente/commit/af6dde6b45827c283106e731950a7f99bea77072)
- [x] Funcionalidad 4: Generación de bitácora transaccional mediante el módulo `logging` para depuración y trazabilidad [Commit](https://github.com/jvit04/Proyecto_Sis_EstacionamientoInteligente/commit/7d9531d1a3558108c8c1c9d8611906614add2f3c)

## Tecnologías
`Python 3.12` `Threading` `Logging` `Datetime`

## Ejecución
# Instrucciones paso a paso
git clone https://github.com/jvit04/Proyecto_Sis_EstacionamientoInteligente.git
cd Proyecto_Sis_EstacionamientoInteligente
# No requiere instalación de dependencias externas
python main.py

## Métricas de Progreso
| Indicador | Valor |
| --- | --- |
| Commits totales | 36 |
| Issues/PRs fusionados | 0/7 |
| Cobertura de pruebas | N/A |
| Última actualización | 2026-03-19 |

## Reflexión y Aprendizajes
- **Habilidades desarrolladas:** Diseño e implementación de sistemas concurrentes, administración de memoria compartida, y prevención de condiciones de carrera mediante programación con hilos (threads).
- **Qué funcionó bien:** Separar la lógica de negocio (entidades como Estacionamiento y Vehiculo) de la lógica de concurrencia (simulación de hilos), lo que facilitó el mantenimiento y las pruebas del código.
- **Qué se podría mejorar:** Se podría implementar la persistencia de datos en una base de datos o un sistema de archivos permanente (como JSON o CSV) para no perder el historial de vehículos y la ocupación al finalizar la ejecución del programa.

- **Conceptos clave aplicados de la materia:** Concurrencia, exclusión mutua, bloqueos (Locks/Mutex), condiciones de carrera (Race Conditions) y sincronización de procesos en sistemas operativos.
