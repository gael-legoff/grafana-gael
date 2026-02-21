# [grafana-gael](https://snapcraft.io/grafana-gael)

_This is NOT an original piece of work, just a snap of Grafana_

The open-source platform for monitoring and observability
Grafana allows you to query, visualize, alert on and understand your metrics no matter where they are stored. Create, explore, and share dashboards with your team and foster a data-driven culture

For more information see: https://grafana.com/grafana/

**Configure the server**

Read the doc at https://grafana.com/docs/grafana/latest/ on how to get started.

```
sudo mkdir -p /var/snap/grafana-gael/common/data/plugins
sudo mkdir -p /var/snap/grafana-gael/common/conf/provisioning/datasources
sudo mkdir -p /var/snap/grafana-gael/common/conf/provisioning/plugins
sudo mkdir -p /var/snap/grafana-gael/common/conf/provisioning/dashboards
sudo mkdir -p /var/snap/grafana-gael/common/conf/provisioning/notifiers
sudo mkdir -p /var/snap/grafana-gael/common/conf/provisioning/alerting

sudo vi /var/snap/grafana-gael/current/grafana.ini
```

```
#################################### Paths ###############################
[paths]
# Path to where grafana can store temp files, sessions, and the sqlite3 db (if that is used)
data = /var/snap/grafana-gael/common/data

# Temporary files in `data` directory older than given duration will be removed
temp_data_lifetime = 24h

# Directory where grafana can store logs
logs = /var/snap/grafana-gael/common/data/log

# Directory where grafana will automatically scan and look for plugins
plugins = /var/snap/grafana-gael/common/data/plugins

# folder that contains provisioning config files that grafana will apply on startup and while running.
provisioning = /var/snap/grafana-gael/common/conf/provisioning

# Unix socket path
socket = /var/snap/grafana-gael/current/grafana.sock
```

`sudo snap restart grafana-gael.grafana-server`

To use Grafana visit http://localhost:3000/

**2026-02-21**
* v12.3.3 available on amd64

**2026-02-11**
* v12.3.2+security-01 available on amd64

**2026-02-03**
* v12.3.2 available on amd64

**2025-12-21**
* v12.3.1 available on amd64

**2025-11-19**
* v12.3.0 available on amd64

**2025-11-19**
* v12.2.2 available on amd64

**2025-11-16**
* v12.2.1 available on amd64

**2025-09-24**
* v12.2.0 available on amd64

**2025-08-31**
* v12.1.1 available on amd64

**2025-07-24**
* v12.1.0 available on amd64

**2025-07-18**
* v12.0.2+security-01 available on amd64

**2025-06-22**
* v12.0.2 available on amd64

**2025-06-17**
* v12.0.1+security-01 available on amd64

**2025-05-24**
* v12.0.1 available on amd64

**2025-05-06**
* v12.0.0 available on amd64

**2025-04-27**
* v11.6.1 available on amd64

**2025-03-26**
* v11.6.0 available on amd64

**2025-02-20**
* v11.5.2 available on amd64

**2025-02-03**
* v11.5.1 available on amd64

**2025-01-28**
* v11.4.1 available on amd64

**2024-12-06**
* v11.4.0 available on amd64

**2024-11-13**
* v11.3.0+security-01 available on amd64
* Fixes CVE-2024-9476

**2024-10-23**
* v11.3.0 available on amd64

**2024-10-18**
* v11.2.2+security-01 available on amd64
* Fixes CVE-2024-9264

**2024-10-12**
* v11.2.2 available on amd64

**2024-06-26**
* v11.1.0 available on amd64

**2024-05-14**
* v11.0.0 available on amd64

**2024-04-06**
* v10.4.1 available on amd64

