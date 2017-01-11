# madek-instance

## quickstart

1. "Fork" this repository on github *(only required if you want to receive update notifications)*

1. clone it to a secure, backed up computer: `git clone git@github:yourUserName/madek-instance my-madek`

1. setup:
  ```
  cd my-madek
  git submodule update --init Madek
  cd Madek && git reset --hard origin/release && git submodule update --init --recursive deploy
  ```

1. configure
  - fill in hostname in file `hosts`
  - global config in file `group_vars/madek.yml`
  - per-host config in file `host_vars/madek.example.com.yml`, rename it to match the hostname
