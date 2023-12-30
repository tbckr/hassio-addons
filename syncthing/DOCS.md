# Configuration

Configuration is done via [Syncthing's web UI](/hassio/ingress/a4f388b4_syncthing) (embedded into Home Assistant).
First start the add-on from the [_Info_ tab](/hassio/addon/a4f388b4_syncthing/info) and then click `OPEN WEB UI`.

## Available directories

When using this add-on to permanently hold your data, put the synced folders inside one of the following directories:

- `/media`
- `/share`
- `/backup`
- `/ssl`
- `/addons`

Only the above directories are mapped into the add-on container. If you put synced folders in any other directory
 (like `/root` or `/mnt`), the synced data will be deleted on container restart.

Syncing the `/backup` directory (preferably in
[send only mode](https://docs.syncthing.net/users/foldertypes.html#send-only-folder)) is a
simple way to automatically backup the Home Assistant backups to any of your other Syncthing devices.
