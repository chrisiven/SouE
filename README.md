# SouE项目
作者：chrisiven@163.com or 342083472@qq.com or chrisiven
开发周期:10天
项目简介:
    一个种子搜索网站
 
项目数:2
    1.BtSpider:抓取数据的爬虫
    2.Django项目:展示数据
 
BtSpider项目:
  架构:
      开发语言:python3.7
      开发框架:自行开发框架
      核心库:requests,asyncio,aiohttp,pymysql,redis,threading
  作用:
      用于抓取特定网站数据从而解析存储到数据库

Django项目:
  架构:
      开发语言:python3.7
      开发框架:django2.2
      数据库:mysql,redis
  作用:
      用于展示爬虫抓取的数据,从而生成种子链接展示给用户


执行思路(简)：BtSpider和Django项目通过redis进行互动,django传入数据到redis,BtSpider使用redis进行监听django传入的数据并且传输到爬虫上到对应网站下载.
