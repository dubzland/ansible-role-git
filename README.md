# Ansible Role: Git
[![Gitlab pipeline status (self-hosted)](https://git.dubzland.net/dubzland/ansible-role-git/badges/master/pipeline.svg)](https://git.dubzland.net/dubzland/ansible-role-git)

Installs and configures Git from source.

## Requirements

Ansible 2.2 or higher.

## Role Variables

Available variables are listed below, along with their default values (see
    `defaults/main.yml` for more info):

### dubzland_git_version

```yaml
dubzland_git_version: "2.6.3"
```

Specific version of Git to install.

### dubzland_git_source_root

```yaml
dubzland_git_source_root: "/usr/local/src"
```

Directory used to store tarballs, as well as extract and build source tree.

### dubzland_git_source_url

```yaml
dubzland_git_source_url: "https://www.kernel.org/pub/software/scm/git-2.22.0.tar.gz"
```

URL used to download Git source tarball.

### dubzland_git_source_sha256sum

```yaml
dubzland_git_source_sha256sum: "a4b7e4365bee43caa12a38d646d2c93743d755d1cea5eab448ffb40906c9da0b"
```

SHA256 checksum used to validate the downloaded source tarball.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
    - role: dubzland.git
```

## License

MIT

## Author

* [Josh Williams](https://codingprime.com)
