---
title: "Extend Taiga"
date: 2020-10-05T11:27:09+02:00
draft: false
image: "images/post/post-3.jpg"
thumbnail: "images/contributions.png"
---

Taiga offers lots of features and [customisation options]({{< ref "/categories/customisation" >}}) that cover many different use cases and users. On top of that, Taiga is easily extensible in many ways, and you can work with Taiga information to add extra functionalities to your projects.

## API

From the beginning, Taiga has aimed to be beautiful as well as useful for developers, so it has a very curated public API, feature complete and well documented. Thanks to this API, you can connect Taiga with other tools in your organization, create your own interfaces and easily automate processes.

taiga-php and taiga-python are both excellent examples of how the API enables new ways of using Taiga, and both are community driven:

- [taiga-php]() is a wrapper made in PHP to handle the Taiga API.
- [taiga-python]() is a library, written in Python, to interact with the API.

You can check all the [community contributions]({{< ref "contributions" >}}) which add functionalities over Taiga's.

> The complete API is available at: [https://taigaio.github.io/taiga-doc/dist/api.html](https://taigaio.github.io/taiga-doc/dist/api.html)

## CSV reports

Each project in Taiga has the option to generate CSVs from the _Admin_ panel. Thanks to these CSVs, it's very straightforward to use the data in spreadsheets to generate custom reports. Taiga offers raw data in CSV so many applications can operate with the data.

You can check this [detailed tutorial]({{< ref "csv-reports.md" >}}) and [this video](https://www.youtube.com/watch?v=tdt7nqXVf_E) where you can have an idea of what you can achieve thanks to this reports.

## Webhooks

Outgoing webhooks send notifications to external services. For example, you can notify the creation of a new sprint, or follow the workflow of issues, tasks and userstories in any of your organization's tools. The external service needs to be ready to process the data in the notification. If you have a customisable reporting system, you could create reports based on the Taiga's notifications.

Currently, Taiga notifies the following events:

- a sprint is created, updated or deleted
- a user story is created, updated or deleted
- a task is created, updated or deleted
- an issue is created, updated or deleted
- a wiki page is created, updated or deleted

Check the documentation to see the [detailed payload](https://taigaio.github.io/taiga-doc/dist/webhooks.html) for each notification.

## Integrations

Taiga se puede conectar con otras aplicaciones para añadir funcionalidades. Algunas integraciones vienen ya con Taiga, otras son compartidas por la comunidad, y además tienes la posibilidad de crear tu propia integración que se ajuste a lo que tu organización necesita.

### Chats

En Taiga puedes configurar y personalizar fácilmente qué eventos quieres notificar en un canal de Slack. De esta forma, tu equipo estará siempre al tanto del estado del proyecto.

Tanto si estás usando Taiga.io como si estás usando una instancia self-hosted, puedes disponer de la integración con Slack.

Check the detailed documentation about installing and [configuring Slack](https://taiga-doc/#integration-slack).

### Repositories

Las integraciones con repositorios son la perfecta para enganchar los flujos de trabajo de negocio y de desarrollo. Por ejemplo, puedes centralizar las issues de todos tus repositorios en un proyecto de Taiga, de forma que se puedan coordinar mejor los esfuerzos y las prioridades.

Actualmente Taiga ofrece, out of the box, integración con los principales sistemas de control de versiones:

- [Github](https://taiga-doc/#integration-github)
- [Gitlab](https://taiga-doc/#integration-gitlab)
- [Bitbucket](https://taiga-doc/#integration-bitbucket)
- [Gogs](https://taiga-doc/#integration-gogs)

### Authorization

Taiga viene con un sistema de usuarios, pero permite fácilmente configurar otros sistemas de autenticación. Puedes usar Taiga dentro de tu organización y usar un sistema de autenticación centralizada. Esto se hace a través de plugins, algunos de Taiga y otros de la comunidad, que se instalan en Taiga.

Taiga ofrece plugins para la autenticación con dos sistemas ampliamente usados, como son GitHub y Gitlab. En Taiga.io puedes usar directamente cualquiera de estos dos sistemas. Para usarlo en tu instancia de Taiga, revisa la documentación sobre instalación y configuración:

- [Github](https://github.com/taigaio/taiga-contrib-github-auth)
- [Gitlab](https://github.com/taigaio/taiga-contrib-gitlab-auth)

Además, la comunidad ha creado plugins para otros sistemas de autenticación, como LDAP o Kerberos. Puedes ver el listado completo en nuestra página de [community contributions]({{< ref "contributions" >}}).

## Deployments

Siendo open source, Taiga se puede instalar self hosted y, además de las herramientas de despliegue oficiales (link-to-dock), la comunidad ha desarrollado otras para instalar Taiga.

Por ejemplo, ansible-for-taiga o docker-taiga

Puedes ver el listado completo en nuestra página de [community contributions]({{< ref "contributions" >}}).

## Import / Export projects

https://tree.taiga.io/support/admin/import-export-projects/
https://tree.taiga.io/support/importers/importers/
