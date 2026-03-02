# noobient.gsettings

## Synopsys

This role lets you override global defaults for GSettings.

## Parameters

| Name | Required | Example | Description |
|---|---|---|---|
| `filename` | yes | `20_corporate-settings` | Filename for GSettings overrides, without the `.gschema.override` extension. |
| `section` | yes | `org.gnome.system.smb` | GSettings section to set. |
| `option` | yes | `workgroup` | GSettings option to set. |
| `value` | yes | `AD` | GSettings value to set. |

## Examples

```yml
- include_role:
    name: noobient.gsettings
  vars:
    filename: '20_corporate-settings'
    section: 'org.gnome.system.smb'
    option: 'workgroup'
    value: "'AD'"
```

## Return Values

N/A

## Support

| Platform | Support | Status |
|---|---|---|
| Linter | ✅ | [![Lint](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/lint.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/lint.yml) |
| AlmaLinux 8 | ✅ | [![AlmaLinux 8](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/almalinux-8.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/almalinux-8.yml) |
| AlmaLinux 9 | ✅ | [![AlmaLinux 9](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/almalinux-9.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/almalinux-9.yml) |
| AlmaLinux 10 | ✅ | [![AlmaLinux 10](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/almalinux-10.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/almalinux-10.yml) |
| Fedora 42 | ✅ | [![Fedora 42](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/fedora-42.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/fedora-42.yml) |
| Fedora 43 | ✅ | [![Fedora 43](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/fedora-43.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/fedora-43.yml) |
| Ubuntu 22.04 | ✅ | [![Ubuntu 22.04](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/ubuntu-22.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/ubuntu-22.04.yml) |
| Ubuntu 24.04 | ✅ | [![Ubuntu 24.04](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/ubuntu-24.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/ubuntu-24.04.yml) |
| Ubuntu 26.04 | ✅ | [![Ubuntu 26.04](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/ubuntu-26.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gsettings/actions/workflows/ubuntu-26.04.yml) |
