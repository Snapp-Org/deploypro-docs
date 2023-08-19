---
title            : Deploy Sample App using AWS Server
sidebar_label    : Deploy Sample App
---

# Deploy Smple App with AWS on [DeployPRO](https://deploypro.dev/)

You can deploy multiple apps and install databases on the same server, but ensure that your resources are sufficient.

For the first try, let's deploy a react app using **DeployPRO** service. Bear in mind, you **must** have `Dockerfile` inside your application in the GitHub Repository.


## React App
👉 Check our react sample app [here](https://github.com/app-generator/deploypro-react). You may fork it for your sample!

1. In the `Application` Menu, click on `+ Create App`.
2. Fill out the form by providing the Application name and Environment Variable if needed. Here is some information you need to consider:

    > General

    - `Server` ( Select any server you have created on DeployPRO )
    - `Type`:
        - Deploy from source code ( Used for deploying any application from your GitHub Repository )
        - MySQL ( Used for creating a database for your application )
        - PostgresSQL ( Used for creating a database for your application )

    > Detail

    - `Repo` ( Select the repository you are going to deploy )
    - `Dockerfile Path` ( Right now, DeployPRO still needs your manual input for the location of your `dockerfile` inside the repository )
    - `Container Port` ( Please manually input the port form your `dockerfile` )
    - `Domain` ( Provide any domain name for your application. We also support `Custom Domain`!)

    > Environment Variable

    - Fill out `Key` and `Value` in case you need to add some variable.

3. Click on `Create Application` button and wait for the status to change to `running`. To monitor the status change, you can use the `refresh` button.
![DeployPRO - Application created](https://github.com/app-generator/deploypro-docs/assets/46531367/6dab439f-ff99-4ec5-8697-39eeb87a8f57)
<br />

4. Once the application is successfully deployed, you can proceed to visit the domain.
![React Domain - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/7141d006-093d-478c-a7b4-2c788b425704)
<br />

5. This is an **optional step** to perform a double-check by navigating to the `Actions` tab in your GitHub repository. Make sure the icon color of workflow run is `green`. This will allow you to confirm whether your application has been successfully deployed. For a detailed status update on the `build_image` and `deploy` process, directly select the workflow.
    ![GitHub Actions - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/f2beb697-e643-4ff9-8eaf-3494d2f5be7b)
    <br />

    On your repository, you will get new module from the deployment proces.
    ![New Module - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/30df6e00-ed93-4ea2-b725-6b8fc3b010a1)
    <br />

    The detailed view of your application resembles the image provided below. You have the flexibility to either make edits or option for deletion of the application.

    ![Application Detail - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/8c595aaf-4720-4c35-a9a9-67c9a135e30f)

    <br />

## Django App
👉 Check our Django sample app [here](https://github.com/app-generator/deploypro-django). You may fork it for your sample!

1. In the `Application` Menu, click on `+ Create App`.
2. Fill out the form by providing the Application name and Environment Variable if needed. Here is some information you need to consider:

    > General

    - `Server` ( Select any server you have created on DeployPRO )
    - `Type`:
        - Deploy from source code ( Used for deploying any application from your GitHub Repository )
        - MySQL ( Used for creating a database for your application )
        - PostgresSQL ( Used for creating a database for your application )

    > Detail

    - `Repo` ( Select the repository you are going to deploy )
    - `Dockerfile Path` ( Right now, DeployPRO still needs your manual input for the location of your `dockerfile` inside the repository )
    - `Container Port` ( Please manually input the port form your `dockerfile` )
    - `Domain` ( Provide any domain name for your application. We also support `Custom Domain`!)

    > Environment Variable

    - Fill out `Key` and `Value` in case you need to add some variable.
    - Within this Django app, there's a specific key that requires your attention. It's labeled as `APP_DOMAIN`, and you'll need to list and provide its corresponding value. The value should match the domain name provided in the details mentioned before.

    ![Django Variable - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/82a1a088-c4fc-42ee-92d1-ea6cc5c9f6cd)
    <br />

3. Click on `Create Application` button and wait for the status to change to `running`. To monitor the status change, you can use the `refresh` button.
![DeployPRO - Application created](https://github.com/app-generator/deploypro-docs/assets/46531367/5280e756-d0fc-467e-a11f-76cdf50c5ae0)
<br />

4. Once the application is successfully deployed, you can proceed to visit the domain.
![React Domain - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/c0a60981-7f7a-4709-a81f-df984947c700)
<br />

5. This is an **optional step** to perform a double-check by navigating to the `Actions` tab in your GitHub repository. Make sure the icon color of workflow run is `green`. This will allow you to confirm whether your application has been successfully deployed. For a detailed status update on the `build_image` and `deploy` process, directly select the workflow.
    ![GitHub Actions - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/375dcc0f-994a-4a03-b987-083749864c8e)
    <br />

    On your repository, you will get new module from the deployment proces.
    ![New Module - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/8c0eee43-346b-4728-853e-3156d1cc044e)
    <br />

    The detailed view of your application resembles the image provided below. You have the flexibility to either make edits or option for deletion of the application.

    ![Application Detail - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/3f868417-7ea0-4584-ad45-fdcaf5327f4b)

    <br />

## Flask App
👉 Check our Flask sample app [here](https://github.com/app-generator/deploypro-flask). You may fork it for your sample!

1. In the `Application` Menu, click on `+ Create App`.
2. Fill out the form by providing the Application name and Environment Variable if needed. Here is some information you need to consider:

    > General

    - `Server` ( Select any server you have created on DeployPRO )
    - `Type`:
        - Deploy from source code ( Used for deploying any application from your GitHub Repository )
        - MySQL ( Used for creating a database for your application )
        - PostgresSQL ( Used for creating a database for your application )

    > Detail

    - `Repo` ( Select the repository you are going to deploy )
    - `Dockerfile Path` ( Right now, DeployPRO still needs your manual input for the location of your `dockerfile` inside the repository )
    - `Container Port` ( Please manually input the port form your `dockerfile` )
    - `Domain` ( Provide any domain name for your application. We also support `Custom Domain`!)

    > Environment Variable

    - Fill out `Key` and `Value` in case you need to add some variable.

3. Click on `Create Application` button and wait for the status to change to `running`. To monitor the status change, you can use the `refresh` button.
![DeployPRO - Application created](https://github.com/app-generator/deploypro-docs/assets/46531367/ff7168ac-29d1-4a96-901e-8b1884e9514d)
<br />

4. Once the application is successfully deployed, you can proceed to visit the domain.
![React Domain - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/0d5bd363-44c1-4dcb-9555-810e25c49fcc)
<br />

5. This is an **optional step** to perform a double-check by navigating to the `Actions` tab in your GitHub repository. Make sure the icon color of workflow run is `green`. This will allow you to confirm whether your application has been successfully deployed. For a detailed status update on the `build_image` and `deploy` process, directly select the workflow.
    ![GitHub Actions - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/33f61fff-2ea3-4355-a009-86a0075a9ae9)
    <br />

    On your repository, you will get new module from the deployment proces.
    ![New Module - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/5f3b704f-1c72-41c9-b26a-83c8fdebb6dd)
    <br />

    The detailed view of your application resembles the image provided below. You have the flexibility to either make edits or option for deletion of the application.

    ![Application Detail - DeployPRO](https://github.com/app-generator/deploypro-docs/assets/46531367/be6d3e4c-48f1-405e-853d-1ea4f46747fa)

    <br />

If you encounter some issue while deploying your application, don't hesitate to [inform us](https://discord.gg/qQhjQZhnur)! 😉

<br />

## Resources

- 👉 [Deploy Projects](https://deploypro.dev/) using your preferred provider: `AWS`, `GCP`, `Azzure`
- 👉 Get [Deployment Support](https://deploypro.dev/support/) from the team behind this service
- 👉 Join the [Community](https://discord.gg/qQhjQZhnur) and chat with the team behind `DeployPRO`
