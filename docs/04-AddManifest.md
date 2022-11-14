# Adding Manifest

Now you have the pipeline imported and ready. Let's configure it by adding a manifest.

## Follow these steps to add a Manifest
***

- Click on the **edit** button on the manifest.
- Now select the **git connector** we had created before in the beginning. Also, we can create a new connector on the go as well.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/manifest-1.png' />
- Check the Manifest Details : 
	- **Identifier** : manifest, 
	- **Branch** : main, 
	- **File/Folder Path** : default-k8s-manifests/Manifests/Files/templates
- Click **Submit**.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/values.png' />
- Now edit the **second manifest** as we need to add the **values.yaml**.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/values-manifest.png' />
- This time select **Values YAML** and **continue**.
<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;width:90%;" src='../../Images/manifest.png' />
- Check In the manifest details : 
	- **Manifest Identifier** : values, 
	- **Branch** : main, 
	- **File Path** : default-k8s-manifests/Manifests/Files/ng_values_dockercfg.yaml
- Click **Submit**

Let's [add the artifacts](docs/project/AddArtifacts.md) now