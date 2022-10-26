# Traps Generic
SNMP traps can be used to gain more details about the health state of your network devices. By adding event-based data to all the metrics reported by a dedicated SNMP extensions, you are able to diagnose the performance and availability issues even better.

**Use Cases**

- Track number of traps reported by their types, so that you can enable alerting for issues such as port flapping
- Review individual events reported by the SNMP devices, so that you have more details explaining metric anomalies

## Dev

### Prerequisites
- Nix-capable environment, for Windows that means [installing WSL](https://docs.microsoft.com/en-us/learn/modules/get-started-with-windows-subsystem-for-linux/2-enable-and-install)
- [nix](https://nixos.org/download.html) / [**nix for WSL**](https://nixos.org/download.html#nix-install-windows)
- Docker (available in the same environment as nix, required for running companions)

Hint: if something doesn't work because of missing package please add the package to `default.nix` instead of installing on your computer. Why solve the problem for one if you can solve the problem for all? ;)

### Everything
```
nix-shell
# caution! if this is your first pull of first extension ever this might take some time
# depending on your network connection
# after it completes: inside the shell
make help
```

### Resources
- [Extension yaml docs](https://www.dynatrace.com/support/help/extend-dynatrace/extensions20/extension-yaml)
- [Extension knowledge base](https://www.dynatrace.com/support/help/extend-dynatrace/extensions20)

### Convinience
This section is entirely **optional**. The repository contains additional amenities, but they're not so straightforward, so we don't recommend them for begginers.  Anyway, you might also like:
- [`direnv`](https://direnv.net/) (which can be installed easily via `nix-env -iA nixpkgs.direnv`)

### Internal tooling
If you're a **Dynatrace employee** you can follow [this link](https://github.com/dynatrace-extensions/precious-toolz-internal) to enable internal tooling