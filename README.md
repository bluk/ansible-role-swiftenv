ansible-role-swiftenv
==================

An [Ansible][ansible] role to install [swiftenv][swiftenv].

Requirements
------------

1. Add `swiftenv` to your `$PATH` after install.

```
echo 'export PATH="$HOME/.swiftenv/bin:$PATH"' >> ~/.bash_profile
```

2. Run the following:

```
~/.swiftenv/bin/swiftenv init
```

Role Variables
--------------

* `swiftenv_install_path` - The path to install `swiftenv`.

* `swiftenv_git_url` - The git URL to clone `swiftenv` from.

* `swiftenv_git_update` - If the cloned `swiftenv` git repository should be updated.

Dependencies
------------

No dependencies.

Example Playbook
----------------

```
- hosts: servers
  roles:
     - { role: bluk.swiftenv }
```

License
-------

[Apache-2.0][license]

[license]: LICENSE
[ansible]: https://www.ansible.com
[swiftenv]: https://github.com/kylef/swiftenv
