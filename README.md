# Ferdi

This role handles installing Ferdi using an RPM.

## Requirements

None

## Role Variables

| Variable          | Required | Default          | Description                                                                                                                                                                                                  |
| ----------------- | -------- | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ferdi_version     | &#9989;  | `latest`         | Using `latest` will always download the latest version erdi. You can select a specific version from the Ferdi [releases page](https://github.com/getferdi/ferdi/releases) (i.e. Ferdi 5.5.0 would be v5.5.0) |
| ferdi_install_dir | &#9989;  | `~/Applications` | The location to place the Ferdi AppImage                                                                                                                                                                     |

## Dependencies

None

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: jaredhocutt.ferdi
      vars:
         ferdi_version: v5.5.0
```

## License

MIT

## Author Information

Jared Hocutt (@jaredhocutt)
