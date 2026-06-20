** 本文档的60%由AI生成 **
# 仓库说明

这是一个自用翻译文件仓库，包含多个程序的个性化中文本地化资源。

## 使用说明

当前目录下执行
```sh

sudo cp file.mo /usr/share/locale/zh_CN/LC_MESSAGES/

```

## 编辑说明

1. 生成 `.po` 文件
   - 使用命令：
     ```sh
        msgunfmt ./source.mo -o ./target.po
     ```
   - 如果 `msgfmt` 未安装，可通过系统包管理器安装 `gettext`。

2. 编辑翻译
   - 修改 `.po` 文件中的翻译条目。
   - 可以使用 `poedit`、`vim`、`emacs` 等工具进行编辑。

3. 生成 `.mo` 文件
   - 使用命令：
     ```sh
        msgfmt ./source.po -o ./target.mo
     ```

4. 使用翻译
   - `sudo cp file.mo /usr/share/locale/zh_CN/LC_MESSAGES/`
