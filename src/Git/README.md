[**Volver al inicio**](../../)

# Introducción a Git

## ¿Qué es Git?

**[Git](https://git-scm.com/)** es un **sistema de control de versiones distribuido** que permite a varios desarrolladores trabajar en un proyecto *al mismo tiempo* sin sobrescribir el trabajo de los demás. Git facilita el *seguimiento de los cambios en el código*, *la colaboración entre equipos*, y *la reversión a versiones anteriores* si es necesario.

## Configuración Inicial y Autenticación

Antes de empezar a usar Git, es necesario configurarlo con tu **nombre de usuario** y **correo electrónico**, que se utilizarán para **identificar tus commits**.

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@example.com"
```

Si estás trabajando con **GitHub** o cualquier otro servicio que requiera autenticación, también necesitarás iniciar sesión. Para ello, generalmente se utiliza un token de acceso personal (PAT) en lugar de la contraseña de tu cuenta.

1. **Generar un Token de Acceso Personal**:
   - Ve a [GitHub](../GitHub/) > Configuración > "Developer settings" > "Personal access tokens".
   - Genera un nuevo token con los permisos necesarios.

2. **Iniciar Sesión con el Token**:
   - Cuando Git te pida las **credenciales**, usa tu **nombre de usuario** y, en lugar de la contraseña, pega el **token de acceso personal**.

## Comandos Básicos de Git

### Inicializar un Repositorio

```bash
git init
```
Este comando inicializa un nuevo repositorio de Git en tu directorio actual.

### Clonar un Repositorio

```bash
git clone url-del-repositorio
```
Clona un repositorio remoto a tu máquina local.

### Ver el Estado del Repositorio

```bash
git status
```
Muestra el estado de los archivos en tu repositorio, como cambios sin confirmar y archivos sin seguimiento.

### Añadir Archivos al Área de Staging

```bash
git add nombre-del-archivo
```
Añade un archivo específico al área de staging. Para añadir todos los archivos, usa `git add .`.

### Hacer un Commit

```bash
git commit -m "Mensaje descriptivo del commit"
```
Guarda los cambios en el historial del repositorio con un mensaje que describa lo que se ha hecho.

### Ver el Historial de Commits

```bash
git log
```
Muestra el historial de commits en el repositorio.

### Crear una Nueva Rama

```bash
git branch nombre-de-la-rama
```
Crea una nueva rama para trabajar en ella sin afectar la rama principal.

### Cambiar de Rama

```bash
git switch nombre-de-la-rama
```
Cambia de una rama a otra.

### Fusionar Ramas

```bash
git merge nombre-de-la-rama
```
Funde la rama especificada con la rama en la que te encuentras actualmente.

### Subir Cambios a un Repositorio Remoto

```bash
git push origin nombre-de-la-rama
```
Envía los commits de tu rama local al repositorio remoto.

### Actualizar tu Repositorio Local con Cambios Remotos

```bash
git pull
```
Descarga y fusiona los cambios del repositorio remoto en tu rama local.

## Resumen

Estos son solo algunos de los comandos básicos que usarás frecuentemente en Git. Recuerda que siempre puedes usar `git --help` para obtener más información sobre cualquier comando o consultar la [documentación oficial](https://git-scm.com/doc).
