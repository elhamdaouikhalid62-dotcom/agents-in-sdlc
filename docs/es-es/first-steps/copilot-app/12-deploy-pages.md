---
title: "Lección 12 - Publica el sitio con GitHub Pages"
description: "Configura el flujo de trabajo de Pages con la aplicación GitHub Copilot, revisa la solicitud de incorporación de cambios y comprueba el Space Quiz publicado."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

Publica el Space Quiz con GitHub Pages para que cualquiera pueda acceder a él. Copilot puede preparar el flujo de trabajo y guiarte durante el despliegue, pero debes revisar los cambios y confirmar que el sitio se ha publicado.

En esta lección:

- Pide a Copilot que configure el despliegue en GitHub Pages.
- Revisa el flujo de trabajo y la solicitud de incorporación de cambios antes de combinarla.
- Sigue el despliegue y comprueba el sitio publicado.

## Escenario

El Space Quiz ya está en un repositorio de GitHub, pero todavía no hay una forma sencilla de acceder a él. Si publicas el sitio de un solo archivo con GitHub Pages, estará disponible en una URL pública sin añadir un servidor ni dependencias de ejecución.

## Pide a Copilot que publique el sitio

En la sesión de la aplicación Copilot de `space-quiz`, envía este prompt:

```plaintext
Activa GitHub Pages para este repositorio. Si es necesario, crea un flujo de trabajo de GitHub Actions que compile y despliegue el sitio web en GitHub Pages. Si aún no hay un README, añade uno que describa la aplicación y cómo ejecutarla localmente. Crea una solicitud de incorporación de cambios con los cambios y combínala cuando se superen las comprobaciones necesarias. Supervisa el despliegue hasta que se complete correctamente y, después, indícame la URL final del sitio web. Si no tienes permiso para activar Pages o combinar la solicitud, dime exactamente qué debo aprobar o hacer. No indiques que el despliegue se ha completado hasta que el sitio esté publicado de verdad.
```

![Diagrama en tres pasos que muestra la combinación de la solicitud de incorporación de cambios de Space Quiz, una ejecución de GitHub Actions correcta con los pasos Build website, Upload artifact y Deploy to Pages, y Space Quiz abierto en yourname.github.io/space-quiz/](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> Este prompt pide al agente que cree y combine una solicitud de incorporación de cambios y que cambie la configuración de Pages del repositorio. Antes de continuar, revisa el diff, los permisos de despliegue y las solicitudes de aprobación de GitHub.

## Revisa el flujo de trabajo y comprueba el despliegue

1. Confirma que solo se ha añadido un README si el repositorio todavía no tenía uno.
2. Revisa los cambios de la solicitud de incorporación de cambios, incluidos los pasos de compilación y despliegue del flujo de trabajo.
3. Combina la solicitud solo después de que se superen las comprobaciones necesarias.
4. Comprueba que la ejecución de despliegue de GitHub Actions finaliza correctamente.
5. Abre la URL indicada y confirma que se carga el Space Quiz.

Si el agente no puede activar Pages o combinar la solicitud, sigue las instrucciones concretas que te proporcione. No des por terminado el trabajo hasta que el despliegue finalice correctamente y el sitio esté disponible.

## Resumen y siguientes pasos

Has publicado el Space Quiz como un sitio web real y has comprobado el despliegue en lugar de confiar únicamente en el informe del agente. Continúa con la [Lección 13: Repaso y pasos siguientes][next-lesson].

[next-lesson]: ../13-review/
