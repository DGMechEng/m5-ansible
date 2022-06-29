# m5-ansible
Module 5 ansible playbooks and supporting files

I was not able to communicate with my database, so my m5_server instance that is running was used to manually configure my database so that my web app can be evaluated.

This package will require a variable file with two usernames and two passwords.  Usernames and passwords don't really matter since database setup isn't working.

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

