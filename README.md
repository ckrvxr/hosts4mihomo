# hosts4mihomo

This project retrieves the hosts file from the source at 6 AM in Beijing every day to create the binary rule file for mihomo (mrs).

### Example:

Typically, only one needs to be selected. StevenBlack is used here.

```yaml
rule-providers:
  stevenblack:
  type: http
  behavior: domain
  format: mrs
  interval: 43200
  url: "https://testingcf.jsdelivr.net/gh/ckrvxr/hosts4mihomo@main/StevenBlack.mrs"

```

```yaml
rules:
  - 'RULE-SET,stevenblack,REJECT'
```

### CDN Links:

(testingcf.jsdelivr.net) (目前中国大陆地区可直连)

* StevenBlack:  https://testingcf.jsdelivr.net/gh/ckrvxr/hosts4mihomo@main/StevenBlack.mrs
* hBlock :  https://testingcf.jsdelivr.net/gh/ckrvxr/hosts4mihomo@main/hBlock.mrs
