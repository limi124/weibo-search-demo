# Weibo Search Demo

一个用于微博关键词搜索结果采集的 Selenium 示例 notebook。

## 内容

- `weibo_search_demo.ipynb`：按关键词搜索微博内容，提取用户名、正文、时间、互动量等字段，并导出为 Excel。

## 环境

建议使用 Python 3.9+。

```bash
pip install pandas selenium webdriver-manager openpyxl
```

## 使用

1. 打开 `weibo_search_demo.ipynb`。
2. 修改 `keywords` 和 `max_pages`。
3. 运行 notebook。
4. 程序会导出 Excel 结果文件。

## 说明

本项目仅用于学习和科研数据采集示例。使用时请遵守网站服务条款、robots 协议及相关法律法规，合理控制访问频率。
