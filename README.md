﻿# CrawlNews
实时抓取教务处公告信息，并推送到指定邮箱
*******
## 技术细节
* 使用urllib2抓取网页内容
* 使用smtplib和email模块发送邮件
* 实现Daemon进程，可部署到linux系统上，平均每3个小时抓取一次
* 把运行出错信息记录到"erro_log"文件中
* 把每次推送的公告信息的最大日期记录到"last_update_time"文件中，避免信息被重复推送
* 对易出错的地方进行异常捕获
