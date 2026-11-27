# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.md) | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | Español | [Français](README.fr.md) | [Deutsch](README.de.md)

Crea prototipos UI/UX con HTML + Tailwind. Busca referencias de diseño, elige un estilo y genera páginas que puedas previsualizar en el navegador.

## Instalación

Instala con npx, preferiblemente en tu proyecto:

```bash
npx skills add ducafecat/design-ui-ux
```

## Cómo usarlo

### 1. Busca referencias de diseño

Prepara un documento de requisitos del producto (PRD) que explique qué quieres crear, para quién y qué pantallas necesitas. Después, escribe:

```text
/design-ui-ux Diseña una interfaz móvil con el estilo de Xiaohongshu.

Referencia:
docs/prd.md
```

![Búsqueda de referencias de diseño](images/1795618228981.png)

### 2. Elige una dirección de diseño

Escoge la opción que prefieras. Si ninguna encaja, pide más propuestas:

```text
Muéstrame otro grupo de referencias.
```

![Selección de la dirección de diseño](images/1795618428611.png)

### 3. Crea el prototipo

Introduce el identificador de la referencia elegida, por ejemplo B2. Después, elige uno de los estilos propuestos; por ejemplo, la opción 1.

![Selecciona una referencia y revisa los estilos propuestos.](images/1795618786169.png)

```text
B2
```

![Selecciona una referencia y revisa los estilos propuestos.](images/1795619134358.png)

Ejemplo para elegir la opción 1:

```text
1
```

Tras la confirmación, el prototipo se guarda en `design/index.html`. Ábrelo en el navegador para previsualizarlo.

![Prototipo terminado](images/1795620741606.png)

### 4. Visualiza las pantallas juntas

Para ver las pantallas una al lado de otra, escribe:

```text
Coloca las vistas de design/index.html una al lado de otra y guárdalas en design/平铺.html.
```

Archivo resultante: `design/平铺.html`

![Pantallas una al lado de otra](images/1795620965224.png)

### 5. Compara varias propuestas

Si no sabes qué estilo elegir, crea una página de inicio por estilo y compáralas:

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

## Comentarios, mantenimiento y licencia

Lee [CONTRIBUTING.md](CONTRIBUTING.md) antes de proponer mejoras. Consulta [CHANGELOG.md](CHANGELOG.md) para el historial y [SECURITY.md](SECURITY.md) para problemas sensibles. Informa de errores reproducibles en [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues).

El proyecto todavía no tiene una licencia definida. Comprueba los permisos pertinentes antes de usarlo o redistribuirlo. Antes de publicarlo, el mantenedor debe verificar las fuentes, los derechos de redistribución y las licencias del código y los datos. Indicar una fuente no concede por sí solo permiso para redistribuir. Consulta el [aviso de procedencia](NOTICE.md).
