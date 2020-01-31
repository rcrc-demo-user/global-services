## Role profiles

1. Check that the sector page has the "Rapid response personnel" section enabled.
   - The sector pages are inside the 2-letter language folders inside the `/app/` [folder](https://github.com/IFRCGo/global-services/tree/publish/app) (for example, `/app/en/` and `/app/es/`).
   - If it is enabled, there will be a `{% include sector-rrp.html %}` line. See the `/app/en/livelihoods.html` [file](https://github.com/IFRCGo/global-services/blob/publish/app/en/livelihoods.html#L8) file for an example.
1. The profiles are updated through the language files in the `/app/_data/` [folder](https://github.com/IFRCGo/global-services/tree/publish/app/_data). Click into the language you want to update, for example the `en.yml` [file](https://github.com/IFRCGo/global-services/blob/publish/app/_data/en.yml)for English.
1. Click the top-right pencil icon to **Edit the file in your fork of this project**.
   - ![](https://raw.githubusercontent.com/IFRCGo/global-services/publish/contributing/img/GitHub--edit-the-file.png) 
1. In the window that opens, scroll down below the sectors section header: 
    ```plain
      #############
      ## SECTORS ##
      #############
    ```
1. Find the sector you want to edit. They will be listed as a short identifier such as `comms` and `opsmanagement`. 
1. Create a list item with `name` and `link` for each role profile.
   - The indentation and spacing of new items needs to match how it is for the others in the file.
   - The `link:` value should be the exact filename (we'll upload it soon). You can leave it blank if you want to list the profile name but aren't ready with the file yet and we'll automatically include a "coming soon" note on the website.
    ```plain
      role-profiles:
        - name: "My Sector Coordinator"
          link: "My Sector Coordinator - profile - 20200130.pdf"
        - name: "My Sector Officer"
          link: 
    ```
1. When you're done editing, scroll to the bottom. In the **Propose file change** box add a short description of your edit, then click **Propose file change**.
   - ![](https://raw.githubusercontent.com/IFRCGo/global-services/publish/contributing/img/GitHub--propose-file-change.png) 
1. On the page that loads, you'll be able to review your changes. Click the green **Create pull request** button, on the next page you'll have the opportunity to add more details if needed, make sure that **Allow edits from maintainers.** is checked, and then click the green **Create pull request** button.
   - ![](https://raw.githubusercontent.com/IFRCGo/global-services/publish/contributing/img/GitHub--comparing-changes.png) 
1. If you need to add files, look for the **...wants to merge** message and click the second link that includes your user name. If not, you can skip to step 16.
   - ![](https://raw.githubusercontent.com/IFRCGo/global-services/publish/contributing/img/GitHub--merge-locations.png)  
   - Click the link and notice that the URL changes from something like `https://github.com/IFRCGo/global-services/pull/2` to something like `https://github.com/rcrc-demo-user/global-services/tree/patch-1`. Earlier there was a message about "your fork of this project". You're now on your fork.
1. Click into the `/app/` folder, then `/assets/`, then `/docs/`, then the folder for the sector you would like to upload documents.
1. Once inside the folder (for example, `https://github.com/rcrc-demo-user/global-services/tree/patch-1/app/assets/docs/logs`) click the **Upload files** button.
1. You can add multiple documents. Add only documents for the sector that you are in. After you've added all the sector files, add a short description of your upload, and then click **Commit changes**.
   - ![](https://raw.githubusercontent.com/IFRCGo/global-services/publish/contributing/img/GitHub--add-files.png)  
1. To add more documents for another sector, go back to step 10.
1. If you are done uploading documents, you can go back to the IFRC version of the project. At the top left of the browser window, click the link for `IFRCGo/global-services`.
   - ![](https://raw.githubusercontent.com/IFRCGo/global-services/publish/contributing/img/GitHub--fork-navigation.png)   
1. Click the **Pull requests** navigation tab, and then click on the item for your open pull request.
   - ![](https://raw.githubusercontent.com/IFRCGo/global-services/publish/contributing/img/GitHub--open-pull.png)  
1. You should see a list of all your edits.
   - ![](https://raw.githubusercontent.com/IFRCGo/global-services/publish/contributing/img/GitHub--two-commits.png) 
1. If you're ready for your changes to be added to the website, you can add a short message at the bottom and click **Comment** to let a maintainer know.
   - ![](https://raw.githubusercontent.com/IFRCGo/global-services/publish/contributing/img/GitHub--ready-to-merge.png) 
