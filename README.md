# Weibo Search Demo

一个通用的微博关键词搜索结果采集示例 notebook。适合按“城市 + 主题词”的方式采集微博搜索结果，例如城市绿地游憩、旅游感知、公共空间评价、灾害事件舆情等主题。

## 内容

- `weibo_search_demo.ipynb`：按关键词搜索微博内容，提取用户名、正文、时间、互动量和链接等字段，并导出为 Excel。

## 环境

建议使用 Python 3.9+。

```bash
pip install pandas selenium webdriver-manager openpyxl
```

## 使用

1. 打开 `weibo_search_demo.ipynb`。
2. 修改配置区：
   - `city`：城市名，例如 `西安`、`南昌`、`九江`
   - `project_name`：研究主题名，例如 `绿地游憩`、`旅游感知`
   - `topic_words`：主题词列表，会自动和城市名组合
   - `extra_keywords`：额外完整搜索词
   - `max_pages`：每个关键词翻页数
3. 运行 notebook。
4. 程序会导出 Excel 结果文件到 `outputs/` 文件夹。

示例：

```python
city = "南昌"
project_name = "绿地游憩"
topic_words = ["公园", "湿地", "绿道", "森林公园", "郊游"]
extra_keywords = ["南昌 赣江 夜游"]
max_pages = 5
```

导出文件示例：

```text
outputs/微博_南昌_绿地游憩_搜索结果.xlsx
```

## 说明

本项目仅用于学习和科研数据采集示例。使用时请遵守网站服务条款、robots 协议及相关法律法规，合理控制访问频率。
