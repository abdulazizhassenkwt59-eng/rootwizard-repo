# RootWizard (`rsu-bridge`)

Rootless Termux command runner, modular addon system, and encrypted command log bridge.

## Install from Local APT Repo

```bash
REPO_DIR="$HOME/rootwizard-repo/apt-repo"
LIST_FILE="${PREFIX:-/data/data/com.termux/files/usr}/etc/apt/sources.list.d/rootwizard.list"

mkdir -p "$(dirname "$LIST_FILE")"
echo "deb [trusted=yes] file://$REPO_DIR ./" > "$LIST_FILE"
apt update
apt install -y --allow-unauthenticated rootwizard
```

