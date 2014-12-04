ansible-crontab
=========

Data driven ansible role that manages user's crontab.


Role Variables
--------------

    # Make sure cron/crond is installed
    manage_cron: false

Example Playbook
----------------

````
- hosts: all
  roles:
   - ansible-crontab
  vars:
    crontab:
    # name of  cron job below acts as key
     Show home:
      user: root
      state: present
      job: ls -l /home
      minute: 0
      hour: 4


````


License
-------

Apache v2

Author Information
------------------

Ryan Yates
