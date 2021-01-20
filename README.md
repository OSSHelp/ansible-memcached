# memcached

[![Build Status](https://drone.osshelp.ru/api/badges/ansible/memcached/status.svg)](https://drone.osshelp.ru/ansible/memcached)

Simple role, which installs memcached

## Usage (example)

Install and configure:

```yaml
    - role: memcached
```

Configure only:

```yaml
    - role: memcached
      memcached_setup: configure
```

## Available parameters

### Main

| Param | Default | Description |
| -------- | -------- | -------- |
| `memcached_setup` | `full` | Setup mode. See [OSSHelp KB article](https://oss.help/kb4895) |
| `memcached_memory` | `64m` | Memcached memory size |
| `memcached_port` | `11211` | Memcached listen port |
| `memcached_listen` | `0.0.0.0,::` | Memcached listen addr |
| `memcached_connlimit` | `1024` | Memcached connection limit |
| `memcached_threads` | `4` | Memcached threads |
| `memcached_debug` | `false` | Memcached log verbosity |

### Misc

| Param | Default | Description |
| -------- | -------- | -------- |
| `memcached_packages` | `memcached` | Packages |
| `memcached_conf_path` | `/etc/memcached.conf` | Memcached config path |
| `memcached_pid_file` | `/var/run/memcached/memcached.pid` | Memcached pid file |
| `memcached_drop_in_path` | `/etc/systemd/system/memcached.service.d` | Systemd override directory |
| `memcached_drop_in_conf` | `override.conf` | Systemd override file |

## FAQ

...

## Useful links

- [Official page](https://memcached.org/)
- [Official documentation](https://github.com/memcached/memcached/wiki)
- [OSSHelp KB Articles](https://rm.osshelp.ru/projects/support-servers/search?utf8=%E2%9C%93&q=memcached&scope=&all_words=&titles_only=&titles_only=1&kb_articles=1&attachments=0&options=0&commit=%D0%9F%D1%80%D0%B8%D0%BD%D1%8F%D1%82%D1%8C)

## TODO

- ...

## License

GPL3

## Author

OSSHelp Team, see <https://oss.help>
