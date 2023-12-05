# Role spreadcat.timewarrior

A simple role to manage a local timewarrior installation.

## Requirements

* `gather_facts: true`
* Repository files for timewarrior either as RPM or DEB package.

## Role Variables

For a list of variables, their settings and examples please see [`./defaults/main.yml`](./defaults/main.yml).

The main parameters you want to probably set are_

* `timewarrior_config`
* `timewarrior_locales`
* `timewarrior_extensions`

## Other Variables

Any other variable is documented in [`./vars/main.yml`](./vars/main.yml).

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in
regards to parameters that may need to be set for other roles, or variables
that are used from other roles.

## Example Playbook

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

```yaml
- hosts: localhost
  gather_facts: false
  connection: local
  roles:
    - role: spreadcat.timewarrior
      x: 42
```

## License

MIT

## Author Information

An optional section for the role authors to include contact information,
or a website (HTML is not allowed).

This role was created and is maintained by Daniel Buøy-Vehn.
