# SPKDSA
A very simplified full stack framework for passwordless authentication using public key digital signature authentication.

## 🌍 Project Neutrality
This project is licensed under the MIT License to ensure maximum openness and neutrality.  

The goal is to avoid restrictions tied to specific governments, organizations, or jurisdictions.

## Legal Precedents
Court rulings (e.g. *Jacobsen v. Katzer*, BusyBox cases, *Artifex v. Hancom*) confirm that
open source licenses are legally enforceable. While these precedents provide important
protection for contributors, this project explicitly seeks to avoid situations where
contributors are excluded based on nationality, politics, or sanctions.

## Neutrality based code contributions
- To maintain long-term neutrality and legal clarity of this project, all contributions must follow the Contributor License Agreement (CLA).
- By contributing, you confirm that your work is your own (or you have the rights to submit it).
- You grant the project maintainers the right to use, modify, and relicense your contribution under the project’s license, ensuring that no future legal or geopolitical restrictions affect this project.
- This approach is informed by international legal precedents (Jacobsen v. Katzer, BusyBox GPL cases, Artifex v. Hancom, Hellwig v. VMware, etc.), which confirm that open-source licenses are legally binding.

For details, refer to [CLA Here](https://github.com/Chewhern/SPKDSA/blob/main/CLA.md)

## Components/Environment required

[Download Dotnet 8.0 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)

Client device requires a desktop environment with resolution of **1920 x 1080**.

On Linux(Ubuntu), you need to execute **apt install dotnet-sdk-8.0**. If such execution was not possible then you can use Windows to compile and deploy on Linux.

### Building applications (On Windows with Visual Studio)
1. Navigate to the source code folder whereby there's ".csproj" inside.
2. Click on the file.
3. Right click on the ".csproj" file inside visual studio and click on "build".
4. The application will reside in "bin/debug".

### Building applications (On MacOS/Linux)
1. Navigate to the source code folder whereby there's ".csproj" inside with command prompt/terminal/console.
2. Do **dotnet build**
3. The application will reside in "bin/debug".

### Building client applications
1. Navigate to a single client's application's both source code folder.
2. Build on the client application without ".Desktop".
3. Build on the client application with ".Desktop".
4. The client application will reside within ".Desktop" folder.
5. Navigate to "bin/debug".

### Run compiled applications (On Windows)
1. Kindly navigate to the respective folder and double click on ".exe".

### Run compiled applications (On MacOS/Linux)
1. Kindly navigate to the respective folder and do **dotnet app.dll**

#### Host and deploy server applications (Web API)
[Click Here](https://learn.microsoft.com/en-us/aspnet/core/host-and-deploy/linux-nginx?view=aspnetcore-9.0&tabs=linux-ubuntu#monitor-the-app)

1. Follow the steps accordingly.
2. Change the "User" to the user that has permission on compiled web api server application.
3. Ignore
```
Colon (:) separators aren't supported in environment variable names. Use a double underscore (__) in place of a colon. The Environment Variables configuration provider converts double-underscores into colons when environment variables are read into configuration. In the following example, the connection string key ConnectionStrings:DefaultConnection is set into the service definition file as ConnectionStrings__DefaultConnection:

Console

Copy
Environment=ConnectionStrings__DefaultConnection={Connection String}
Save the file and enable the service.
```
4. Finish until **systemctl**.
