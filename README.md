# ml-id-lab3
AWS Immersion Day 2019 (ML)


Create a GitHub repo and create an OAuth token

To integrate your continous delivery pipeline with GitHub, you will use OAuth tokens. Go to GitHub's Token Settings to generate your token and ensure you enable the following two scopes:

  - repo, which is used to read and pull artifacts from public and private repositories into a pipeline
  - admin:repo_hook, which is used to detect when you have committed and pushed changes to the repository

Make sure to copy your new personal access token now as you will need it later.

You will need a GitHub repo for your code. In GitHub create a new repository called "ml-id-lab3" and make sure it is public. Do not initialize with a README file and do not add any .ignore or license file. Copy your GitHub repo URL as you will need it later.

Open up a terminal (or cmd on Windows) and change directory into the directory where you extracted the Immersion Day material earlier. Now initialize your git repository by running the following command lines:

```
   cd Lab3
   git init
```

Stage your files running the following command lines:

```
   git add .
   git commit -am "First commit"
```

Set the remote origin and push the files by running the following command lines (use the GitHub repo URL from step 2):

```
   git remote add origin https://github.com/<GITHUBUSER>/ml-id-lab3.git
   git push -u origin master
```

Now validate that you have a CloudFormation directory and Source directory in your GitHub repo.
