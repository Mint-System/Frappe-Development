| command            | option       | description                                                                                    |
| ------------------ | ------------ | ---------------------------------------------------------------------------------------------- |
| version            |              | Show tool versions.                                                                            |
| install            | [type]       | Init Python env, install Frappe and init default site.                                         |
| install-docker-dev | [type]       | Install Docker Development environment.                                                        |
| native-bench       | [command]    | Run bench command on default site. Options: drop-site, new-site, backup, ...                   |
| docker-bench       | [command]    | Run bench command on default site in docker. Options: drop-site, new-site, backup, ...         |
| new-app            | [name]       | Create new Frappe app                                                                          |
| install-app        | [name] [url] | Install app from git url.                                                                      |
| uninstall-app      | [name]       | Uninstall app on default site.                                                                 |
| docker-install-app | [name] [url] | Install app from git url on Docker container.                                                  |
| start              | [option]     | Start Docker containers or bench. Options: dev, bench, native, db, site, worker, nginx or all. |
| restart            |              | Restart Docker containers.                                                                     |
| stop               |              | Stop Docker containers.                                                                        |
| stop-bench         |              | Stop Docker development server.                                                                |
| kill               |              | Remove Docker containers.                                                                      |
| kill-dev           |              | Remove Docker development containers.                                                          |
| logs               |              | Show log for frappe-python Docker container.                                                   |
| clear-cache        |              | Clear cache for all sites.                                                                     |
| upgrade            |              | Upgrade Frappe bench.                                                                          |
| source             |              | Source the Python virtual env.                                                                 |
