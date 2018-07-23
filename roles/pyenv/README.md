pyenv
=========

This role will setup pyenv on a server, install required python version,
create virtualenv, and install requirements.

Requirements
------------

None

Role Variables
--------------

Refer to `defaults/main.yml`

Dependencies
------------

None

Example Playbook
----------------

    - name: setup pyenv and install python env
      hosts: ubuntu
      roles:
        - {
            role: pyenv,
            shell_rc: "~/.zshrc",
            python_version: "3.6.5",
            virutalenv_name: "myenv",
            requirements_path: "files/requirements.txt"
          }

License
-------

MIT

Author Information
------------------

Guo Qiao(Joe), a Python Developer working in New Zealand.
