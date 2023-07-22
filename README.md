# 简介

本项目每周五自动生成 GeoIP 文件，同时提供命令行界面（CLI）供用户自行定制 GeoIP 文件，包括但不限于 V2Ray dat 格式路由规则文件 `geoip.dat` 和 MaxMind mmdb 格式文件 `Country.mmdb`。

This project releases GeoIP files automatically every Friday. It also provides a command line interface(CLI) for users to customize their own GeoIP files, included but not limited to V2Ray dat format file `geoip.dat` and MaxMind mmdb format file `Country.mmdb`.

## 与官方版 GeoIP 的区别

- 中国大陆 IPv4 地址数据融合了 [IPIP.net](https://github.com/17mon/china_ip_list/blob/master/china_ip_list.txt) 和 [@gaoyifan/china-operator-ip](https://github.com/gaoyifan/china-operator-ip/blob/ip-lists/china.txt)
- 中国大陆 IPv6 地址数据融合了 MaxMind GeoLite2 和 [@gaoyifan/china-operator-ip](https://github.com/gaoyifan/china-operator-ip/blob/ip-lists/china6.txt)
- 新增类别（方便有特殊需求的用户使用）：
  - `geoip:cloudflare`（`GEOIP,CLOUDFLARE`）
  - `geoip:cloudfront`（`GEOIP,CLOUDFRONT`）
  - `geoip:facebook`（`GEOIP,FACEBOOK`）
  - `geoip:fastly`（`GEOIP,FASTLY`）
  - `geoip:google`（`GEOIP,GOOGLE`）
  - `geoip:netflix`（`GEOIP,NETFLIX`）
  - `geoip:telegram`（`GEOIP,TELEGRAM`）
  - `geoip:twitter`（`GEOIP,TWITTER`）

## 下载地址

> 如果无法访问域名 `raw.githubusercontent.com`，可以使用第二个地址 `cdn.jsdelivr.net`。
> *.sha256sum 为校验文件。

### V2Ray dat 格式路由规则文件

> 适用于 V2Ray、Xray-core 和 Trojan-Go。

- **geoip.dat**：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/geoip.dat](https://raw.githubusercontent.com/yaling888/geoip/release/geoip.dat)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip.dat](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip.dat)
- **geoip.dat.sha256sum**：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/geoip.dat.sha256sum](https://raw.githubusercontent.com/yaling888/geoip/release/geoip.dat.sha256sum)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip.dat.sha256sum](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip.dat.sha256sum)
- **geoip-only-cn-private.dat**（精简版 GeoIP，只包含 `geoip:cn` 和 `geoip:private`）：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/geoip-only-cn-private.dat](https://raw.githubusercontent.com/yaling888/geoip/release/geoip-only-cn-private.dat)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip-only-cn-private.dat](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip-only-cn-private.dat)
- **geoip-only-cn-private.dat.sha256sum**：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/geoip-only-cn-private.dat.sha256sum](https://raw.githubusercontent.com/yaling888/geoip/release/geoip-only-cn-private.dat.sha256sum)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip-only-cn-private.dat.sha256sum](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip-only-cn-private.dat.sha256sum)
- **geoip-asn.dat**（精简版 GeoIP，只包含上述新增类别）：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/geoip-asn.dat](https://raw.githubusercontent.com/yaling888/geoip/release/geoip-asn.dat)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip-asn.dat](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip-asn.dat)
- **geoip-asn.dat.sha256sum**：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/geoip-asn.dat.sha256sum](https://raw.githubusercontent.com/yaling888/geoip/release/geoip-asn.dat.sha256sum)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip-asn.dat.sha256sum](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/geoip-asn.dat.sha256sum)
- **cn.dat**（精简版 GeoIP，只包含 `geoip:cn`）：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/cn.dat](https://raw.githubusercontent.com/yaling888/geoip/release/cn.dat)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/cn.dat](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/cn.dat)
- **cn.dat.sha256sum**：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/cn.dat.sha256sum](https://raw.githubusercontent.com/yaling888/geoip/release/cn.dat.sha256sum)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/cn.dat.sha256sum](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/cn.dat.sha256sum)
- **private.dat**（精简版 GeoIP，只包含 `geoip:private`）：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/private.dat](https://raw.githubusercontent.com/yaling888/geoip/release/private.dat)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/private.dat](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/private.dat)
- **private.dat.sha256sum**：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/private.dat.sha256sum](https://raw.githubusercontent.com/yaling888/geoip/release/private.dat.sha256sum)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/private.dat.sha256sum](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/private.dat.sha256sum)

### MaxMind mmdb 格式文件

> 适用于 [Clash](https://github.com/yaling888/clash) 和 Leaf。

- **Country.mmdb**：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/Country.mmdb](https://raw.githubusercontent.com/yaling888/geoip/release/Country.mmdb)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country.mmdb](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country.mmdb)
- **Country.mmdb.sha256sum**：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/Country.mmdb.sha256sum](https://raw.githubusercontent.com/yaling888/geoip/release/Country.mmdb.sha256sum)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country.mmdb.sha256sum](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country.mmdb.sha256sum)
- **Country-only-cn-private.mmdb**（精简版 GeoIP，只包含 `GEOIP,CN` 和 `GEOIP,PRIVATE`）：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/Country-only-cn-private.mmdb](https://raw.githubusercontent.com/yaling888/geoip/release/Country-only-cn-private.mmdb)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country-only-cn-private.mmdb](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country-only-cn-private.mmdb)
- **Country-only-cn-private.mmdb.sha256sum**：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/Country-only-cn-private.mmdb.sha256sum](https://raw.githubusercontent.com/yaling888/geoip/release/Country-only-cn-private.mmdb.sha256sum)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country-only-cn-private.mmdb.sha256sum](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country-only-cn-private.mmdb.sha256sum)
- **Country-asn.mmdb**（精简版 GeoIP，只包含上述新增类别）：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/Country-asn.mmdb](https://raw.githubusercontent.com/yaling888/geoip/release/Country-asn.mmdb)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country-asn.mmdb](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country-asn.mmdb)
- **Country-asn.mmdb.sha256sum**：
  - [https://raw.githubusercontent.com/yaling888/geoip/release/Country-asn.mmdb.sha256sum](https://raw.githubusercontent.com/yaling888/geoip/release/Country-asn.mmdb.sha256sum)
  - [https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country-asn.mmdb.sha256sum](https://cdn.jsdelivr.net/gh/yaling888/geoip@release/Country-asn.mmdb.sha256sum)

## License

[CC-BY-SA-4.0](https://creativecommons.org/licenses/by-sa/4.0/)

This product includes GeoLite2 data created by MaxMind, available from [MaxMind](http://www.maxmind.com).
