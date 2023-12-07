# Role spreadcat.timewarrior

A simple role to manage a local timewarrior installation.

## Requirements

* `gather_facts: true`
* Repository files for timewarrior either as RPM or DEB package.
* Provide the `become` password so that the role can elevate the rights where needed.

## Role Variables

For a list of variables, their settings and examples please see [`./defaults/main.yml`](./defaults/main.yml).

The main parameters you want to probably set are:

* `timewarrior_config`
* `timewarrior_locales`
* `timewarrior_extensions`

## Other Variables

Any other variable is documented in [`./vars/main.yml`](./vars/main.yml).

## Dependencies

No other roles are required.

## Example Playbook

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

```yaml
- hosts: all
  gather_facts: true
  roles:
    - role: spreadcat.timewarrior
      timewarrior_config:
        verbose: "yes"
      timewarrior_locales:
        - nb_NO
      timewarrior_exstensions:
        - ./files/timewarrior/tmw_extension.py
```

## Limitations

* The role does not support configuring a work week in the configuration file.

## License

MIT

## Author Information

This role was developed and is maintained by dbv <dbv.github@micronarrativ.org>.
