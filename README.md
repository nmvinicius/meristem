# Meristem

A living code repository. Code is an object in a graph, history is stored change by change, and a branch is a disposable notebook.

The presentation is at https://nmvinicius.github.io/meristem/.

## Run it locally

The current snapshot is [2026.11.06](https://github.com/nmvinicius/meristem/releases/tag/2026.11.06). The archive contains the `meristem` CLI for Linux x86_64, the logical snapshot, and the two seed images.

Docker Engine, the Compose plugin, and a network connection are required. The builder downloads its base images on first boot.

```bash
tar -xzf meristem-zeroed-20261106-142412.tar.gz
cd meristem-zeroed-20261106-142412
sudo ./install-zeroed.sh
```

The repository listens on http://127.0.0.1:8080 and the frontend on http://127.0.0.1:8100.

The snapshot is the event log. Embeddings are rebuilt locally after startup. The CLI does not connect to a remote database.
