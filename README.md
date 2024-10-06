# HHA504_assignment_functions

## 1. Deploy a Serverless Function

### GCP
![gcp-function-config](https://github.com/user-attachments/assets/012e8722-53fa-433d-8b42-b498a76aabc4)
![gcp-function-config](https://github.com/user-attachments/assets/bfbfe813-db73-4581-8f7d-d545348794b6)
![gcp-function-code/test](https://github.com/user-attachments/assets/75094897-787d-48c7-99c0-3219f10352e3)
![gcp-function-deployed](https://github.com/user-attachments/assets/f5009020-c654-4422-a7a9-6d678c8521b6)
![gcp-function-test-url](https://github.com/user-attachments/assets/b672dfa3-9b33-48b7-b97b-e6b67c121fd3)
- On GCP, I navigated to cloud run function and pressed the create function button. Next, I made the function name to reflect the assignment and left the region as us-central1 (Iowa). The trigger type by default was HTTPS, which is also what we wanted for the assignment. In the trigger section, I changed the authentication operation to allow unauthenticated invocations. Under the runtime section, for autoscaling, I changed the maximum number of instances to 3. When pressing next, I was brought to the next code step. I adjusted the runtime type to python 3.10 and edited the main.py file. For the main.py file, I changed the else and return section of the code to reflect the assignment. Then, I tested the function and made the triggering event of world for name. After pressing run test, I was able to get Hello World! as the response in the terminal. Furthermore, I deployed the function and tested the function in a Colab notebook. By using the GCP URL, I was able to get Hello World! as the response in the Colab notebook as well.

### Azure
![azure-function-config](https://github.com/user-attachments/assets/72fd4b9c-9daa-47f7-876a-8cc6370297a6)
![azure-function-config](https://github.com/user-attachments/assets/184c1898-20d6-4673-9a60-489e025b87b2)
![azure-function-config](https://github.com/user-attachments/assets/02859d77-771e-484f-9c53-1339af75f201)
![azure-function-trigger](https://github.com/user-attachments/assets/017f5df6-fd42-4bf2-9570-497e78465d10)
![azure-function-trigger](https://github.com/user-attachments/assets/58d0aa00-9750-4f61-ad3a-24eaa205101b)
![azure-function-code/test](https://github.com/user-attachments/assets/a1d7fbe4-0f8a-476a-8da8-2fee338a8022)
![azure-function-code/test](https://github.com/user-attachments/assets/cb0dd4e9-c1bb-44f9-8191-eceba21ca5e4)
![azure-function-test-url](https://github.com/user-attachments/assets/ae61e985-fa4f-4141-99af-2ee70b62fc73)
- On Azure, I navigated to function app and pressed the create function app button. I chose consumptions as the hosting plan option and configured the settings for the function app. For the basics configurations, I made sure the function app was created under the right subscription and resource group. I made the name of the function app to reflect the assignment and chose python 3.11 as the runtime stack and version. I chose East US and left the operating system as Linux. For the storage and networking section, I left everything as the default settings and options. Next, I disabled the application insights under monitoring and enabled basic authentication under deployment. After pressing create, the function app was successfully deployed. Then, when opening the function app that was just created, I navigated to the create function button under the overview section. I selected the template to be an HTTP trigger and created a name for the function while leaving everything else as the default settings and options. After pressing create, I was brought to the code and test page where edited the code script. I changed the if and return section of the code to reflect the assignment. Then, I tested the function and made the input name and world under the body section. After pressing run, I was able to get Hello World! as the output. Furthermore, I pressed the get function URL button to copy the link of the function for the purpose of testing the function in a Colab notebook. By using the Azure URL, I was able to get Hello World! as the response in the Colab notebook as well.

## 2. Create a Cron Job
![cronjob-code](https://github.com/user-attachments/assets/2381e3f1-5905-472f-a3a3-af8ce4e6c3fc)
- For the cron job code, I started by giving it a name that reflects the assignment. I wanted to schedule the task to run every day at 8am, which equates to the cron expression of "0 8 * * *". However, for the purpose of completing the assignment in a timely manner, I also added the manual trigger of workflow_dispatch to can run the task on demand. Then, the cron job will run the code for the task with the latest version of Ubuntu by using the fourth version of the checkout action. If the task is succefully executed, it will display "Scheduled task executed" in the console.

![successfully-executed](https://github.com/user-attachments/assets/c68939c1-b385-4767-a6c0-f7b2aec04a22)
- I was able to successfully run the task on the second attempt after addressing a capitalization error for a command in the yaml file.

## 3. Explore Functions as a Service (FaaS)
- Some use cases for serverless functions include event-driven applications and scheduled tasks. They provide many benefits for users and might be a cost-efficient option. There is no need to maintain an operating system and you can use any programming language to run. Additionally, you can run severless on demand rather than leaving it as always running. From completing the assignment, I did not notice any limitations, which may be due to the simplicity of the homework. However, through research, I discovered that depending on the complexity of the serverless function, limitations may include long execution times, challenges in management, and difficulties in troubleshooting. Furthermore, I realized from completing the assignment that the layout of GCP was more straightforward to navigate and configure, while Azure was more complex and sometimes confusing to navigate and configure. 
