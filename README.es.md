# Bindings de Control de CMDR Buanzox para Elite Dangerous

Datos publicos para el tutorial de CarrierTV sobre el perfil de control de CMDR Buanzox para Elite Dangerous.

Este es el unico archivo traducido del repositorio. Las tablas de datos, la documentacion detallada, los nombres de archivo y los nombres tecnicos de los bindings quedan en ingles para mantener compatibilidad y evitar duplicacion.

Este repositorio contiene solo datos aptos para publicacion: archivos `.binds` instalables, tablas revisadas de controles y documentacion. No contiene videos fuente, capturas, hojas de revision, carpetas locales, identificadores personales ni videos generados.

## Presets

- `binds/BUANZOFAOFF.binds`: perfil nativo DualShock4. Proba este primero si Elite Dangerous detecta el control como `DualShock4`.
- `binds/BUANZOFAOFFXINPUT.binds`: fallback XInput. Usalo si Steam Input o Windows exponen el control como un gamepad estilo Xbox.

## Instalacion

1. Cerra Elite Dangerous.
2. Descarga el archivo `.binds` que quieras usar.
3. Copialo a:

```text
%LOCALAPPDATA%\Frontier Developments\Elite Dangerous\Options\Bindings
```

4. Inicia Elite Dangerous.
5. Anda a `Options > Controls`.
6. Selecciona `BUANZOFAOFF` o `BUANZOFAOFFXINPUT`.
7. Aplica el preset.

El repositorio de GitHub es la ubicacion publica principal para descargar los archivos y revisar la lista completa de bindings.

## Datos

- [data/canonical_bindings.tsv](data/canonical_bindings.tsv): tabla canonica revisada.
- [data/canonical_bindings.json](data/canonical_bindings.json): la misma tabla en formato JSON.
- [data/export_candidates.tsv](data/export_candidates.tsv): filas mapeadas a acciones XML de Frontier para generar los `.binds`.

Las notas de columnas y limitaciones estan en [data/README.md](data/README.md), en ingles.

## Contexto del Tutorial

El video explica el perfil como una gramatica de control, no solo como una lista de botones:

- Alternate Controls es la capa normal de vuelo.
- El modo regular se conserva para trabajo temporal de thrust lateral.
- Flight Assist Off se trata como una postura deliberada de combate.
- Las familias de botones ayudan a memorizar: Cross/X para extremos y targeting, Circle para aproximacion/utilidades, Square para armas/paneles, Triangle para viaje/mapas/estado de nave.

## Lista Completa de Bindings

Esta es la lista practica de botones asignados segun las tablas publicas. Los archivos TSV y JSON tambien incluyen filas en blanco, defaults, ejes y datos de auditoria.

### Capas de Vuelo y Movimiento

| Accion | Binding |
| --- | --- |
| Yaw izquierda | `L1` |
| Yaw derecha | `R1` |
| Toggle Alternate Controls | `CIRCLE+D-PAD LEFT` |

### Doctrina de Throttle

| Accion | Binding |
| --- | --- |
| Velocidad -100% | `X+L1` |
| Velocidad 0% | `L1+R1` |
| Velocidad 25% | `SQUARE+D-PAD DOWN` |
| Velocidad 50% | `SQUARE+R1` |
| Velocidad 75% | `CIRCLE` |
| Velocidad 100% | `X+R1` |

### Combate y Flight Assist

| Accion | Binding |
| --- | --- |
| Primary fire | `R2` |
| Secondary fire | `L2` |
| Deploy hardpoints | `SQUARE` |
| Cycle next fire group | `SQUARE+L1` |
| Toggle Flight Assist | `TRIANGLE+R1` |
| Engine boost | `CIRCLE+L1` |
| Silent running | `TRIANGLE+L1` |
| Toggle orbit lines | `R3` |

### Targeting

| Accion | Binding |
| --- | --- |
| Select target ahead | `X` |
| Cycle next target | `X+D-PAD LEFT` |
| Select highest threat | `X+D-PAD DOWN` |
| Select wingman's target | `X+D-PAD RIGHT` |
| Cycle next subsystem | `X+D-PAD UP` |
| Target next system in route | `CIRCLE+R1` |

### Energia y Utilidades de Nave

| Accion | Binding |
| --- | --- |
| Energia a motores | `D-PAD UP` |
| Energia a armas | `D-PAD RIGHT` |
| Energia a sistemas | `D-PAD LEFT` |
| Balancear distribucion | `D-PAD DOWN` |
| Cargo scoop | `CIRCLE+D-PAD UP` |
| Landing gear | `CIRCLE+D-PAD DOWN` |
| Luces de nave | `TRIANGLE+R3` |
| Night vision | `TRIANGLE+L3` |

### Paneles, Mapas y Headlook

| Accion | Binding |
| --- | --- |
| Panel externo | `SQUARE+D-PAD LEFT` |
| Panel de comms | `SQUARE+D-PAD UP` |
| Panel interno | `SQUARE+D-PAD RIGHT` |
| Galaxy map | `TRIANGLE+D-PAD LEFT` |
| System map | `TRIANGLE+D-PAD RIGHT` |
| Supercruise | `TRIANGLE+D-PAD DOWN` |
| Hyperspace jump | `TRIANGLE+D-PAD UP` |
| Switch cockpit mode | `TOUCHPAD` |
| Enter FSS mode | `TOUCHPAD` |
| Headlook | `R3+L3` |

Nota sobre el panel inferior/role panel: `SQUARE+D-PAD DOWN` parece el combo esperado para completar la familia de paneles, pero en este perfil no abre el panel inferior; configura la velocidad al 25%. Para usar el panel inferior, activa headlook con `R3+L3`, mira hacia abajo hasta que el panel haga foco, y volve a presionar `R3+L3` para salir. Si queres un atajo directo, `SQUARE+X` es un candidato limpio para agregar manualmente, pero no esta incluido en los `.binds` publicados.

## Limite de Privacidad

Este repo fue privado mientras se revisaba, pero todo lo que contiene debe tratarse como publico. Antes de publicar datos nuevos, hay que revisar [RELEASE_CHECKLIST.md](RELEASE_CHECKLIST.md) y [docs/privacy-checklist.md](docs/privacy-checklist.md).
