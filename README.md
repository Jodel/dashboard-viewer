# The Jodel Dashboard Viewer
This [resin.io](https://resin.io/) based application runs on a raspberry pi to
display our [grafana](http://grafana.org/) dashboards (powered by
http://prometheus.io/).

![dashboard-at-jodel](dashboard.jpg)

## Use it
Add your resin git remote and push the project. For details see
[resin.io's getting started documentation](http://docs.resin.io/#/pages/installing/gettingStarted.md).

Just clone this repo instead of the example.
After that, you need to set some [environment variables](http://docs.resin.io/#/pages/management/env-vars.md):

- `URL`: Dashboard URL to open
- `PASS`: The dashboard runs dropbear, this var will be the root password. If unset, defaults to 'root'
