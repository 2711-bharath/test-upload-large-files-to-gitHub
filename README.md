# test-upload-large-files-to-gitHub

#### Step 01

Download and install Git on your pc.

Download link:- https://git-scm.com/downloads

#### Step 02

Then download and install GitLFS on your pc.

Download link: https://git-lfs.github.com/

#### Step 03

Now clone your GitHub repository to your local machine.

#### Step 04

Go inside the cloned repository. (If you want to upload the file to another folder already created inside the repository, then go to that folder)

Right-click the background and again click ‘Git Bash Here.

Run the following command

```bash
git lfs track ".fileextension"
```

**Example for pkl**

```bash
git lfs track "*.pkl"
```

#### Step 05

After executing step 4 there .gitattributes file is generated in your local. Now push it to remote

```bash
git add .gitattributes
```

```bash
git commit -m "commit message"
```

```bash
git push
```

#### Step 06

After this, you need to add your large file to the staging

```bash
git add "filename.pkl"
```

#### Step 07

To ensure that your large file is added to staging you can track it using this command

```bash
git lfs ls-files
```

#### Step 08

Now you can commit your file and push it remote

```bash
git commit -m "commit message"
```

```bash
git push
```

#### Step 09

Now you can visit your remote repository to verify if your large file is uploaded or not
