# DomainSpider

此项目包含两种获取WHOIS信息的方法。

其一为通过`python-whois` 模块直连whois服务器43端口，其二为静态爬虫重复爬取。

### var_HTTP

##### 使用方法：

安装相应模块，配置`./send_var_SMTP.py` 中的SMTP服务，运行`./main.py` 。新队列输入`1` ,更新提醒列表输入`2`。

进一步可以把`alram.sh` 放入crontab.daily，配置工程位置实现每日检查。

> 附有一份流程简图观察文件流向

##### 备注：

* `words.txt ` 来源与`google-10000-english-no-swear` 中筛选出的三位高频短单词


* 此方法采用单进程
* 目前仅提供一所网站的解析，已知 ` .gs ` 还有两个备选项。

