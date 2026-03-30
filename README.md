<<<<<<< HEAD
# 论文 Word 格式化脚本（format_paper）

## 功能说明

根据你在 Ask 阶段确认的最终细则（A4/边距/1.5倍行距/标题大纲级别/章强制起页/引言起算页码/TOC 样式/图表题注连续编号/参考文献样式等）对输入 `.docx` 进行版式重排，并输出新的 `*_formatted.docx`。

关键点：
- 目录（TOC）是 Word 字段：脚本会修改 `styles.xml` 中 `TOC1/TOC2/TOC3` 样式；你打开输出文件后建议手动“更新目录”一次。
- 引言位于新 section：脚本会修改 OOXML，把引言 section 的页码 start 设置为 `1`。

## 环境要求

- Python 3.7+（你的环境通常是 3.7，因此脚本固定依赖 `python-docx==0.8.11`）
- 依赖见 `requirements.txt`

## 安装

```bash
cd format_paper
pip install -r requirements.txt
```

## 使用

```bash
python format_paper.py input.docx
```

默认输出：`input_formatted.docx`

指定输出：

```bash
python format_paper.py input.docx -o output.docx
```

## 需要人工复核的点

- 图/表题注的文本格式如果偏离常见 `图1 ...` / `表1 ...`，可能无法被识别。
- 脚注“每页重新编号”的逻辑强依赖模板设置；脚本尽力做版式统一，但建议你抽查一两页。
=======
# -
本工具基于 Python 开发，能够根据《华东政法大学硕士学位论文格式模板》自动格式化 Word 文档。只需在命令行中运行脚本，即可快速将毕业论文、学位论文等学术文档调整为统一、规范的排版样式，大幅节省手动调整格式的时间。  ✨ 主要功能 页面设置 正文样式 标题层级识别 脚注处理 图表与公式 参考文献格式化 长引文处理   
>>>>>>> b8782a9eae3f45c811ee5cb61dbdcb5b7bf113b6
