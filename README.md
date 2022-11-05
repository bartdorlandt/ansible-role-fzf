# Poetry
Sets up fzf; fuzzy finder

## Requirements
- git

## Role Variables
Available variables are listed below, along with default values (see defaults/main.yml):

    fzf_parentdir: "{{ ansible_env.HOME }}/git"

In which the fzf repository is cloned.

## Dependencies
None

## Example Playbook

    - hosts: localhost
      roles:
        - role: bartdorlandt.fzf

or with variables:

    - hosts: localhost
      roles:
        - role: bartdorlandt.fzf
          vars:
            fzf_parentdir: "{{ ansible_env.HOME }}/something"

## License

MIT/BSD

## Author Information

This role was created in 2022 by Bart Dorlandt.