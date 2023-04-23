## Configure Webhook to trigger CI Pipeline automatically on every change

### Technologies used:

Jenkins, GitLab, Git, Docker, Java, Maven

Project Description:

Install GitLab Plugin in Jenkins

Configure GitLab access token and connection to Jenkins in GitLab project settings

Configure Jenkins to trigger the CI pipeline, whenever a change is pushed to GitLab

### Project Description:

Install GitLab Plugin in Jenkins

Configure GitLab access token and connection to Jenkins in GitLab project settings

Configure Jenkins to trigger the CI pipeline, whenever a change is pushed to GitLab

Here's a step-by-step guide on how to configure a webhook to trigger a CI pipeline automatically on every change in GitLab using Jenkins:

Step 1: Install GitLab Plugin in Jenkins

In your Jenkins instance, navigate to "Manage Jenkins" > "Manage Plugins" > "Available" tab.

Search for "GitLab Plugin" and select it.

Click on the "Install without restart" button to install the plugin.

Once the installation is complete, Jenkins will restart.

Step 2: Configure GitLab access token and connection to Jenkins in GitLab project settings

Go to your GitLab project's settings in your GitLab instance.

Under "Integrations", select "Jenkins" from the list of available integrations.

Enter the Jenkins URL in the "Jenkins URL" field. This should be the URL of your Jenkins instance.

If you want to use an access token for authentication, enter the access token in the "Token" field. Alternatively, you can also use the username and password fields for authentication.

Check the "Active" checkbox to enable the integration.

Click on the "Add Webhook" button to save the settings.

Step 3: Configure Jenkins to trigger the CI pipeline on every change

In your Jenkins instance, navigate to your Jenkins job that represents your CI pipeline.

Click on "Configure" to edit the job.

Under the "Build Triggers" section, check the "Build when a change is pushed to GitLab" checkbox.

Configure the "Project URL" field to match the URL of your GitLab project. This should be in the format "https://<gitlab-instance-url>/<namespace>/<project-name>".

Click on "Save" to save the job configuration.

Step 4: Test the webhook

To test the webhook, make a change in your GitLab project, such as pushing a commit or merging a merge request.

Check the "CI/CD" > "Pipelines" section in your GitLab project to see if the pipeline is triggered.

Go to your Jenkins instance and check the "Build History" of your CI pipeline job to see if a new build is triggered automatically.

That's it! Now your Jenkins CI pipeline should be triggered automatically on every change in your GitLab project, thanks to the webhook integration between GitLab and Jenkins. Make sure to review and verify your pipeline configuration and settings to ensure smooth and successful pipeline executions.
