# HHA504_assignment_functions

## 1. Deploy a Serverless Function

## 2. Create a Cron Job
![cronjob-code](https://github.com/user-attachments/assets/2381e3f1-5905-472f-a3a3-af8ce4e6c3fc)
- For the cron job code, I started by giving it a name that reflects the assignment. I wanted to schedule the task to run every day at 8am, which equates to the cron expression of "0 8 * * *". However, for the purpose of completing the assignment in a timely manner, I also added the manual trigger of workflow_dispatch to can run the task on demand. Then, the cron job will run the code for the task with the latest version of Ubuntu by using the fourth version of the checkout action. If the task is succefully executed, it will display "Scheduled task executed" in the console.
![successfully-executed](https://github.com/user-attachments/assets/c68939c1-b385-4767-a6c0-f7b2aec04a22)
- I was able to successfully run the task on the second attempt after addressing a capitalization error for a command in the yaml file.

## 3. Explore Functions as a Service (FaaS)
