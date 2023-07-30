---
sidebar_order    : 3
title            : Create a Static App using AWS Server
sidebar_label    : Create a Static App
---

# Create a Static App with AWS on [DeployPRO](https://deploypro.dev/)

You can install multiple apps and databases on the same server, but ensure that your resources are sufficient.

For the first try, let's deploy a react app using **DeployPRO** service. Bear in mind, you **must** have `Dockerfile` inside your application in the GitHub Repository.

👉 Check our react sample app [here](https://github.com/app-generator/deploypro-react). You may fork it for your sample!

## React App
1. In the `Application` Menu, click on `+ Create App`.
2. Fill out the form by providing the Application name and Environment Variable if needed. Here is some information you need to consider:

    > General
    - `Server` ( Select any server you have created on DeployPRO )
    - `Type`:
        - Deploy from source code ( Used for deploying any application from your GitHub Repository )
        - MySQL ( Used for creating a database for your application )
        - PostgresSQL ( Used for creating a database for your application )
    
    > Detail
    - `Dockerfile Path` ( Right now, DeployPRO still needs your manual input for the location of your `dockerfile` inside the repository )
    - `Container Port` ( Please manually input the port form your `dockerfile` )
    - `Port` ( You can provide any number for your port. However, make sure that you have different port number for each application on a server )
    - `Domain` ( Provide any domain name for your application. We also support `Custom Domain`!)

    > Environment Variable
    - Fill out `Key` and `Value` in case you need to add some variable.

3. Click on `Create Application` button and wait for a couple second.
![DeployPRO - Application created](https://github.com/app-generator/deploypro-docs/assets/46531367/b72526c2-a2c5-46d0-a381-5c5060b86d49)
<br />

4. After your application created, check `Actions` Tab on your GitHub repository to confirm whether your application is deployed successfullly.

If you encounter some issue while deploying your application, don't hesitate to [inform us](https://discord.gg/qQhjQZhnur)!

<br />

## Resources

- 👉 [Deploy Projects](https://deploypro.dev/) using your preferred provider: `AWS`, `GCP`, `Azzure`
- 👉 Get [Deployment Support](https://deploypro.dev/support/) from the team behind this service
- 👉 Join the [Community](https://discord.gg/qQhjQZhnur) and chat with the team behind `DeployPRO`
