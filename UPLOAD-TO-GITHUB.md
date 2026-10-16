# 上传到 Gobi-GBA / Gobi-Investment-Skills

本次只交付文件，没有替你推送或修改 GitHub。截图显示目标仓库为公开仓库；本包按公开展示整理。

## 网页上传成果包

1. 双击解压 `research-studio-v30-github.zip`，得到 `research-studio-v30` 文件夹。不要只把 ZIP 本身上传，否则同事不能直接浏览文件。
2. 打开 GitHub 中 `Gobi-GBA / Gobi-Investment-Skills`，进入 **Code** 页。
3. 点击右上方 **Add file → Upload files**。
4. 从 Finder 把整个 `research-studio-v30` 文件夹拖入上传区域。检查文件路径以 `research-studio-v30/` 开头，这样保留原仓库的 README 和已有 Skills。
5. 在提交说明填写 `Add Research Studio v30 skills, manual and research examples`。选择 **Create a new branch for this commit and start a pull request**，分支名可填 `research-studio-v30`（如已存在，使用新的名字）。点击 **Propose changes**。
6. 在下一页点击 **Create pull request**。检查 **Files changed**，本次应只有新增目录；如果出现意外删除或覆盖，先不要合并。
7. 检查完成后点击 **Merge pull request → Confirm merge**。如仓库要求其他管理员审批，按页面提示完成。合并后同事可在默认分支打开本目录与 README。

不同仓库权限和规则可能导致按钮文案不同；有的上传页显示 **Commit changes**。如果没有新分支选项，可先在 Code 页的分支下拉中创建分支，再上传。无需创建新的仓库。

GitHub 网页单文件上限 25 MiB，一次最多 100 个文件；这个成果包按此范围整理。步骤依据 [GitHub 官方上传说明](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)。

## 让仓库首页也能找到成果

合并后，打开原仓库根目录的 README，点铅笔编辑，在末尾加一行入口即可；保留原有介绍：

```markdown
- [Research Studio：四个投研 Skill、使用手册与研究样例](research-studio-v30/README.md)
```

本包的 README 放在子目录内会自动显示为该目录的介绍页。不要直接用它覆盖原仓库 README，否则相对链接和原有说明可能被破坏。

## 如果还要保存完整源码

`research-studio-source-v30.zip` 是另一份脱敏代码快照，文件数超过单次网页上传限制，建议用 GitHub Desktop：

1. 在 GitHub Desktop 中 **File → Clone repository**，选择已有仓库，克隆到一个新的本地目录；见 [GitHub Desktop 官方克隆说明](https://docs.github.com/en/desktop/adding-and-cloning-repositories/cloning-and-forking-repositories-from-github-desktop)。
2. 在 **Current Branch → New Branch** 创建一个新分支，例如 `research-studio-source-v30`。
3. 解压源码 ZIP，把整个 `research-studio-source-v30` 文件夹放进刚克隆的仓库目录；保留原有文件，不复制到仓库根目录覆盖现有 README。
4. 查看 Changes，确认没有密钥或意外删除；填写提交说明并 Commit，再点击 **Publish branch / Push origin**。
5. 点击 **Create Pull Request**，在 GitHub 复核后合并。完整源码的配置说明在其 `docs/LOCAL-QUICKSTART.md`。

上传源码只保存开发成果，不会迁移团队数据库，不会连上原云端密钥，也不会自动更新现有网站。现有网站仍按其部署流程发布；GitHub Pages 本身不能直接运行此应用的服务端、数据库和模型调用。
