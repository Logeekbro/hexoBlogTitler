# hexoBlogTitler
可能有人和我一样，想把以前做的笔记发布在hexo上，但hexo只能解析在文件头部指定的特定格式的标题，如果有大量笔记需要上传，一一添加不太现实。
此脚本可以便捷的为你所有没标题的md文件添加文件名为标题，且**已有标题**的文件不会重复添加。
>  **已有标题的判定标准：文件内容以 --- 开头**   
>  **只提供了两种常见OS及架构的可执行程序，需要其它版本的请自行从源文件构建(go build .)**

#### 使用方法(以Windows10为例): 
1. 将原笔记移到hexo的_posts文件夹下
2. 从releases中下载对应的.exe文件
3. 运行程序(.exe)，将_posts文件夹的绝对路径粘贴到窗口中，然后回车即可。  

#### 多类型文件支持
  此脚本只内置了md文件的标题添加规则(mdtitler.go)，可以通过实现ititler接口来自定义其它文件的标题添加规则(参考mdtitler.go)，   
  同时将main函数中的添加规则改为自定义的即可。
#### 可能说得不太清楚，有问题请提交issue😊
