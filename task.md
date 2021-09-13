| command            | option       | description                                                                                    |
| ------------------ | ------------ | ---------------------------------------------------------------------------------------------- |
| version            |              | Show tool versions.                                                                            |
| install            | [type]       | Init Python env, install Frappe and init default site for native environment.                  |
| install-docker-dev | [type]       | Install Docker Development environment.                                                        |
| bench-native       | [command]    | Run bench command on native environment.                                                       |
| bench-docker       | [command]    | Run bench command on Docker environment.                                                       |
| bench-docker-dev   | [command]    | Run bench command Docker development environment.                                              |
| new-app            | [name]       | Create new Frappe app in the native environment.                                               |
| install-app        | [name] [url] | Install app from git url for native environment.                                               |
| uninstall-app      | [name]       | Uninstall app in the native environment.                                                       |
| docker-install-app | [name] [url] | Install app from git url on Docker environment.                                                |
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
