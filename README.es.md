# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.md) | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | Español | [Français](README.fr.md) | [Deutsch](README.de.md)

Una skill de diseño UI/UX para asistentes de programación. Elige una referencia y un estilo para convertir tus requisitos en un prototipo HTML + Tailwind que puedes abrir en el navegador.

## Instalación

Ejecuta este comando desde la carpeta del proyecto:

```bash
npx skills add ducafecat/design-ui-ux
```

## Cómo usarlo

### 1. Busca referencias de diseño

Describe qué quieres crear, quién lo usará y qué pantallas necesitas. Si tienes un documento de requisitos (PRD), incluye su ruta:

```text
/design-ui-ux Diseña una interfaz móvil con el estilo de Xiaohongshu.

Referencia:
docs/prd.md
```

![Búsqueda de referencias de diseño](images/1795618228981.png)

### 2. Elige una dirección de diseño

Elige una referencia que te guste. Si ninguna encaja, pide otra selección:

```text
Muéstrame otro grupo de referencias.
```

![Selección de la dirección de diseño](images/1795618428611.png)

### 3. Crea el prototipo

Responde con el identificador de la referencia, por ejemplo:

![Selección de referencia](images/1795618786169.png)

```text
B2
```

Después, elige un estilo:

![Opciones de estilo](images/1795619134358.png)

Para elegir la primera opción, responde:

```text
1
```

Tras la confirmación, el prototipo se guarda en `design/index.html`. Ábrelo en el navegador para previsualizarlo.

![Prototipo terminado](images/1795620741606.png)

### 4. Visualiza las pantallas juntas

Pide una página con todas las pantallas juntas:

```text
Coloca las vistas de design/index.html una al lado de otra y guárdalas en design/平铺.html.
```

Archivo resultante: `design/平铺.html`

![Pantallas una al lado de otra](images/1795620965224.png)

### 5. Compara varias propuestas

¿Aún tienes dudas? Pide una página de inicio para cada estilo:

```text
Crea una página de inicio para cada opción 1, 2, 3 y 4, y guárdalas en design/compare.html.
```

Archivo resultante: `design/compare.html`

![Cuatro propuestas de diseño](images/1795619938511.png)

## Requisitos

- La instalación requiere Node.js 22.20 o posterior y npm / npx. Las páginas HTML generadas no requieren Node.js.
- La búsqueda local de datos requiere Python 3, sin paquetes de terceros. Sin Python puedes crear páginas siguiendo las pautas de diseño, pero no utilizar la búsqueda local.
- Para buscar referencias y revisar páginas necesitas un navegador con capturas de pantalla y vista previa de HTML local. Ego Lite es la opción predeterminada y requiere configurar por separado la habilidad `ego-browser`. También puedes usar otro navegador según las instrucciones de la habilidad.
- Tailwind debe compilarse durante el desarrollo. Compílalo antes de la entrega para que el HTML final pueda abrirse sin Node.js, CDN ni compilación en tiempo de ejecución.

## Comentarios y licencia

Lee [CONTRIBUTING.md](CONTRIBUTING.md) antes de proponer mejoras. Consulta [CHANGELOG.md](CHANGELOG.md) para el historial y [SECURITY.md](SECURITY.md) para problemas sensibles. Informa de errores reproducibles en [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues).

Este proyecto se distribuye bajo la [licencia MIT](LICENSE). El código, los datos, las fuentes, las imágenes y otros recursos de terceros conservan sus respectivas licencias. Consulta [NOTICE.md](NOTICE.md) para los créditos y las fuentes.
