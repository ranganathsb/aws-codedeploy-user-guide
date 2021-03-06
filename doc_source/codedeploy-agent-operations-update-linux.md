# Update the AWS CodeDeploy Agent on Amazon Linux or RHEL<a name="codedeploy-agent-operations-update-linux"></a>

After the AWS CodeDeploy agent \(`codedeploy-agent.noarch.rpm`\) is installed on an instance, it will be updated automatically within 24 hours of the release of a new version\. The update time cannot be easily cancelled or rescheduled\. If a deployment is in progress during the update, the current deployment lifecycle event will finish first\. After the update is complete, the deployment will resume with the next deployment lifecycle event\.

If you want to force an update of the AWS CodeDeploy agent, sign in to the instance, and run the following command:

```
sudo /opt/codedeploy-agent/bin/install auto
```