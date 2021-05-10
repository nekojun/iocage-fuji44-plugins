# iocage-fuji44-plugins

This is the index repository for iocage-plugin maintained by fuji44.

- [Official iXsystems iocage plugins](https://github.com/freenas/iocage-ix-plugins)
- [Official community plugins](https://github.com/ix-plugin-hub/iocage-plugin-index)

## Usage

Use the `-g` option of the `iocage fetch` command to specify the URL of this repository. And for the `-P` option, specify the name of the plugin you want to install.

```
sudo iocage fetch -P flexget -n flexget -g https://github.com/fuji44/iocage-fuji44-plugins.git ip4_addr="em0|192.168.0.100/24"
```

We used to specify `--branch main`, but we found out that `iocage update` does not allow the same specification, which causes problems.
Therefore, for the time being, the main branch for iocage-related repositories will be `master`.
We'll change it back to `main` when the iocage command is able to deal with this problem.

## Plugins

- [flexget](https://github.com/fuji44/iocage-plugin-flexget)
- [mirakurun](https://github.com/fuji44/iocage-plugin-mirakurun)
- [scrapyd](https://github.com/fuji44/iocage-plugin-scrapyd)
