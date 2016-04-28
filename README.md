# atom-editor

This role installs and configures [Atom text editor](https://atom.io).

## Role Variables

- atom_editor.packages (_required_)
  - list of  [apm](https://github.com/atom/apm) packages you want to install
  - each item has to have key _package_name_ containing name of package

    Example:

    ~~~yaml
    atom_editor:
      packages:
        - package_name: atom-beautify
        - package_name: git-plus
    ~~~

## Example Playbook

~~~yaml
---
- hosts: localhost
  roles:
    - atom-editor
  vars:
    atom_editor:
      packages:
        - package_name: atom-beautify
        - package_name: git-plus
~~~

## License

BSD

## Author Information

- Mailo Světel — http://him.rlnd.cz
