# 基于 goreplay 日志清洗组合和可视化方案

goreplay 要想把数据传到到 es 里面，需要回放的时候才能使用对应的 es 插件，这个插件【[shaonian/goreplay](https://github.com/ShaoNianyr/goreplay)】我也曾经做过升级，兼容 es6.x 以上的版本。但是很多时候我们希望，不需要回放也能传到 es 里面去，且能够对 goreplay 的日志进行清洗和挖掘，所以这里用传统 elk 的方式，对 goreplay 的日志进行清洗组合，并结合 grafana 来做可视化的数据大屏。

欢迎来 star ~

技术交流 QQ 群: 552643038

## 技术方案
* goreplay
* elasticsearch
* filebeat
* logstash
* grafana

## 快速体验

```
docker-compose up -d
```

## grafana dashboard

```
https://grafana.com/grafana/dashboards/11924
```

## 效果

<img src="https://github.com/ShaoNianyr/goreplay-grafana/blob/master/dashboard.png">

## 注意事项

代码里面提供了 es-cluster 集群的部署方式，实际 demo 使用的是 es 单节点部署。
