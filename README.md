Airsonic
=========

This is the fork of the original Airsonic server.
Airsonic-Advanced has several key performance and feature enhancements. It adds and supersedes several features in Airsonic.

See: https://github.com/airsonic-advanced/airsonic-advanced

Role Variables
--------------


| Parameter               | Default                        | Description                                |
|-------------------------|--------------------------------|--------------------------------------------|
| airsonic_version        | 11.0.0-SNAPSHOT.20220124042650 | Airsonic version to install                |
| airsonic_install_folder | /opt/airsonic                  | Installation location                      |
| airsonic_context_path   | /                              | Ui path where Airsonic will resist         |
| airsonic_port           | 8080                           | Server port Airsonic will listen on        |
| airsonic_user           | airsonic                       | System user Airsonic server will use       |
| airsonic_user_group     | airsonic                       | System user group Airsonic server will use |

Dependencies
------------

There are no specific dependencies. But on Debian Buster openjdk 11 will be installed instead of openjdk 17.

Example Playbook
----------------

        - name: "Install Airsonic"
          hosts: airsonic
        
          roles:
            - role: airsonic
              vars:
                airsonic_version: 11.0.0-SNAPSHOT.20220124042650
                airsonic_install_folder: /opt/airsonic

License
-------

MIT
