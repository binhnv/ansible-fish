# ansible-fish

Install fish via Homebrew.

## Role Variables

* `set_fish_as_default_shell`: Defaults to `false`.

## Dependencies

* [icopp.homebrew](https://github.com/icopp/ansible-homebrew)

## Example Playbook

```
  - hosts: all
    roles:
      - role: icopp.fish
```

```
  - hosts: all
    roles:
      - role: icopp.fish
        set_fish_as_default_shell: true
```

## License

MIT
