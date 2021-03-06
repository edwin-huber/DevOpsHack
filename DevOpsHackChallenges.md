# DevOps Challenge \#1 - VSTS Project Setup #
In this challenge you will create a VSTS account, invite users, set up a project and create a team with your colleagues. If you need help check out the [hints for this challenge](/FirstSteps/FirstSteps.md).

 

## Achievements ##
| # | Achievement   | Maximum score |
|-|-|-|
|1.| Create a Microsoft Account on https://signup.live.com/| 10 |
|2.| Create a Free Microsoft Azure Account on https://azure.microsoft.com/de-de/free/| 10 |
|3.| Create a VSTS account on http://visualstudio.com| 10 |
|4.| Give your colleagues access to your account | 10 |
|5.| Give your team members an appropriate security level | 10 |
|6.| Create a Team Project called RedBlueTeamProject within your VSTS account| 10 |
|7.| Invite users to your new Team Project | 10 |
|8.| Create a team named "Team Blue" within your Team Project and invite your colleagues |10|

## Bonus Goals ##
| # | Bonus Goal   | Maximum score |
|-|-|-|
|1.| Create another team named "Team Red" within your Team Project and invite some colleagues |10|


# DevOps Challenge \#2 - Work Management and process customization #
In this challenge, you will configure VSTS to trace and plan your work.
If you need help check out the [Process Customization Hints](/ProcessCustomization/ProcessCustomization.md) and [WorkItem Management Hints](/WorkItemManagement/WorkManagement.md) plus the [Dashboard customization Hints](/Dashboard/Dashboard.md).
## Achievements ##
| # | Achievement   | Maximum score |
|-|-|-|
|1.| Create a custom process template called "RedBlueAgileTemplate" based on agile template | 10 |
|2.| Create a new Work Item Type "Vision" above Scenario | 10 |
|3.| Modify your team project to inherit from this template. | 10 |
|4.| Customize your board to display items which are done in green + also display Epics |10|
|5.| Create work items with releationship helping you manage the next challenges and keep track of your progress. Create them in a hierarchical manner. Starting at Feature / Epic level.  | 10 |
|6.| Link work items, view history | 10 |
|7.| Modify dashboard to show Reports & Stats (Come back to this after completing challenges 4, 5 and 6 to finish this Goal)  | 10 |
|8.| Modify dashboard to show team members, your current workitems, nr of bugs | 10 |


## Bonus Goals ##
| # | Bonus Goal   | Maximum score |
|-|-|-|
|1.| Add a few styling rules to your board highlighting important Items ( e.g. Bugs or Items with a special Tag)| 10 |
|2.| Add a custom state Testing in your Work Item| 10 |
|3.| Add a custom field 'Coffee consumed(in liters)' on your work item | 10 |
|4.| Modify your work view  to display the new hierarchy level|10|
|5.| Customize your board to display Id, owner and the value of your new custom field|10|



