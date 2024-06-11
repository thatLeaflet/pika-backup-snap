## WIP, not working yet (issue with installing Borgbackup in the snap)

Note: This is an unofficial repackaging and is not endorsed by the upstream project. The upstream Pika Backup project can be found [here](https://gitlab.gnome.org/World/pika-backup).

## Want to build the snap yourself?

Before you begin
- Ensure you have snapd installed
- Ensure you have git installed

How to set up snapcraft
- Install snapcraft: run `sudo snap install snapcraft --classic`
- Install lxd: run `sudo snap install lxd`
- Add your user to the lxd group: run `sudo usermod -aG lxd $USER`
- Reboot your computer
- Configure lxd: run `lxd init --minimal`

How to build the snap
- Enter a nice working directory (e.g. ~/projects)
- Download repo: run `git clone https://github.com/thatLeaflet/pika-backup-snap.git && cd ./pika-backup-snap`
- Build the snap: run `SNAPCRAFT_ENABLE_EXPERIMENTAL_EXTENSIONS=1 snapcraft`
- Install the snap: run `sudo snap install --dangerous ./pika-backup_*.snap`
