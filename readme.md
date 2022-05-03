# Change ports Bind

Alter bind ports for image after running command 

```bash
  docker container run
```

1. First step
Stop the image in running

```bash
  docker stop <container-name/container-id>
```

2. Alter file config container

Edit hostconfig.json and config.v2.json files of the respective container by adding your port to PortBindings key and ExposedPorts key respectively.
file::*/var/lib/docker/containers/<container-id>*

permission need root

3. Start container

```bash4
  docker start <container-name/container-id>
```


