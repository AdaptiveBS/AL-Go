# #4 Create a release of your application
*Prerequisites: A completed [scenario 3](RegisterSandboxEnvironment.md)*

1. On github.com, open **Actions** in your project and select **Create Release**. Choose **Run workflow**. Enter 1.0 as **name** and **tag** of the release, and then choose **Run workflow**.
![Run workflow](images/4a.png)
1. When the **create release** workflow completes, choose the **Code** section to see the releases.
![Run workflow](images/4b.png)
1. Choose the release (1.0) and you will see the release. The release notes are pulled from all pull-requests checked in since the last release. The auto-generated release note also contains a list of the new contributers and a link to the full changelog. Choose the **Edit** button (the pencil) to modify the release notes. At the bottom, you can see the artifacts published, both the apps and the source code. A tag is created in the repository for the release number to always keep this.
![Run workflow](images/4c.png)
1. Under **Actions**, select the **CI/CD** workflow and choose **Run workflow** to kick off a new CI/CD workflow. After the CI/CD workflow finishes, you can inspect the workflow output to see that the latest release was used as a baseline for the upgrade tests in the pipeline. You will also see that the new build, just created was deployed to the QA environment automatically.
![Run workflow](images/4d.png)

---
[back](../README.md)