# DevOps Challenge \#3 - Version Control #
In this challenge, you will set up version control, upload code and configure policies.
If you need help check out the [Version Control Hints](/VersionControl/VersionControl.md).
## Achievements ##
| # | Achievement   | Maximum score |
|-|-|-|
|1.| Create a new Git repository in your Team Project| 10 |
|2.| Clone our sample repository found [here](https://github.com/DanielMeixner/DevOpsHackSample) to your machine | 10 |
|3.| Push the code to your new repo in your Team Project  | 10 |
|4.| Modify your repo to require a pull request to merge code into your master branch  | 10 |
|5.|Modify your repo to require a Work Item linked to a pull request |10|
|6.| Configure your repo to require at least one of your colleagues as approver  | 10 |
|7.| Create a new Branch. Check it out and modify code locally changing the displayed Name of the Demo Website. Commit the change, then initiate and complete a pull request. Link a work item and follow the review process. | 10 |

## Bonus Goals ##
| # | Bonus Goal   | Maximum score |
|-|-|-|
|1.| Investigate the history of the file committed following the trace from the work item | 10 |
|-| (With several teammembers:) Create a merge conflict on purpose and solve it |-|
|2.| Integrate an external Git Repository (e.g. hosted on GitHub) and wire it up for CI |-|
|-| Discuss: What would be an appropriate code flow & branching stratgey in Git?|-|
|-| Discuss: What are the main differentiators between TFVS and Git?  |-|
|3.| Revisite this Challenge after you have successfully created a Build definition and change the Branch Policie to also require a successful build. Create a Pull Request to see it working. |10|



# DevOps Challenge \#4 - Build Configuration for CI #
In this challenge, you will set up a build definition for your project and configure it for continuous integration. 
If you need help check out the [Build Configuration Hints](/BuildConfiguration/BuildConfiguration.md).
## Achievements ##
| # | Achievement   | Maximum score |
|-|-|-|
|1| Create a new build definition "CI Build" | 10 |
|1| Configure your build definition to build the ASP.NET Core website | 10 |
|1| Modify your build definiton for CI - so set the trigger to build with every new push to the master branch| 10 |
|1| Clone your build definition, call the clone "PR Build" and set the trigger to Pull Request | 10 |
|1| Modify your PR Build to run unit tests | 10 |
|1| Modify your source code locally, push the code, trigger a PR and follow the Pipeline | 10 |

## Bonus Goals ##
| # | Bonus Goal | Maximum score |
|-|-|-|
|1| Create a private build agent (e.g. on your local machine or any VM) and spin it up so it is connected to your account. (You can find the required agent application in your VSTS portal for download). | 10 |
|1| Modify your CI build to create a work item on failure. | 10 |



# DevOps Challenge \#5 - Release Management #
In this challenge, you will release your application to Azure. If you need help check out the [Release Management Hints](/ReleaseManagement/ReleaseManagement.md).
## Achievements ##
| # | Achievement   | Maximum score |
|-|-|-|
|1| Create a release definition which will be triggered automatically after a successful build of "CI build". | 30 |
|1| Add a task to deploy the required infrastructure on Azure. Use the ARM Template provided  in /env/Templates/FullEnvironmentSetupMerged.json and also use the provided parameters file in the same folder. Overwrite the parameters as required. (See hints.)  | 10 |
|1| Modify your release definition to deploy your application. Use task "Azure Deploy App Service". Use your the name of your website as App Service Name. Pick to deploy to slot "Dev". *Hint: You can use variables for the values provided. Typically you'd work with values provided by a dropdown list. In our case those values might not exisit yet, so we have to provide them manually.*| 10 |
|1| Modify your code locally, push the code and watch the pipeline. | 10 |
|1| Create another release environment which deploys to another deployment slot. | 10 |

## Bonus Goals ##
| # | Bonus Goal   | Maximum score |
|-|-|-|
|1|Add a 3rd deployment slot called "Test" by modifiying your ARM template accordingly.|50|


# DevOps Challenge #6 - Automated Testing #
In this challenge, you will integrate automated tests into your application.
If you need help check out the [Auto Test Hints](/AutoTest/AutoTest.md).

## Achievements ##
| # | Achievement   | Maximum score |
|-|-|-|
|1|  Create an automated performance test for the start page of your website which will be executed after deploying to environment "Dev". Configure it to simulate 100 users over 2 minutes. Configure it to fail if response times are larger then 5 seconds. *Hint: There's a task which will help you.*| 10 |
|1|  Create a (multi-step) cloud based load test for your website which will be executed after release to test environment.Use the loadtest provided. | 10 |


## Bonus Goals ##
| # | Bonus Goal   | Maximum score |
|-|-|-|
|1| Visual Studio users only: Use VS to record a new webtest and use it during release. | 10 |

# DevOps Challenge #7 - Application Monitoring #
In this challenge, you will set up monitoring for your application in Azure.
If you need help check out the [Application Monitoring Hints](/ApplicationMonitoring/ApplicationMonitoring.md).
## Achievements ##
| # | Achievement   | Maximum score |
|-|-|-|
|1| **Understanding Application Insights**: Find the Application Insights (AI) component(s) for your app in Azure portal. Search for the different instances of AI for your slots. Check the default charts and take a look at how to create own charts. Search for the Application ID and the instrumentation key which "wire up" your application with correspondig telemetry services. Try to understand how the wiring works under the hood for the different slots. | 30 |
|1| **Deployment Markers:** You want to be able to see application releases in your AI charts. Add Release Annotations by adding a new task in your release definition for every environment. 
|-| What could you do to avoid doing modifications like this for every environment?||
|-| What is the problem with specifying an AppID in the task? How could you solve this problem? (You don't have to solve it, but think about how to solve it.) | 30 |
|1| **Custom Server Telemetry:** Collect a custom telemetry event in your webpage for whenever someone triggers a product search. Collect the time it takes to run the search. *Hint: ApplicationInsights is already pre-wired. All you have to do ist specify the line of code in SearchController.cs. You can check the OrdersController.cs file which is already tracing for code snippets. See hint file for details.* | 50 |
|1| **Custom Client Telemetry:**  Instrument your client Web Pages. Add a code snippet to track usage of the carousel found on the home page. Being responsible for the website you might want to know: Are customers actually using the option to flip through offerings? *Hint: Application Insights is already pre-wired. All you have to do is to specify the logging with a small Java Script snippet. You can check **/Views/ShoppingCart/Index.cshtml** for an analog procedure or check the hints file.* | 50 |
|1| **View AI logs & analytics:** Now re-deploy your application and use it to see if data is being logged. View the Azure portal to find the logs in the correspoding AI component. You don't have to deploy to every slot for this exercise. In your AI portal check the analytics button to run some SQL-like queries.   | 20 |
|1| **Custom Charts** Create charts in the metrics explorer to display your new metrics. |10| 
|1| **Availability Test:** Add an Availability test in Azure Portal from 5 locations in a 5 min frequency with dependencies; Match content for a string found in your startpage. Set alerts to send you an email. Provoke an error.| 20 |
|1| **Work Item Creation:** Find the place to create a work item from AI in Azure Portal. Configure the settings to create a Work Item in your VSTS project. | 10 |
|1| **Dashboard** Adjust your VSTS dashboard to show AI metrics. | 10 |

## Bonus Goals ##
| # | Bonus Goal   | Maximum score |
|-|-|-|
|1| Solve the problem with the specified AppId in the Release Annotation task. | 100 |


# DevOps Challenge 8 - Containers #
In this challenge, you will create a pipeline for container deployment. If you need help check out the [Container Hints](/Containers/Containers.md).
## Achievements ##
| # | Achievement   | Maximum score |
|-|-|-|
|1| "Dockerize your application" by creating a Dockerfile for it. You don't have to have Docker installed to create a Dockerfile. In doubt, check the hints file. | 10 |
|1| In Azure Portal create an Azure Container Registry.|10|
|1| Create a new build definition in VSTS for your application which creates a container image.| 10 |
|1| Extend your pipeline to automatically deploy your image into your container registry. |10|
|1| If you have Docker installed, run the image locally and pull it from your Azure Registry. |10|
|1| Running a container locally is rather boring. Run your container image as an Azure Container Instance manually on a managed container platform. |10||1| Create a release pipeline which deploys your container to Azure Container Instances.|10|

# DevOps Challenge 9 - Start in the cloud #
In this challenge you will set up an end to end devops pipeline starting in the Azure Portal. Azure Portal can do a lot of the steps we did so far on it's own. 
If you need help check out the [Azure Portal Deployment Hints](/StartInTheCloud/StartInTheCloud.md).
## Achievements ##
| # | Achievement   | Maximum score |
|-|-|-|
|1| In Azure Portal create a new Azure Web App.| 10 |
|1| Connect it to VSTS and configure it to configure a pipeline for you.| 10 |
|1| Investigate the pipeline and trigger a release. | 10 |



