# flexhub-monitoring-setup

Default user name and password for Grafana is admin/foobar.

In order to run an example monitoring setup with a local flexhub node just run this sequence of docker-compose commands:

```bash
docker-compose -p monitoring up -d
docker-compose -p exporters -f exporters.yml up -d
```

The dashboards can then be found at http://localhost:3000/dashboards

## Node Eth - Ethereum-based metrics

|||
|-----|-----|
| Blocks per Minute | number of blocks per 1 minute |
| Net Peers	| number of peers currently connected to the client |
| Block Number | block number at a certain point in time |
| Latest Block Transactions | number of transactions in a latest block |
| Pending Block Transactions | number of transactions in a pending block |

## Node Server - Server metrics

Various server metrics (CPU, RAM, disk space, etc.)