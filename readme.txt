Belchertown 3.0.0 skin for WeeWX
Copyright 2018 Pat O'Brien

The maintained installation and configuration guide is README.md in this
repository. It covers stock WeeWX 5, report paths, MQTT and forecasts.

Install the fixed archive:

weectl extension install https://github.com/weewx-packages/catalog/releases/download/belchertown/v3.0.0/belchertown-3.0.0.tar.gz

Use the WeeWX environment and add --config /path/to/weewx.conf if needed.
Restart WeeWX after reviewing [StdReport][[Belchertown]]. Wait for the next
archive interval or run weectl report run Belchertown. The installer uses
skins/Belchertown, user.belchertown and HTML_ROOT = belchertown by default;
WeeWX prefixes the relative report path with the station's configured web
output root. Check the merged directory in weewx.conf.

Upgrade using the fixed archive after backing up the skin and configuration.
Remove with weectl extension uninstall Belchertown and restart WeeWX.
Forecasts use the configured provider; the former DarkSky instructions no
longer describe this release. See README.md for the supported providers.

Original credits are retained in README.md, including Gary Roderick's chart
work, Brian's weather icons and the upstream contributors. See LICENSE for GPLv3.
