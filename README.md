# Nuki · 抜き

[![Latest release](https://img.shields.io/github/v/release/woolpixels/Nuki-releases?label=release)](https://github.com/woolpixels/Nuki-releases/releases/latest)
![Platform](https://img.shields.io/badge/platform-macOS%20(Apple%20Silicon)-lightgrey)

Nuki 是一个本地运行的电子书章节工具：从一本书里抽出某个角色或关键词相关的章节，或把零散的 EPUB / TXT / PDF 重新整理成一本完整的新书。

所有处理都在本机完成，不上传任何文件。

> 本仓库仅用于发布安装包与说明文档。

## 目录

- [下载与安装](#下载与安装)
- [功能](#功能)
- [导出、封面与目录](#导出封面与目录)
- [桌面版说明](#桌面版说明)
- [隐私](#隐私)
- [常见问题](#常见问题)
- [反馈与联系](#反馈与联系)
- [版本记录](#版本记录)

## 下载与安装

**系统要求**：搭载 Apple 芯片（M1 / M2 / M3 / M4 等）的 Mac。暂不支持 Intel 芯片的 Mac。

1. 前往 [Releases](https://github.com/woolpixels/Nuki-releases/releases/latest)，下载 `Nuki-<版本>-arm64.dmg`。
2. 双击 dmg，把 Nuki 拖到「应用程序」文件夹。
3. 首次打开时若被 macOS 阻止，见下方「首次打开」。

升级时用新的 dmg 再拖一次并选择「替换」即可，原有设置不受影响。

### 首次打开

当前版本尚未使用 Apple Developer ID 签名和公证，首次打开时系统可能提示「无法验证开发者」。这不是病毒，按下列任一方式放行一次即可：

- **方法 A**：在「应用程序」中按住 Control 点按（或右键）Nuki →「打开」→ 再点「打开」。
- **方法 B**（较新的 macOS 上方法 A 无效时）：先双击 Nuki 让它被拦截一次，然后打开「系统设置」→「隐私与安全性」，在页面下方找到 Nuki 的提示，点「仍要打开」并输入电脑密码确认。

## 功能

### 角色抽读

从一本书中按关键词找出相关章节，再按原书顺序重组成新的 EPUB 或 TXT。适合抽取某个角色的剧情线、整理 CP 相关章节、按地点或事件重组内容。

- 导入格式：EPUB、TXT（一次一本）
- 支持多个关键词，实时显示每个关键词的命中次数
- 查看命中章节列表，按原书顺序或命中次数排序，可设置最低命中次数
- 预览关键词所在段落（高亮显示），可手动取消不想保留的章节
- 导出格式：EPUB、TXT

### 整理成书

把一个或多个电子书文件重新识别章节、排序，生成新的完整电子书。只放一个 TXT 文件，也可以直接整理成带封面、目录和分章结构的 EPUB。

- 导入格式：EPUB、TXT、PDF，可混合导入多个文件
- 自动识别章节，自动排序，也可手动拖动调整顺序
- 检查跳号、重复标题与混合来源
- 目录名称可选「简化编号标题」（第1章、第2章……），只改目录，不改正文标题
- 导出格式：EPUB、TXT、PDF

## 导出、封面与目录

**封面**（导出 EPUB 时可选）：使用原书封面 / 自动生成 / 上传自己的图片 / 不使用封面。

**目录**：Nuki 会重新生成目录。

| 导出格式 | 目录形式 |
| --- | --- |
| EPUB | nav / ncx |
| PDF | 书签 |
| TXT | 开头生成目录 |

**PDF 说明**：

- 来源 PDF 若为整页排版，Nuki 会尽量保留原始页面与插图。
- 扫描型 PDF 也可参与整理，导出 EPUB 时按页面图片重新排列，但无法导出为 TXT。

## 桌面版说明

生成新书后，可以直接：

- 导入 Kindle（优先使用 Kusuri；未安装时尝试 Amazon Send to Kindle）
- 用默认阅读器打开
- 打开所在文件夹或另存为

新书默认保存到「下载」文件夹；遇到同名文件会自动添加序号，不会覆盖。

## 隐私

Nuki 不需要账号，也没有服务端。

- 不上传电子书、章节内容或关键词
- 所有解析、重组与导出都在本机完成
- 「最近处理」只在本机记录书名、格式和上次使用的关键词，不保存书籍文件，可逐条删除

## 常见问题

**提示有 DRM / 无法处理？**
带版权保护（DRM）的电子书无法读取，这是正常限制。

**支持 AZW3 / MOBI 吗？**
暂不支持，请先用其他工具转为 EPUB。

**TXT 分章不准或出现乱码？**
在「章节确认」步骤切换编码（常见为 UTF-8 或 GB18030）或修改识别规则。

**安装后图标还是旧的？**
系统图标缓存所致，重新安装或重启电脑即可。

## 反馈与联系

遇到问题、发现错误或有功能建议，可以在 [Issues](https://github.com/woolpixels/Nuki-releases/issues) 留言，或发邮件至 [odyssey.moment@outlook.com](mailto:odyssey.moment@outlook.com)。

反馈时请附上 Nuki 版本号（窗口右上角）、出问题的步骤和截图。

## 版本记录

当前版本：**v1.3.0**。完整更新内容见 [CHANGELOG.md](CHANGELOG.md) 与 [Releases](https://github.com/woolpixels/Nuki-releases/releases)。

---

Nuki · 抜き — Made by Woolpixels · Copyright © 2026 Woolpixels
