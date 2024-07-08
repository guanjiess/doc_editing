##1. 需求

1. 将微服务介绍重命名为 `README.md`，并且移动到上级目录。
2. 微服务介绍中的受众和目的移动到架构设计的顶部
3. 架构设计中的技术债务挪动到`README.md`中，作为第四章
4. 启动指导、历史问答作为第五、六章。



## 2. 需求分析

1. 需要对markdown文件的内容进行搬移、调整。标题
   - 正文段落
   - 网页、本地文件的超链接，注意搬移后的文件地址会发生变化
   - 表格
   - 需要调整文档的格式
2. 用Python实现

##3. 实现方法

1. 读取待操作的markdown文件，将其转为 html
2. 用beautiful soup提取指定标题的内容
3. 将所提取的内容按照 markdown 添加到目标文件中
   - 标题 
   - 外部链接
4. 工具
   - python文件操作： os  shutil
   - https://daringfireball.net/projects/markdown/syntax
   - [python-markdown](https://python-markdown.github.io/)
   - [beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)