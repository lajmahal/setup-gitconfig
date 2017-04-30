setup-gitconfig
=========

Generates the gitconfig. Ensures your build server will always use the correct name and email address when interacting with git repos with strict commit hooks.

Role Variables
--------------

* `gitconfig_name` - The name to use on the commits.
* `gitconfig_email` - The email address to use on the commits.

Example Playbook
----------------
    - hosts: localhost
      vars:
        gitconfig_name: "John Doe"
        gitconfig_email: "john.doe@email.com"
      roles:
         - setup-gitconfig
