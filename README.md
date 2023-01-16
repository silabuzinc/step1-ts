# Pre-requisitos

- Tener instalado node.
- Tener instalado algún **package manager**: [`npm`](https://www.npmjs.com/), [`yarn`](https://yarnpkg.com/), [`pnpm`](https://pnpm.io/)

# Instalación

Los comandos a listar son con `npm` (pero puede usar algún otro package manager)

```bash
npm install
```

Verificando la versión instalada de Typescript

```bash
npx tsc -v
```

## NPX

`npx` (Node Package Execute) viene con `npm` (si tienes una versión mayor a la 5.2.0).

Es un ejecutor de paquetes `npm` que puede ejecutar cualquier paquete que desee desde el registro `npm` sin siquiera instalar ese paquete.

- `npm` es una herramienta usada para instalar paquetes.
- `npx` es una herramienta usada para ejecutar paquetes.

## Instalación global de Typescript

⚠️ En caso desee instalar typescript de manera global:

```bash
npm install -g typescript
```

Verificando versión instalada

```bash
tsc -v
```

# Generando tsconfig.json

Ejecutar el siguiente comando:

```bash
npx tsc -init
```

## Opciones activadas en tsconfig:

Dentro de las líneas del archivo tsconfig, activar las siguientes:

```json
/* Modules */
"rootDir": "./src",

/* Emit */
"outDir": "./dist",
"removeComments": true,
```

# Experimentación

Ya no será necesario mapear cada archivo, ahora bastará ejecutar `npx tsc`:

```bash
npx tsc
```