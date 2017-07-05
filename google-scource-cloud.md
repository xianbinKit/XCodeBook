# XCode with Google Source Cloud

##### Original inscructions of Google

```
https://cloud.google.com/source-repositories/docs/adding-repositories-as-remotes

```

Follow the inscructions above to create your google project and configurate with google source cloud.

##### Init a gcloud project in your local directory

```
cd [LOCAL_DIRECTORY]
gcloud init
gcloud source repos clone [REPO_NAME]
```

!!! the \[REPO\_NAME\] is repository name in first step but not the project name!

##### Create a XCode project and copy the contents of project into your \[LOCAL\_DIRECTORY\]



##### Configure remote project url

```
git remote add origin https://source.developers.google.com/p/[PROJECT_ID]/
```

difference to the google instructions, here change google to orogin as above. XCode prefer origin

the https need to be the clone URL of repository, but not exactly as above.

##### Configure  credential 

```
git config credential.helper gcloud.sh
```

this is something like ssl, the username is still your google account email, but the password will generated automatically.

##### Configure XCode \(XCode 9.0\)

Open XCode project, XCode will recognize git project automatically, try to push, then you get an error fail with a http link.

Open the link, follow the inscrctions, you will get a report with password.

**Reopen** XCode, try to push again, you can retry username and password, use the password you just got.





