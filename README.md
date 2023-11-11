Fedora Common
=========

A collection of common settings useful across multiple Fedora related playbooks and roles.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

End user configurable variables are listed below, along with default values (see `defaults/main.yaml`):

| Variable   | Default Value | Notes |
| ---------- | ------------- | ----- |
|  |  |  |

Variables set in vars/main.yaml shown here for reference. Not intended for modification at runtime.

| Variable   | Value | Notes |
| ---------- | ------------- | ----- |
| fc_modularity | true if F38 or older | True if modularitly is available in DNF repositories. Modularity was removed in F39. |

Dependencies
------------

None

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
