>Fork至hoxu/gitstats

## 更改 2024.12.3
1. 适配Windows下命令行,替换 'wc -l'、'grep -v ^commit'
2. 提交者名字 支持中文
3. 修正 多目录时只保留了最后一个目录信息changes_by_date_by_author stamp -> author -> {lines_added:0,commits:0}
4. 修正 changes_by_date_by_author[stamp][author]['lines_added'] 算法累加错误
5. 新增 按作者统计阶段+lines的详情

## 更改
修改并适配了Python3
1. 修改print -> print()
2. 修改map() -> list(map())
3. 修改 Pipline output -> output.decode()
4. 添加了部分中文注释

## 使用方式
1. 安装gnuplot，用以生成交互式图表， 
    Mac OS可以使用`brew install gnuplot`安装
    Windows可以从 https://sourceforge.net/projects/gnuplot/ 下载安装
2. 进入项目目录，使用以下命令运行。
```
python3 gitstats  Git项目目录  报告目录
```
3. 使用浏览器打开 报告目录/index.html

## 报告示例
![](https://tva1.sinaimg.cn/large/006y8mN6ly1g82ni5c6tnj30s80h176c.jpg)

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g82nh49rorj30s70llq4i.jpg)

