## How to create a local cluster

### Requirements:

- [Task](https://taskfile.dev)
- [Docker](https://docker.com)
- [k3d](https://k3d.io/v5.3.0/) <sub> (Higher than v5.0) </sub>
- [kubectl]()
- [Helm]()

### Instructions

Type the following command to delete any previous resources and start a new local cluster:

```bash
task
```

---

After successfully initializing the local cluster, you must install one of the provided CI tools:

- To install Drone:
```sh
task drone:install
```

- To install Concourse CI:
```sh
task concourse:install
```

- To install Argo Workflow:
```sh
task argo:install
```

- To install Gitlab:
```sh
task gitlab:install
```