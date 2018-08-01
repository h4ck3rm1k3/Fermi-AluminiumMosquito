# Fermi-AluminiumMosquito
Codename : FermiAluminiumMosquito 

Package to manage my personal git repositories.

Submodules :
A. SSH
B. GIT
D. Linux Shell Commands
D. Linux Filesystem

Implementation :
Ansible/Paramiko

Integrations :
I1. Archive.org
I2. GITHUB
I3. Travis
I4. CircleCI

Rough requirements

1. run on multiple computers
1.1 manage a list of computer resources that are available, use ssh agent to access them to begin with.
1.2 mangage port forwarding.
1.3 manage remote deployment like ansible, use ansible where it makes sense.

2. inventory git and other repos lying around.
2.1 run `locate .git ` to start with to get a list of git repositories
2.2 interpret git config files in directories.
2.3 allow for saving repository information in the database as well as build status on a given machine.

3. inventory requirements
collect needed modules for a given package

4. manage submodules
5. capture data that is not checked in and move to archive.org
6. remove sensitive data.
7. be able to reproduce environment on another machine.
8. be able to run builds and collect build artifacts.
9. run tests and test artifacts.
10. run introspection and inspections on process and collect artifacts as needed in standard manner.
11. use standard automake, python, cmake, files.
12. interpret travis and circle ci files.
13. manage git pulls and integrations.
14. interface with git and provide a remote api that mirrors git
15. create a remote CLI that can do all the commands remotely that you can do via the api.
16. provide a swagger api
