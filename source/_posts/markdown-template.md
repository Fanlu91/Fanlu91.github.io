---
title: Markdown 模板
date: 2018-12-19 17:01:12
tags: 
- markdown
- template
- cheatsheet
---

常用markdown语法参考及有用的链接。
在线富文本转markdown http://markitdown.medusis.com/ 
html转markdown http://domchristie.github.io/turndown/ 

通常参考学习github上的readme文件即可。

---
# 分隔符
```
---
# 分隔符 
```

# 标题
```
# 标题
### 这是标题3
#### 这是标题4
```

### 这是标题3
#### 这是标题4
> 要注意\#后面需要跟空格，否则有可能无法渲染，比如目前博客用的hexo。


# 转译字符
```
使用 \ , 比如 \# \>
```
使用 \ , 比如 \# \>

> Hexo 的markdown解析比较不尽如人意，发现部分转译无法实现。

# 链接
```
[fanlucloud.com](http://www.fanlucloud.com)
```
[fanlucloud.com](http://www.fanlucloud.com)

# 引用
在文字前 添加 \>
```
 > 比如这个
```
 > 比如这个

# 有序列表
```
1. 有序列表 在行首增加数字和英文句点, 不要求数字一定要连续
2. 有序列表
3. 有序列表
```
1. 有序列表 在行首增加数字和英文句点, 不要求数字一定要连续
1. 有序列表
4. 有序列表

# 无序表
```
* 无序列表 在行首增加 * 或 -
- 无序列表 在行首增加 * 或 -
```
* 无序列表 在行首增加 * 或 -
- 无序列表 在行首增加 * 或 -

# 字样式
```
**粗体**
*斜体*
~~删除线~~
```
**粗体**
*斜体*
~~删除线~~


# 表格
```
| 凡路|内容 | 版本 |
|---|---|---|
| fanlucloud | Markdown| Latest |
```

| 凡路|内容 | 版本 |
|---|---|---|
| fanlucloud | Markdown| Latest |

# 代码
在代码前后增加 三个反单引号

```
int i = 0; i = 1;
for (int i = 0; i < 100; i++)
{
      printf("hello from fanlu!\n");
}
```