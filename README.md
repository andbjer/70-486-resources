# 70-486 Resources
Exam 70-486 Objectives and Resources

# 1. Design the application architecture

**Weighting: 15-20%**

## Plan the application layers

**Objectives:**
- Plan data access
- plan for separation of concerns, appropriate use of models, views, controllers, components, and service dependency injection
- choose between client-side and server-side processing
- design for scalability
- choose between ASP.NET Core and ASP.NET
- choose when to use .NET standard libraries

## Design a distributed application

**Objectives:**
- Design a hybrid application
- plan for session management in a distributed environment
- plan web farms
- run Microsoft Azure services on-premises with Azure Pack
- enable deferred processing through Azure features including queues, scheduled and on-demand jobs, Azure Functions, and Azure Web Jobs

**References:**
- [Distributed caching in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/performance/caching/distributed?view=aspnetcore-2.2) 

## Design and implement the Azure Web Apps life cycle

**Objectives:**
- Identify and implement Start, Run, and Stop events
- code against application events in applications
- configure startup tasks, including IIS, app pool configuration, and third-party tools

**References:**
- [How to configure and run startup tasks for a cloud service](https://docs.microsoft.com/en-us/azure/cloud-services/cloud-services-startup-tasks)
- [Common Cloud Service startup tasks](https://docs.microsoft.com/en-us/azure/cloud-services/cloud-services-startup-tasks-common)
- [Windows Azure Start-up Tasks Part 1](https://blogs.msdn.microsoft.com/cclayton/2012/05/17/windows-azure-start-up-tasks-part-1/)
- [RoleEntryPoint.OnStart Method](https://docs.microsoft.com/en-us/previous-versions/azure/reference/ee772851(v=azure.100))

## Configure state management

**Objectives:**
- Choose a state management mechanism including in-process, out of process, and Redis-based state management
- plan for scalability
- use cookies or local storage to maintain state
- apply configuration settings in web.config files
- implement sessionless state including query strings
- configure middleware to enable session and application state in ASP.NET Core

**References:**
- [Session and app state in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/app-state?view=aspnetcore-2.2)
- 

## Design a caching strategy

**Objectives:**
- Implement page output caching and data caching
- create cache profiles
- implement HTTP caching
- implement Azure Redis caching
- plan a content delivery network (CDN) strategy, for example, Azure CDN

**References:**
- [Response caching in ASP.NET Core](https://docs.microsoft.com/nb-no/aspnet/core/performance/caching/response?view=aspnetcore-2.2)
- 

## Design and implement a Web Socket strategy

**Objectives:**
- Read and write string and binary data asynchronously
- choose a connection loss strategy
- decide when to use Web Sockets
- implement SignalR
- enable web socket features in an Azure Web App instance

**References:**
- [WebSocket](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket)
- [Introduction to ASP.NET Core SignalR](https://docs.microsoft.com/en-us/aspnet/core/signalr/introduction?view=aspnetcore-2.2)
- [WebSockets support in ASP.NET Core](https://docs.microsoft.com/nb-no/aspnet/core/fundamentals/websockets?view=aspnetcore-2.2)

## Design a configuration management solution

**Objectives:**
- Manage configuration sources, including XML, JSON, and INI files
- manage environment variables
- implement Option objects
- implement multiple environments using files and hierarchical structure
- manage sensitive configuration
- react to runtime configuration changes
- implement a custom configuration source
- secure configuration by using Azure Key Vault
- use the Secret Manager tool in development to keep secrets out of your code for configuration values

**References:**
- [Tutorial: Use Azure Key Vault with an Azure web app in .NET](https://docs.microsoft.com/nb-no/azure/key-vault/tutorial-net-create-vault-azure-web-app)
- [Add Key Vault to your web application by using Visual Studio Connected Services](https://docs.microsoft.com/en-us/azure/key-vault/vs-key-vault-add-connected-service)
- [Safe storage of app secrets in development in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/app-secrets?view=aspnetcore-2.2&tabs=windows)

## Interact with the host environment

**Objectives:**
- Work with file system using file providers
- work with environment variables
- determine hosting environment capabilities
- implement native components, including PInvoke and native dependencies for hosts including Linux and Windows
- use ASP.NET hosting on an Open Web Interface for .NET (OWIN)-based server

**References:**
- [Open Web Interface for .NET (OWIN) with ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/owin?view=aspnetcore-2.2)

## Compose an application by using the framework pipeline

**Objectives:**
- Add custom request processing modules to the pipeline
- add, remove, and configure services used in the application
- design and implement middleware
- design for kestrel, Http.sys web server and IIS
- design and implement startup filters

**References:**
- [ASP.NET Core Middleware](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/middleware/?view=aspnetcore-2.2)
- [App startup in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/startup?view=aspnetcore-2.2)
- [Resolving ASP.NET Core Startup Class from the DI Container](https://www.strathweb.com/2017/06/resolving-asp-net-core-startup-class-from-the-di-container/)

# 2. Design the build and deployment architecture

**Weighting: 10-15%**

## Design a browser artifact build strategy

**Objectives:**
- Design a JavaScript build pipeline using Gulp, Grunt, npm and Bower
- design an artifact build strategy using Less, Sass and Font Awesome
- design and implement a bundling and minification strategy for browser artifacts, including JavaScript, CSS and images

## Design a server build strategy

**Objectives:**
- Manage NuGet dependencies
- target runtimes, including the full .NET Framework, .NET core, and .NET standard
- manage debug and release configurations, including compilation and optimization options
- include or exclude files from build
- manage build sources, including content, resources, and shared files
- implement metadata for projects, including version, release notes, and descriptions
- define other build options, including xmlDoc and warningsAsErrors
- work with static files in ASP.NET core

**References:**
- [dotnet build](https://docs.microsoft.com/en-us/dotnet/core/tools/dotnet-build)
- [Additions to the csproj format for .NET Core](https://docs.microsoft.com/en-us/dotnet/core/tools/csproj) 
- [How to generate XML documentation for CSPROJ with multiple targets](https://stackoverflow.com/questions/47115877/how-to-generate-xml-documentation-for-csproj-with-multiple-targets)
- [A mapping between project.json and csproj properties](https://docs.microsoft.com/en-us/dotnet/core/tools/project-json-to-csproj)

## Design a publishing strategy

**Objectives:**
- Implement application publishing using dotnet.exe
- manage publishing options in csproj
- implement additional tooling
- implement pre-publish and post-publish scripts
- implement native compilation
- publish to Docker container image

## Implement an Azure deployment strategy

**Objectives:**
- Deploy Azure Web App using supported deployment models including FTP, Kudu, Web Deploy, and Visual Studio Publishing Wizard
- provision ARM- based resources while deploying applications
- implement deployment environments, including dev, test, and prod in Azure
- use deployment slots for staging sites
- deploy to Azure Stack

## Implement a on-premises deployment strategy

**Objectives:**
- Deploy application to IIS using Web Deploy, xcopy, and Visual Studio Publishing Wizard
- deploy application to Windows Nano Server, deploy application to IIS Hosted Web Core, deploy application to HTTP.sys web server
- deploy application to Kestrel on Windows and Linux
- implement reverse proxying to Kestrel using IIS and Nginx

**References:**
- [HTTP.sys web server implementation in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/servers/httpsys?view=aspnetcore-2.2)
- [Kestrel web server implementation in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/servers/kestrel?view=aspnetcore-2.2)
- [Host ASP.NET Core on Windows with IIS](https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/iis/?view=aspnetcore-2.2)
- [Host ASP.NET Core on Linux with Nginx](https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/iis/?view=aspnetcore-2.2)

# 3. Design the User Experience

**Weighting: 15-20%**

## Create elements of the user interface for a web application

**Objectives:**
- Create and apply styles by using CSS
- structure and lay out the user interface by using HTML
- implement dynamic page content based on a design

**References:**
- [Pseudo-classes](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)
- [Combinators and selector lists](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Combinators_and_multiple_selectors)
- [What is the difference between :first-child and :first-of-type?](https://stackoverflow.com/questions/24657555/what-is-the-difference-between-first-child-and-first-of-type)

## Design and implement UI behavior

**Objectives:**
- Implement client-side validation
- use JavaScript to manipulate the DOM
- extend objects by using prototypal inheritance
- use AJAX to make partial page updates

**References:**
- [Inheritance in JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Inheritance)
- [RegExp](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp)
- [Ajax](https://api.jquery.com/category/ajax/)
- [What is JSONP, and why was it created](https://stackoverflow.com/questions/2067472/what-is-jsonp-and-why-was-it-created)

## Design the UI layout of an application

**Objectives:**
- Implement partial views and view components for reuse in different areas of the application
- design and implement pages by using Razor Pages
- design and implement layouts to provide visual structure
- define and render optional and required page sections
- create and use tag and HTML helpers to simplify markup

**References:**
- [Views in ASP.NET Core MVC](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/overview?view=aspnetcore-2.2)
- [Partial views in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/partial?view=aspnetcore-2.2)
- [ASP.NET Core built-in Tag Helpers](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/tag-helpers/built-in/?view=aspnetcore-2.2)

## Plan a responsive UI layout

**Objectives:**
- Plan for applications that run on multiple devices and screen resolutions
- use media queries and Bootstrap’s responsive grid
- detect browser features and capabilities
- create a web application that runs across multiple browsers and mobile devices
- enable consistent cross-browser experiences with polyfills

**References:**
- [Using the viewport meta tag to control layout on mobile browsers](https://developer.mozilla.org/en-US/docs/Mozilla/Mobile/Viewport_meta_tag)
- [@media](https://developer.mozilla.org/en-US/docs/Web/CSS/@media)
- [Using media queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)
- [HTML <link> media attribute](https://www.w3schools.com/tags/att_link_media.asp)

## Plan mobile UI strategy

**Objectives:**
- Implement mobile specific UI elements such as touch input, low bandwidth situations, and device oritentation changes
- define and implement a strategy for working with mobile browsers

**References:**
- 

# 4. Develop the User Experience

**Weighting: 15-20%**

## Plan for search engine optimization and accessibility

**Objectives:**
- Use analytical tools to parse HTML
- provide an xml sitemap and robots.txt file to improve scraping
- write semantic markup for accessibility, for example, screen readers
- use rich snippets to increase content visibility

**References:**
- [Accessibility](https://developer.mozilla.org/en-US/docs/Web/Accessibility)
- [ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA)

## Plan and implement globalization and localization

**Objectives:**
- Plan a localization strategy
- create and apply resources to UI including JavaScript resources
- set cultures
- implement server side localization and globalization

**References:**
- [Globalization and localization in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/localization?view=aspnetcore-2.2)
- [ASP.NET Globalization and Localization](https://docs.microsoft.com/en-us/previous-versions/c6zyy3s9%28v%3dvs.140%29)
- [ASP.NET Web Page Resources Overview](https://docs.microsoft.com/en-us/previous-versions/ms227427(v=vs.140))
- [How to: Retrieve Resource Values Programmatically](https://docs.microsoft.com/en-us/previous-versions/ms227982(v=vs.140))

## Design and implement MVC controllers and actions

**Objectives:**
- Apply authorization attributes, filters including global, authentication, and overriddable filters
- choose and implement custom HTTP status codes and responses
- implement action results
- implement MVC areas
- implement Dependency Injection for services in controllers

**References:**
- [Filters in ASP.NET Core](https://docs.microsoft.com/nb-no/aspnet/core/mvc/controllers/filters?view=aspnetcore-2.2)
- [Format response data in ASP.NET Core Web API](https://docs.microsoft.com/en-us/aspnet/core/web-api/advanced/formatting?view=aspnetcore-2.2)
- [Controller action return types in ASP.NET Core Web API](https://docs.microsoft.com/en-us/aspnet/core/web-api/action-return-types?view=aspnetcore-2.2)
- [Dependency injection into controllers in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/mvc/controllers/dependency-injection?view=aspnetcore-2.2)

## Design and implement routes

**Objectives:**
- Define a route to handle a URL pattern
- apply route constraints
- ignore URL patterns
- add custom route parameters
- define areas
- define routes that interoperate with Single Page Application frameworks such as Angular

**References:**
- [Routing in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/routing?view=aspnetcore-2.2)
- [Routing to controller actions in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/mvc/controllers/routing?view=aspnetcore-2.2)

## Control application behavior by using MVC extensibility points

**Objectives:**
- Create custom middleware and inject it into the pipeline
- implement MVC filters and controller factories
- control application behavior by using action results, model binders, and route handlers
- inject services into a view

**References:**
- [Write custom ASP.NET Core middleware](https://docs.microsoft.com/nb-no/aspnet/core/fundamentals/middleware/write?view=aspnetcore-2.2)
- [Custom ASP.NET Core Middleware Example](https://devblogs.microsoft.com/dotnet/custom-asp-net-core-middleware-example/) 
- [Dependency injection into views in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/dependency-injection?view=aspnetcore-2.2)
- [Filters in ASP.NET Core](https://docs.microsoft.com/nb-no/aspnet/core/mvc/controllers/filters?view=aspnetcore-2.2)

## Design and implement serialization and model binding

**Objectives:**
- Serialize models and data using supported serialization formats, including JSON, XML, protobuf, and WCF/SOAP
- implement model and property binding, including custom binding and model validation
- implement web socket communication in MVC
- implement file uploading and multipart data
- use AutoRest to build clients

**References:**
- [SerializableAttribute Class](https://docs.microsoft.com/en-us/dotnet/api/system.serializableattribute?view=netcore-2.2)
- [XML and SOAP Serialization](https://docs.microsoft.com/en-us/dotnet/standard/serialization/xml-and-soap-serialization?view=netframework-4.8)
- [Model Binding in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/mvc/models/model-binding?view=aspnetcore-2.2)
- [WebSockets support in ASP.NET Core](https://docs.microsoft.com/nb-no/aspnet/core/fundamentals/websockets?view=aspnetcore-2.2)

# 5. Troubleshoot and Debug Web Applications

**Weighting: 20-25%**

## Prevent and troubleshoot runtime issues

**Objectives:**
- Troubleshoot performance, security, and errors
- implement tracing, logging, and debugging including IntelliTrace
- enable and configure health monitoring including Performance Monitor
- configure and use App Insights runtime telemetry

**References:**
- [Trace the flow of a Cloud Services application with Azure Diagnostics](https://docs.microsoft.com/en-us/azure/cloud-services/cloud-services-dotnet-diagnostics-trace-flow)
- 

## Design an exception handling strategy

**Objectives:**
- Handle exceptions across multiple layers
- use MVC middleware to configure error handling
- use different exception handling strategies for different environments
- create and display custom error pages
- configure a custom pipeline for error handling
- handle first chance exceptions
- configure and use App Insights
- log application exceptions

## Test a web application

**Objectives:**
- Create and run unit tests, for example, use the Assert class, create mocks and stubs
- create and run web tests including using Browser Link
- debug a web application in multiple browsers and mobile emulators
- use Azure DevTest Labs
- use Visual Studio Team Services

**References:**
- [Use Azure DevTest Labs for VM and PaaS test environments](https://docs.microsoft.com/en-us/azure/lab-services/devtest-lab-test-env)
- 

## Debug an Azure application

**Objectives:**
- Collect diagnostic information by using Azure App Insights
- choose log types, for example, event logs, performance counters, and crash dumps
- stream logs directly to Visual Studio from a deployed site
- debug an Azure application by using Visual Studio and remote debugging
- interact directly with remote Azure websites using Server Explorer

**References:**
- [Troubleshoot an app in Azure App Service using Visual Studio](https://docs.microsoft.com/nb-no/azure/app-service/troubleshoot-dotnet-visual-studio)
- [LogLevel Enumeration](https://docs.microsoft.com/en-us/previous-versions/azure/reference/ee773154(v=azure.100))
- [Azure Diagnostics 1.3 and later configuration schema](https://docs.microsoft.com/nb-no/azure/azure-monitor/platform/diagnostics-extension-schema-1dot3)
- 

# 6. Design and Implement Security

**Weighting: 15-20%**

## Configure authentication

**Objectives:**
- Authenticate users
- enforce authentication settings
- implement ASP.NET Core Identity
- enable Facebook, Google and other external providers
- implement account confirmation, password recovery, and multi-factor authentication
- perform authentication using Azure Active Directory, Azure Active Directory B2C, Azure Active Directory B2B, and Microsoft Identity manage user session by using cookies
- acquire access tokens using the Microsoft Authentication Library (MSAL)

**References:**
- [Introduction to Identity on ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity?view=aspnetcore-2.2&tabs=visual-studio)
- [Configure ASP.NET Core Identity](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity-configuration?view=aspnetcore-2.2)
- [Facebook, Google, and external provider authentication in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/social/?view=aspnetcore-2.2&tabs=visual-studio)
- [Account confirmation and password recovery in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/accconfirm?view=aspnetcore-2.2&tabs=visual-studio)
- [Azure Active Directory with ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/azure-active-directory/?view=aspnetcore-2.2)
- [Tutorial - Enable your Web Apps to sign-in users and call APIs with the Microsoft identity platform for developers](https://azure.microsoft.com/en-us/resources/samples/active-directory-aspnetcore-webapp-openidconnect-v2/)
- [Azure AD with ASP.NET Core 2.0](https://www.c-sharpcorner.com/article/azure-ad-with-asp-net-core-2-0/)
- [Azure AD Authentication in ASP.NET Core APIs part 1: Basic setup, checking scopes, creating a test client](https://joonasw.net/view/azure-ad-authentication-aspnet-core-api-part-1)
- 

## Configure and apply authorization

**Objectives:**
- Create roles 
- authorize roles programmatically
- configure and work with custom UserStores using middleware
- configure controllers and actions to participate in authorization

**References:**
- [Razor Pages authorization conventions in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/authorization/razor-pages-authorization?view=aspnetcore-2.2)
- [Simple authorization in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/authorization/simple?view=aspnetcore-2.2)
- [Role-base authorization in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/authorization/roles?view=aspnetcore-2.2)

## Design and implement claims-based authentication

**Objectives:**
- Perform authentication and authorization using tokens including OpenID, OAuth, JWT, SAML, bearer tokens, etc.

**References:**
- [Claims-based authorization in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/authorization/claims?view=aspnetcore-2.2)
- [Policy-based authorization in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/authorization/policies?view=aspnetcore-2.2)

## Manage data integrity

**Objectives:**
- Apply encryption to application data
- apply encryption to the configuration sections of an application
- sign application data to prevent tampering
- secure data using Azure Key Vault
- implement encryption for data protection using the data protection APIs in transit and at rest

**References:**
- [Tutorial: Use Azure Key Vault with an Azure web app in .NET](https://docs.microsoft.com/nb-no/azure/key-vault/tutorial-net-create-vault-azure-web-app)
- [Get started with the Data Protection APIs in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/security/data-protection/using-data-protection?view=aspnetcore-2.2)

## Implement a secure site

**Objectives:**
- Secure communication by applying SSL certificates
- require SSL for all requests
- enable SSL hosting in the development environment
- implement SSL using Azure Load Balancers
- salt and hash passwords for storage
- use HTML encoding to prevent cross-site scripting attacks (ANTI-XSS Library)
- implement deferred validation and handle unvalidated requests, for example, form, querystring, and URL
- prevent SQL injection attacks by parameterizing queries
- prevent cross-site request forgeries (XSRF)
- use Azure Security Center to monitor Azure resources
- implement Cross Origin Resource Sharing (CORS)
- implement protection against open redirect attacks

**References:**
- [HttpServerUtility.HtmlEncode Method](https://docs.microsoft.com/en-us/dotnet/api/system.web.httpserverutility.htmlencode?view=netframework-4.8&viewFallbackFrom=netcore-2.2)
- [Prevent Cross-Site Scripting (XSS) in ASP.NET Core](https://docs.microsoft.com/nb-no/aspnet/core/security/cross-site-scripting?view=aspnetcore-2.2)
- [Enable Cross-Origin Requests (CORS) in ASP.NET Core](https://docs.microsoft.com/nb-no/aspnet/core/security/cors?view=aspnetcore-2.2)
