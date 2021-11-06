# BlockIP
收集常见的恶意扫描、采集、攻击等ip。

## 项目说明

建立个人博客的这一年中，遇到过无数次的恶意扫描，恶意采集，甚至还有恶意的攻击。有的CDN支持UA黑白名单，所以屏蔽起来相对省力很多。而有的CDN不支持，或者有人没有使用CDN，想要通过阻断恶意的ip来保障安全，是一个非常漫长且巨大的工程。

事实上已有类似的开源项目，但是有很多都不再更新，或者更新的IP并未通过人工审核，所以决定重新新建一个项目。本项目的目的在于持续不断收集和更新已知的恶意请求ip地址，以便有需要的人可以直接将ip导入到对应配置的地方。

分类说明：

1. attack.txt 收集恶意攻击的IP或网段，前两个IP刷过我1TB流量；
2. saomiao.txt 收集恶意扫描的IP或网段，比如长期请求不同程序的后台或0day地址；
3. caiji.txt 收集恶意采集的IP或网段，比如用Python或Go频繁扫描网站内容的。

## IP来源

已有的IP来自于个人网站的访问日志以及命中CDN阻断规则的记录，所有的IP均是人工识别审核过的。因此早前在CDN的访问控制中填写的黑名单IP不会写入本项目，除非再次发现该IP的恶意请求。

在未来，如果有更多有兴趣的朋友愿意贡献，本项目的IP来源可能就会更广泛。

## PR说明

欢迎各位大佬们分享和完善这个项目。为了避免IP数量过大导致误封现象严重，本项目的所有IP都将会通过人工审核。请在创建PR时附上IP对应的请求日志，以便查证和审核。

当然，本项目收集的`ip.txt`不一定能直接适用于所有的控制台导入规则，所以建议PR时候保证每行一个IP或网段，以回车隔断。

