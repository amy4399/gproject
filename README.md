# 南方科技大学本科毕业论文LaTeX模板（WebLaTeX版）

本模板专为 WebLaTeX / Overleaf 等在线 LaTeX 编辑器设计，无需额外的 `.cls` 文类文件。

## 三个版本选择

| 版本 | 文件名 | 说明 | 推荐场景 |
|------|--------|------|---------|
| **标准版** | `main-standard.tex` | 严格按照原模板，带字体 fallback | ⭐ 推荐使用 |
| 兼容版 | `main.tex` | 指定 SimSun / SimHei 字体 | 字体环境确认的情况 |
| 简化版 | `main-simple.tex` | 使用 ctex 默认字体 | 兼容性优先 |

## 使用方法（标准版）

1. 将 `main-standard.tex` 改名为 `main.tex`
2. 将 `references.bib` 和整个 `fonts/` 文件夹一起上传
3. 编译器选择 **XeLaTeX**，BibTeX 选择 **Biber**
4. 在 `main.tex` 顶部的论文信息填写区填入你的信息
5. 开始写作你的论文

## 文件结构（标准版）

```
├── main.tex           # 主文件（从 main-standard.tex 重命名）
├── references.bib     # 参考文献文件
├── fonts/
│   ├── simhei.ttf     # 黑体
│   ├── simsun.ttc     # 宋体
│   ├── simsunb.ttf    # 宋体备用
│   └── times/
│       ├── times.ttf      # Times New Roman
│       ├── timesbd.ttf    # Times New Roman Bold
│       ├── timesbi.ttf    # Times New Roman Bold Italic
│       └── timesi.ttf     # Times New Roman Italic
└── README.md          # 本说明文件
```

## 主要功能

- 中文封面 + 英文封面
- 诚信承诺书
- 中文摘要 + 英文摘要
- 目录
- 正文（带章节格式）
- 参考文献（GB7714-2015格式）
- 附录
- 致谢

## 编译命令

```bash
xelatex main.tex
biber main
xelatex main.tex
xelatex main.tex
```

## 注意事项

- 务必使用 XeLaTeX 编译器
- 参考文献使用 Biber 处理
- 学校可能会更新格式要求，请以最新官方要求为准
