plexmediaserver
=========

Installs and updates Plex Media Server using the plexupdate.sh script by Henric Andersson.

Requirements
------------

None.

Role Variables
--------------

| Variable | Description | Default |
|----------|-------------|---------|
| plexupdate_install_dir | Where to install plexupdate | '/opt/plexupdate' |
| plexupdate_repo | URL to plexupdate repo | 'https://github.com/mrworf/plexupdate.git' |
| plexupdate_AUTODELETE | plexupdate: Delete downloaded package after using | yes |
| plexupdate_AUTOINSTALL | plexupdate: Install downloaded package | yes |
| plexupdate_AUTOSTART | plexupdate: Start Plex Media Server after installing/updating | yes |
| plexupdate_AUTOUPDATE | plexupdate: Make plexupdate automatically update itself | yes |
| plexupdate_CHECKUPDATE | plexupdate: Check for updates only | no |
| plexupdate_DOWNLOADDIR | plexupdate: Download location | null |
| plexupdate_FORCE | plexupdate: Download even if it's already been downloaded | no |
| plexupdate_NOTIFY | plexupdate: Notify user if we downloaded/installed something | yes |
| plexupdate_PLEXSERVER | plexupdate: IP of Plex Server | 127.0.0.1 |
| plexupdate_PLEXPORT | plexupdate: TCP Port of Plex Server | 32400 |
| plexupdate_PUBLIC | plexupdate: Use pulic (non-plexpass) version | no |
| plexupdate_TOKEN | plexupdate: Plex login credential token | null |

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: plexservers
      roles:
         - { role: TheRealJohnDavies.plexmediaserver }

License
-------

GPLv2

Author Information
------------------

John Davies

