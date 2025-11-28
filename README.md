# QixOS Core System Modules

System configuration modules for QixOS.

## Modules

- `system/boot/` - Boot loader configuration
- `system/network/` - Networking setup
- `services/` - System services
- `hardware/` - Hardware configuration
- `security/` - Security & firewall

## Usage
```qix
# In your system configuration
imports = [
  <qixos-core/modules/services/openssh.qix>
  <qixos-core/modules/system/boot/systemd-boot.qix>
];

services.openssh = {
  enable = true;
  permitRootLogin = false;
};
```

## License

MIT
