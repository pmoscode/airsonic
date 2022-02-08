Airsonic
=========

Installs a standalone Airsonic server.

Role Variables
--------------

version: Airsonic version to install (only semver number)

Dependencies
------------

none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

        - name: "Install Airsonic"
          hosts: airsonic
        
          roles:
            - role: airsonic
              vars:
                version: 10.6.2

License
-------

MIT
