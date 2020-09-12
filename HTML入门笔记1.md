# Html入门笔记

## Html起源
李爵士发明www。1990发明了html、url和http。用自己发明的网址访问了自己搭建的服务器。本质是希望内容共享。

## Html的head
### 需要声明：
* 文档类型：!DOCTYPE html
* 语言：lang='zh-CN'
* meta：一些默认字段，以及对字符编码（charset='UTF-8'）的设置
* 标题：title  

## Html的body
### 章节标签：
* h1~h6：标题
* section：章节，区分不同大块内容
* article：文章，定义来自于外部的内容
* main：主要部分
* aside：次级部分
* header和footer：开头和结尾

### 全局属性：
class、id、contenteditable（用户可以编辑）、hidden、style、tabindex（tab键的交互顺序）、title（与溢出隐藏配合使用，展示完整内容）

### 内容标签：
* ul或ol+li、dl+dt+dd：不同样式和用途的列表
* a：链接，跳转其他url
* strong：内容强调，默认字体加粗
* em：语气强调，默认斜体
* code：放代码，类似vscode代码样式
* pre：保留程序员写的多个空白
* hr：分隔线
* quote和blockquote：引用
