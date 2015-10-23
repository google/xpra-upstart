This is not an official Google product.

# Upstart Xpra config
Missing upstart config for Xpra (screen for X). Should work on Ubuntu 14.04.

# Usage

```shell
sed --in-place "s|\\\$USER|$USER|g" xpra.conf
sed --in-place "s|\\\$HOME|$HOME|g" xpra.conf
sudo cp xpra.conf /etc/init/
sudo initctl reload-configuration
sudo service xpra start
```

Starts a service for Xpra for `DISPLAY=:100`.
