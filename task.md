| command | option       | description                                                                              |
| ------- | ------------ | ---------------------------------------------------------------------------------------- |
| version |              | Show tooling version                                                                     |
| install | [type]       | Init Python env, install Frappe and init default site. Use type docker for Docker setup. |
| new-app | [name]       | Create new Frappe app                                                                    |
| get-app | [name] [url] | Install app from git url                                                                 |
| start   | [name]       | Start Docker containers or by default run bench. Options: db,bench or docker.            |
| restart |              | Restart Docker containers                                                                |
| stop    |              | Stop Docker containers                                                                   |
| kill    |              | Remove Docker containers                                                                 |
