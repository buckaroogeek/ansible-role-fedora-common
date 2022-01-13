Fedora Common
=========

A collection of utility tasks that help set up and configure a fedora machine. Examples include a fail fast check for a fedora host and an option to disable zram swap.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

End user configurable variables are listed below, along with default values (see `defaults/main.yaml`):

| Variable   | Default Value | Notes |
| ---------- | ------------- | ----- |
| fc_disable_zram | false | Disable zram swap |

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      tasks:
      - name: "Include fedora_common"
        include_role:
          name: "fedora_common"
        vars:
          fc_disable_zram: true

License
-------

BSD

Author Information
------------------

Author: Brad Smith
Email: bradley.g.smith@gmail.com
