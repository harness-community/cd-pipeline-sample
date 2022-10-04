# GitHub Personal Access Token   

Harness needs a [**Personal Access Token**](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to access GitHub repositories. 

Refer to the **[Add a GitHub Connector documentation](https://ngdocs.harness.io/article/jd77qvieuw-add-a-git-hub-connector#step_3_credentials)** for how to generate the token or follow the steps given below :arrow_down_small: 

- Login to GitHub and click on Settings from the top-right menu
- Select **Developer Settings** from the list of Account Settings
- Select **Personal access tokens** 
- Click on **Generate new token** (grant ALL permissions)
- Copy the generated token and save it.
- Click **New Secret**, then select **Text**. 
- *image to be inserted*
- Enter “GitHub Personal Access Token” in the **Secret Name** field.
- Enter your `Personal Access Token` in the **Secret Value** field, then click **Save**.

Easy peasy lemon squeezy! Right? :lemon: 

Ok, now if you’re feeling like you’ve got this, feel free to jump over to Harness and add two more secrets:

- A text secret called ‘**Docker Hub Access Token**’ (Again, our crack team of naming specialists is top notch!) populated with your `Docker Hub access token`.
- Create a new **Docker connector** (under PROJECT SETUP select Connectors)   
    - Overview  

        **Name the connector**: Harness-Docker 
        **Details**  
        **URL**:  https://registry.hub.docker.com/v2/  
        **Provider type**: DockerHub  
        **Authentication**: Anonymous (no credentials required)  
        **Delegates Setup**: Use any available Delegate




