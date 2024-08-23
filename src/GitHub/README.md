[**Volver al inicio**](../../)

# Guía de Introducción a GitHub

## 1. ¿Qué es GitHub?

[**GitHub**](https://github.com/) es una **plataforma** basada en la web que **utiliza [Git](../Git/)** como sistema de control de versiones. GitHub permite a los desarrolladores **alojar sus repositorios de código**, **colaborar en proyectos**, y gestionar versiones de manera eficiente. Aunque Git y GitHub *están estrechamente relacionados*, **no son lo mismo**.

## 2. Diferencias entre Git y GitHub

- **Git**: Es un sistema de control de versiones distribuido que permite a los desarrolladores seguir el historial de cambios en su código, revertir a versiones anteriores y colaborar en un proyecto sin sobrescribir el trabajo de los demás. **Git se utiliza localmente en tu computadora**.

- **GitHub**: Es una plataforma que facilita el uso de Git al ofrecer un lugar centralizado donde los desarrolladores pueden alojar y compartir sus repositorios de Git. Además, GitHub proporciona **herramientas adicionales** para la colaboración, como **issues**, **pull requests**, y **revisiones de código**.

En resumen, **Git** es la **herramienta de control de versiones**, mientras que **GitHub** es el **servicio que aloja repositorios** y **facilita la colaboración** entre desarrolladores.

## 3. Fork vs. Clone

### 3.1. ¿Qué es un Fork?

Un **Fork** es una **copia de un repositorio** que se realiza en la **cuenta personal** de GitHub de un usuario. El **propósito** de un fork es **crear una versión independiente** del proyecto original, permitiendo al usuario **realizar cambios sin afectar el repositorio original**. Los forks son útiles cuando quieres **contribuir a un proyecto pero no tienes permisos para modificar** el repositorio principal directamente.

**Ejemplo de uso de Fork:**

1. Encuentras un proyecto interesante en **GitHub** y quieres **contribuir**.
2. Haces un **fork** del proyecto para **crear una copia en tu cuenta** de GitHub.
3. Realizas **cambios en tu copia** del repositorio.
4. Si tus cambios son útiles, puedes enviar un **pull request** para que los dueños del repositorio original revisen y, eventualmente, **integren** tus cambios.

### 3.2. ¿Qué es un Clone?

Un **Clone** es una **copia completa de un repositorio** ***(incluyendo todo su historial de commits)*** que se realiza en **tu máquina local**. A diferencia de un **fork**, que es una **copia en la nube**, un **clone es local** y te permite trabajar en el **código en tu computadora**.

**Ejemplo de uso de Clone:**

1. Quieres trabajar en un proyecto existente.
2. Clonas el repositorio en tu **máquina local** usando el comando `git clone`.
3. Trabajas en el **código localmente**.
4. **Si tienes permisos**, puedes enviar tus cambios de vuelta al repositorio remoto usando `git push`. **Si no tienes permisos**, podrías enviar tus cambios a tu fork y luego hacer un **pull request**.

```bash
# Comando para clonar un repositorio
git clone https://github.com/usuario/repositorio.git
```
[Aprender acerca de Git](../Git/)

## 4. El Valor del Software Libre

El **Software libre** y abierto es fundamental para la **colaboración en la comunidad** de software. Aquí hay algunas razones por las que el código libre es valioso:

- **Colaboración Global**: Permite a desarrolladores de todo el mundo trabajar juntos en proyectos, aportando diversas perspectivas y habilidades.
  
- **Aprendizaje y Educación**: El código abierto permite a los nuevos desarrolladores aprender de proyectos reales, estudiar cómo otros resuelven problemas y aplicar esos conocimientos en sus propios proyectos.

- **Transparencia y Confianza**: El código abierto permite a los usuarios ver exactamente cómo funciona el software, lo que puede generar confianza al saber que el código ha sido revisado y aprobado por otros.

- **Innovación Acelerada**: Al permitir que cualquiera pueda contribuir, el código abierto fomenta la innovación rápida y la mejora continua del software.

- **Independencia Tecnológica**: El uso de software de código abierto puede reducir la dependencia de proveedores específicos y evitar el bloqueo tecnológico.

## 5. Ejercicios Prácticos

1. **Hacer un Fork y Contribuir**: Haz un fork de un proyecto en GitHub y realiza un cambio significativo, luego envía un pull request al repositorio original, de ser posible documentarlo adecuadamente.

2. **Clonar un Repositorio y Trabajar en él**: Clona un repositorio de un proyecto de interés, realiza cambios localmente y, si tienes permisos, sube esos cambios al repositorio remoto.

3. **Explorar Repositorios de Código Abierto**: Investiga varios proyectos de código abierto en GitHub. Elige uno que te interese y lee el código, la documentación, y los issues para entender cómo puedes contribuir.

## 6. Recursos Adicionales

- [Pro Git Book](https://git-scm.com/book/en/v2): Un libro completo sobre Git, disponible en línea de manera gratuita.
