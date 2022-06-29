# m5-ansible
Module 5 ansible playbooks and supporting files

I was not able to communicate with my database, so my m5_server instance that is running was used to manually configure my database so that my web app can be evaluated.

Also, for reasons that I can't figure out, gradle will not run properly in the background, so it needs to be started from the command line in order to access the web app. Edit: this comment may not be correct.  I think that it is just taking several minutes for my server to start responding.

This package will require a variable file with two usernames and two passwords.  Usernames and passwords don't really matter since database setup isn't working. Re-running the playbooks before looking at the web app, though, may result in the web app not working as my create_secrets.yaml is writing the passwords from this file to a secret which my Java app is then accessing in order to pass to the database.

I've included a couple of files that aren't called out in the create_all.yaml file so that I can continue to work on these.

Format for ../var-file.yaml:
---
user:
  - user1
  - user2
password:
  - password1
  - password2
key:
  - keyname

