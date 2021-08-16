| command        | option       | description                                                                            |
| -------------- | ------------ | -------------------------------------------------------------------------------------- |
| version        |              | Show tooling version                                                                   |
| install        | [type]       | Init Python env, install Frappe and init default site.                                 |
| docker-install | [type]       | Init Python env, install Frappe and init default site using docker.                    |
| native-bench   | [command]    | Run bench command on default site. Options: drop-site, new-site, backup, ...           |
| docker-bench   | [command]    | Run bench command on default site in docker. Options: drop-site, new-site, backup, ... |
| new-app        | [name]       | Create new Frappe app                                                                  |
| install-app    | [name]       | Install app on default site.                                                           |
| uninstall-app  | [name]       | Uninstall app on default site.                                                         |
| get-app        | [name] [url] | Install app from git url                                                               |
| start          | [option]     | Start Docker containers or benach. Options: native, db, all or docker.                 |
| restart        |              | Restart Docker containers                                                              |
| stop           | [option]     | Stop Docker containers or docker bench. Options: docker, all.                          |
| kill           |              | Remove Docker containers                                                               |
| clear-cache    |              | Clear cache for all sites.                                                             |
| upgrade        |              | Upgrade Frappe bench.                                                                  |
