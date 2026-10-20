# Loki + Promtail Log Starter (Lite)

## English

A Promtail scrape for `/var/log/nginx/access.log` and the example lines it matches. The push URL is `http://127.0.0.1:3100/loki/api/v1/push`, which is the path Promtail examples have used. Check upstream docs before you send that to a live process.

Not in this subset: the compose file, the Loki config, the syslog listener, the Grafana profile, and the env marker tags.

### Deliverables

- `deliverables/promtail-nginx.yaml` — nginx combined-log scrape
- `examples/nginx-access.log` — RFC 5737 combined-format lines
- `examples/logql-nginx.txt` — selectors for `job="nginx-access"` and `host="example.com"`

## 中文

一份只抓 `/var/log/nginx/access.log` 的 Promtail 配置，以及它对得上的示例行。推送地址是 `http://127.0.0.1:3100/loki/api/v1/push`，这是 Promtail 示例里用过的路径。发给正在跑的进程之前，请核对官方文档（check upstream docs）。

精简版不含：compose 文件、Loki 配置、syslog 监听、Grafana profile，以及镜像记号标签。

### 交付文件

- `deliverables/promtail-nginx.yaml`
- `examples/nginx-access.log`
- `examples/logql-nginx.txt`

Full version: GUMROAD_URL
