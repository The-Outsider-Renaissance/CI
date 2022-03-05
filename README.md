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

<details>
<summary><b>Optionally: Installing Vault (Click here)</b>
</summary>

### Requirements (MacOS/Darwin)

- [jq]()
- [Vault's CLI]()

To install Vault:
```sh
task vault
# Then follow instructions that may appear on terminal and afterward
task vault:set # To configure a sample kv secret
```

---

</details>

After successfully initializing the local cluster, you must install one of the provided CI tools:

- To install Drone:
```sh
task drone:install
```

- To install Concourse CI:
```sh
task concourse:install
```

- To install Jenkins:
```sh
task jenkins:install
```