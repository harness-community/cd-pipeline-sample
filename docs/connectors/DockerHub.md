# Docker Hub

Follow these steps to set up a Docker Connector

- Click **New Connector**.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/new-connector.png' />
- Enter `“Docker Hub”` in the **Name** field, then click **Continue**.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/docker-name.png' />
- Enter `“https://index.docker.io/v1/”` in the **Docker Registry URL** field. That ‘/v1/’ bit is the tricky part. Tripped me up the first time I worked through this, and I’m (dramatic superhero voice) Captain Canary!
- Select **DockerHub** for the **Provider Type**.
- Enter your Docker Hub username in the **Username** field, then click **Create or Select a Secret**.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/docker-details.png' />
- Select **Docker Hub Access Token**, then click **Apply Selected**.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/docker-token.png' />
- Verify that **Docker Hub Access Token** appears in the **Password** field. Then click **Continue**.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/docker-secret.png' />
- Select **Only use Delegates with all of the following tags**. Select **mern-demo** from the drop-down menu. Selecting a specific delegate can be useful in select circumstances. Like when you have many delegates or many clusters. This is how you ensure your CI work is happening in the correct cluster.
- Click **Save and Continue**.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/docker-delegate.png' />
- Wait for the test to complete, then click **Finish**.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/docker-completed.png' />
- At this point, we’ve created the Docker Hub connector. W00t! Feeling good about how to create those connectors? 