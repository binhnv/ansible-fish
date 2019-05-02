# ansible-fish

Install fish via Homebrew.

## Role Variables

* `fish_default_shell`: Set `fish` as default shell. Defaults to `true`.
* `fish_install_omf`: Install Oh-My-Fish. Defaults to `true`.
* `fish_users`: A list of dictionary of user information. Defaults to
  ```
  name: "{{ ansible_user_id }}"
  omf_location: "{{ ansible_user_dir }}/.local/share/omf"
  ```

## Dependencies

There is no dependency for this role. But some package managers are required
* `Homebrew` if using macOS

## Example Playbook

```
  - hosts: all
    roles:
      - role: binhnv.fish
```

## License

MIT
