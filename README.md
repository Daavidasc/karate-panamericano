# Karate Panamericano

> Juego de pelea por turnos en consola, hecho en C++ con arte en bloques ANSI. Elige un país y pelea por el podio de los Juegos Panamericanos.

## Sobre el proyecto

**Karate Panamericano** es un juego de karate en consola ambientado en los Juegos Panamericanos. Eliges uno de 10 países, personalizas tu karateka con los colores de su bandera y avanzas por un torneo de eliminación directa hasta el podio.

## Características

- 10 países jugables: USA, Chile, Brasil, Colombia, México, Perú, Canadá, Argentina, Bolivia y República Dominicana.
- Combate por turnos: **Atacar** (puñetazo o patada) o **Defenderse**.
- Sistema de resistencia, empuje y recuperación según el tipo de golpe.
- 10 % de probabilidad de que un ataque falle.
- Penalidades: acumular 3 te descalifica.
- Jueces con puntuación aleatoria.
- Torneo completo: **Cuartos de final → Semifinal → Final → Podio**.
- Gráficos en consola con caracteres de bloque y colores ANSI de 256 tonos (escenarios por ronda, karatecas animados con pose, golpe, patada y defensa).
- Menú con instrucciones y créditos.

## Cómo se juega

| Dónde | Tecla | Acción |
|---|---|---|
| Menú principal | `1` | Jugar |
| | `2` | Instrucciones |
| | `3` | Créditos |
| | `0` | Salir |
| Tu turno | `1` | Atacar |
| | `2` | Defenderse |
| Al atacar | `1` | Puñetazo (menos daño, empuja poco) |
| | `2` | Patada (más daño, empuja más) |

Una defensa exitosa reduce el daño recibido, pero cada tipo de ataque tiene su costo de recuperación. Gana quien deje al rival sin resistencia o con 3 penalidades.

## Requisitos

- Windows
- Visual Studio con soporte de C++ (TODO: indicar versión usada)
- Una terminal con soporte de **colores ANSI de 256 tonos** (secuencias de escape VT). Recomendado: **[Windows Terminal](https://aka.ms/terminal)** (Windows 10/11). El `cmd.exe` clásico (conhost) puede mostrar los códigos de color como texto en lugar de colores.
- Tamaño de al menos **190 columnas × 45 filas** (maximiza la ventana o reduce la fuente con `Ctrl` + rueda del mouse).
- Fuente monoespaciada con soporte de caracteres de bloque (por ejemplo **Cascadia Mono** o **Consolas**).

## Cómo ejecutarlo

1. Abre el proyecto en Visual Studio (`.sln` / `.cpp`).
2. Compila en modo **Release** (o Debug).
3. Ejecuta el `.exe` **desde Windows Terminal** (no desde el `cmd` clásico) y maximiza la ventana antes de empezar.

## Estructura

```
.
├── main.cpp        # TODO: ajustar al nombre real del archivo
└── README.md
```

## Limitaciones conocidas

- Solo funciona en Windows (usa `conio.h` y colores de consola).
- Requiere una consola grande; en ventanas pequeñas el arte se desfasa.
