# Overleaf Toolkit

## Getting Started

- Run `bin/init`
  - this will populate config files in `config/`
- Run `bin/up`
  - this will start the service with docker-compose


## Doctor

Run `bin/doctor` for debug output


## Config files

- `config/docker-compose.yml`
  - base config file for docker-compose, not meant to be edited
- `config/local.yml`
  - local overrides, and environment configuration, editable


## Data directories

- `data/mongo`
- `data/redis`
- `data/sharelatex`

All are persisted outside of the containers. 


## TODO

- [ ] Improve the init script
- [ ] Investigate how we can support using external mongo/redis easily
  - Docker networking, etc
- [ ] Consistent `--help` output from each tool
- [ ] Full documentation
   - [ ] New user walkthrough
   - [ ] Documentation for each file
   - [ ] Documentation for each tool in the bin folder
