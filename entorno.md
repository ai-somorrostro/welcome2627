# Instalación del un entorno de desarrollo

## Objetivo

Instalar y dejar operativo un entorno de desarrollo Linux completo, elegido y configurado por el alumno, con las herramientas necesarias para trabajar con Python y Node.js desde terminal. Las demostraciones y entregas se realizarán en terminal.

## Requisitos previos

- Equipo con Windows, macOS o Linux.
- Al menos 25 GB libres de disco y 4 GB de RAM disponibles para la máquina/entorno Linux.
- Conexión a internet.
- Permisos de administrador en el equipo.

## Paso 1 — Elegir el método de instalación

El alumno elige **uno** de los siguientes métodos para tener Linux funcionando:

- **WSL** (Windows Subsystem for Linux)
- **Máquina virtual** (VirtualBox, VMware o similar)
- **Dual boot** (Linux instalado junto al sistema operativo actual)

## Paso 2 — Elegir la distribución

El alumno elige libremente la distribución Linux (por ejemplo Ubuntu, Debian, Fedora, Arch, openSUSE, etc.).

Requisito: la distribución debe poder instalarse tanto con **entorno gráfico (GUI)** como con acceso a **terminal**, aunque el uso durante las demos y la evaluación será únicamente por terminal.

## Paso 3 — Instalar el software base

Sobre el entorno Linux ya instalado, debe quedar disponible lo siguiente:

| Herramienta | Descripción |
|---|---|
| Python 3.12 | Intérprete de Python |
| uv | Gestor de paquetes y entornos de Python |
| Node.js | Entorno de ejecución de JavaScript |
| opencode | Herramienta de línea de comandos |
| git | Control de versiones |

### Verificación

Comprobar la instalación con:

```bash
python3.12 --version
uv --version
node --version
opencode --version
git --version
```

Las cinco comprobaciones deben devolver una versión sin errores.

## Paso 4 — Recuperación ante fallos

El entorno debe poder recuperarse si falla, sin perder la configuración. Según el método elegido en el Paso 1:

- **WSL**: exportar la distribución con `wsl --export` tras la instalación del software base.
- **VirtualBox/VMware**: crear una snapshot de la máquina virtual una vez completada la instalación.
- **Dual boot**: disponer de un mecanismo de backup del sistema (imagen de disco, Timeshift, o similar) y de un medio de arranque (USB live) para reinstalar o restaurar si el sistema deja de arrancar.

Se debe documentar qué mecanismo de recuperación se usó y cómo se restaura el entorno a partir de él.

## Entrega

- Capturas o registro (terminal) de las cinco verificaciones del Paso 3.
- Descripción breve del método (Paso 1) y la distribución (Paso 2) elegidos.
- Descripción del mecanismo de recuperación (Paso 4) y evidencia de que existe (snapshot, export, backup).

## Criterios de evaluación

- [ ] Entorno Linux instalado y accesible por terminal
- [ ] Python 3.12 instalado y verificado
- [ ] uv instalado y verificado
- [ ] Node.js instalado y verificado
- [ ] opencode instalado y verificado
- [ ] git instalado y verificado
- [ ] Mecanismo de recuperación definido y verificado
