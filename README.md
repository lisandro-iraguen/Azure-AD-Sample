

# Microsoft Graph sample Blazor WebAssembly app

[![.NET](https://github.com/microsoftgraph/msgraph-sample-blazor-clientside/actions/workflows/dotnet.yml/badge.svg)](https://github.com/microsoftgraph/msgraph-sample-blazor-clientside/actions/workflows/dotnet.yml) ![License.](https://img.shields.io/badge/license-MIT-green.svg)

This sample demonstrates how to use the Microsoft Graph .NET SDK to access data in Office 365 from Blazor WebAssembly apps.

> **NOTE:** This sample was originally built from a tutorial published on the [Microsoft Graph tutorials](https://docs.microsoft.com/graph/tutorials) page. That tutorial has been removed.

## Register an app in Azure AD

1. Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com). Login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.

1. Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.

1. Select **New registration**. On the **Register an application** page, set the values as follows.

    - Set **Name** to `Blazor Graph Sample`.
    - Set **Supported account types** to **Accounts in any organizational directory and personal Microsoft accounts**.
    - Under **Redirect URI**, set the first drop-down to **Single-page application (SPA)** and set the value to `https://localhost:7067/authentication/login-callback`.

1. Select **Register**. On the **Blazor Graph Tutorial** page, copy the value of the **Application (client) ID** and save it, you will need it in the next step.

## Configure the sample

1. Create a new file in the **./GraphSample/wwwroot** directory named **appsettings.Development.json** and add the following code.

    ```json
    {
      "AzureAd": {
        "ClientId": "YOUR_CLIENT_ID_HERE"
      }
    }
    ```

1. Replace `YOUR_CLIENT_ID_HERE` with the **Application (client) ID** value from your app registration.

result:

![image](https://github.com/user-attachments/assets/b171256b-6264-4780-8832-0923c6c4b8da)
![image](https://github.com/user-attachments/assets/04a57c8e-4f87-459b-8dc1-620e77f8b6e2)
![image](https://github.com/user-attachments/assets/2af542b5-330f-4840-8095-9607d5fe03a1)
![image](https://github.com/user-attachments/assets/36d42590-fcac-4ccf-b831-3bdb1ff91011)




