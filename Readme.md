<h1><img align="left" width="128px" alt="." src="./assets/branding/logo-main-color.svg"> RQT2 Components </h1>

Sistema de diseño y libería de componentes base para **[RQT2](https://github.com/RQT2)**. Contine los recursos y estilos compartidos necesariso para todo el front-end de la IDE.

> [!CAUTION]
> Al modificar un recurso aquí, los cambios se reflejan en todo el proyecto.

## Contenido

```text
./
├── assets/
│   ├── branding/       # Logo
│   ├── icons/          # Iconos de acciones
│   └── fonts/          # Archivos de fuentes
├── styles/
│   ├── themes/         # Archivos .qss
│   └── palette.json    # Definición de colores
├── releases/           # Capturas de pantalla e imágenes
└── README.md
```

## Logo

`./assets/branding`

<img align="left" width="128px" alt="." src="./assets/branding/logo-main-color.svg">
<img align="left" width="128px" alt="." src="./assets/branding/logo-main-dark.svg">
<img align="left" width="128px" alt="." src="./assets/branding/logo-main-light.svg">

---
---
---
---
---

### Archivos

* `logo.`, `template.svg`: Archivos base para modificación.
* `logo-main-.`: Isotipos SVG generados a partir de `template.svg` para iconos medianos y grandes.
* `symbolic-.`: Isotipos SVG generados a partir de `template.svg` para iconos representativos/pequeños.
* `icon-`: Iconos PNG generados a partir de `logo-main-.` y `symbolic-.`.

## Paleta de colores

### Tema claro

| Rol        | Color |
| :----------|-------|
|Fondo       |![#ffffff](https://placehold.co/16x16/ffffff/ffffff.png) `#ffffff`|
|Primer plano|![#000000](https://placehold.co/16x16/000000/000000.png) `#000000`|
|Azul        |![#0090ff](https://placehold.co/16x16/0090ff/0090ff.png) `#0090ff`|
|Verde       |![#068989](https://placehold.co/16x16/068989/068989.png) `#068989`|
|Purpura     |![#c60184](https://placehold.co/16x16/c60184/c60184.png) `#c60184`|
|Rojo        |![#ff4f5e](https://placehold.co/16x16/ff4f5e/ff4f5e.png) `#ff4f5e`|
|Naranja     |![#e5a436](https://placehold.co/16x16/e5a436/e5a436.png) `#e5a436`|

### Tema oscuro

| Rol        | Color |
| :----------|-------|
|Fondo       |![#000000](https://placehold.co/16x16/000000/000000.png) `#000000`|
|Primer plano|![#ffffff](https://placehold.co/16x16/ffffff/ffffff.png) `#ffffff`|
|Azul        |![#0090ff](https://placehold.co/16x16/0090ff/0090ff.png) `#0090ff`|
|Verde       |![#3fe1b0](https://placehold.co/16x16/3fe1b0/3fe1b0.png) `#3fe1b0`|
|Purpura     |![#fe4aa3](https://placehold.co/16x16/fe4aa3/fe4aa3.png) `#fe4aa3`|
|Rojo        |![#ff4f5e](https://placehold.co/16x16/ff4f5e/ff4f5e.png) `#ff4f5e`|
|Naranja     |![#ffbd4f](https://placehold.co/16x16/ffbd4f/ffbd4f.png) `#ffbd4f`|

## Estilos y Temas

`./styles`

* **palette.json**: Diccionario main de colores para uso en `Qt`>`Pyside6`.
* **themes/**: Temas de colores `.qss`.

## Tipografía

`./assets/fonts`

<img align="left" width="18%" alt="." src="./releases/fonts/nunito-sans.png">
<img align="left" width="18%" alt="." src="./releases/fonts/ubuntu-mono.png">
<img align="left" width="16%" alt="." src="./releases/fonts/ubuntu-mono-nerd-font.svg">

| Fuente | Uso |
| :----- | --- |
| **Nunito Sans** | Interfaz (UI). |
| **Ubuntu Mono** | Código/Terminal. |
| **Nerd Fonts** | Iconos. |

## Iconos

`./assets/branding`

Iconos simbolicos: En combinación con [Nerd Fonts](https://www.nerdfonts.com/cheat-sheet) son usados para las acciones de la IDE.

| Icono | Nombre | Rol |
| :-----|--------|-----|
| <img align="left" width="22px" alt="." src="/assets/icons/3d/default.svg"> | `3d` | Acceso directo a RViz. |
| <img align="left" width="22px" alt="." src="/assets/icons/emulator/default.svg"> | `emulator` | Acceso directo a `gz sim` (Simulador de Gazebo). |
| <img align="left" width="22px" alt="." src="/assets/icons/widgets/default.svg"> | `widgets` | Acceso directo a rqt. |
| <img align="left" width="22px" alt="." src="/assets/icons/daemon/default.svg"> | `daemon` | Reinicia el proceso de ROS2. |
| <img align="left" width="22px" alt="." src="/assets/icons/bug/default.svg"> | `bug` | Obtener backtrace de nodos usando `gdb`. |
| <img align="left" width="22px" alt="." src="/assets/icons/compile/default.svg"> | `compile` | Crea el espacio de trabajo de ROS2: Primero resuelve dependencias con `rosdep install` para construir el espacio de trabajo con `colcon build` y finalmente cargar el overlay generado. |
| <img align="left" width="22px" alt="." src="/assets/icons/clean/default.svg"> | `clean` | Elimina los directorios `build`, `install` y `log` creados por `colcon build`. |
| <img align="left" width="22px" alt="." src="/assets/icons/load/default.svg"> | `load` | Carga el overlay `install/local_setup.$SHELL` generado por `colcon build`. |
| <img align="left" width="22px" alt="." src="/assets/icons/settings/default.svg"> | `settings` | Abre un fomulario para editar archivos de configuración de paquetes de ROS2 como **package.xml** o **CMakeList.txt**. |
| <img align="left" width="22px" alt="." src="/assets/icons/list/default.svg"> | `list` | Abre la ventana de nodos y topicos en ejecución. |
| <img align="left" width="22px" alt="." src="/assets/icons/launch/default.svg"> | `launch` | Abre la ventana de nodos y lanzadores disponibles. |
| <img align="left" width="22px" alt="." src="/assets/icons/run/default.svg"> | `run` | Ejecuta nodos o lanzadores. |
| <img align="left" width="22px" alt="." src="/assets/icons/stop/default.svg"> | `stop` | Detiene nodos o lanzadores en ejecución. |
| <img align="left" width="22px" alt="." src="/assets/icons/unsynchronize/default.svg"> | `synchronize` | Se conecta a topicos como publicador o subscriptor. |
| <img align="left" width="22px" alt="." src="/assets/icons/synchronize/default.svg"> | `unsynchronize` | Se desconecta de topicos anteriormente conectado desde la IDE. |
| <img align="left" width="22px" alt="." src="/assets/icons/new/default.svg"> | `new` | Crea elementos nuevos (paquetes/lanzadores/nodos). |
| <img align="left" width="22px" alt="." src="/assets/icons/nodes/default.svg"> | `nodes` | Abre ventana `node-graph` (parecido a `rqt_graph`). |
| <img align="left" width="22px" alt="." src="/assets/icons/params/default.svg"> | `params` | Abre un fomulario para editar parametros de nodos (`ros2 param set`). |
| <img align="left" width="22px" alt="." src="/assets/icons/record/default.svg"> | `record` | Graba los datos publicados sobre un topico con `ros2 bag`. |
| <img align="left" width="22px" alt="." src="/assets/icons/play/default.svg"> | `play` | Reproduce los datos grabados de un topico con `ros2 bag`. |
| <img align="left" width="22px" alt="." src="/assets/icons/ssh/default.svg"> | `ssh` | Abre un formulario para establecer una conexión SSH. |
| <img align="left" width="22px" alt="." src="/assets/icons/teleop/default.svg"> | `teleop` | Abre un formulario para enviar instrucciones de control manual con `ros2 teleop`. |
| <img align="left" width="22px" alt="." src="/assets/icons/close/default.svg"> | `close` | Window button: Cerrar ventana. |
| <img align="left" width="22px" alt="." src="/assets/icons/minimize/default.svg"> | `maximize` | Window button: Maximizar ventana. |
| <img align="left" width="22px" alt="." src="/assets/icons/maximize/default.svg"> | `minimize` | Window button: Minimizar ventana. |
| <img align="left" width="22px" alt="." src="/assets/icons/restore/default.svg"> | `restore` | Window button: Restaura el tamaño de la ventana. |
| <img align="left" width="22px" alt="." src="/assets/icons/tab/default.svg"> | `split` | Window button: Abre una terminal. |
| <img align="left" width="22px" alt="." src="/assets/icons/split/default.svg"> | `tab` | Window button: Cierra la terminal. |
