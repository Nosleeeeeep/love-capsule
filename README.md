# Paper Note Link Pages

这是一个部署在 GitHub Pages 上的静态网页项目，用来承载部分纸质字条上写到的附加链接页面。纸质字条才是主体；网页只是某些字条里的补充体验，不要把项目理解成“纸条胶囊网页版”。后续 agent 请保持项目简单：纯 HTML/CSS/JS，尽量不要引入构建工具、服务器或框架。

## 线上地址

主页：

```text
https://nosleeeeeep.github.io/love-capsule/
```

第一个附加网页：

```text
https://nosleeeeeep.github.io/love-capsule/capsule-001.html
```

GitHub 仓库：

```text
https://github.com/Nosleeeeeep/love-capsule
```

## 文件放置规则

- `index.html` 是主页，可以放所有附加网页的入口链接。
- 每个独立附加网页放在仓库根目录，可以沿用 `capsule-001.html`、`capsule-002.html`、`capsule-003.html` 这种命名；这里的 `capsule` 只是历史文件名，不代表要把纸质字条做成网页版。
- 如果添加图片、音频或其他资源，新建 `assets/` 目录，并按页面分文件夹保存，例如 `assets/capsule-001/photo-1.jpg`。
- 不要提交 `.tools/`，它只是本地临时工具目录，已经在 `.gitignore` 中忽略。

新增网页示例：

```text
capsule-002.html
```

发布后的访问地址会是：

```text
https://nosleeeeeep.github.io/love-capsule/capsule-002.html
```

## 部署方式

这个仓库已经启用 GitHub Pages：

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/root`

部署流程：

1. 在本地修改或新增 `.html` / `assets` 文件。
2. 确认页面在本地可打开，复杂交互请用本地 HTTP 服务预览。
3. 提交改动：

   ```powershell
   git add .
   git commit -m "Add note link page"
   ```

4. 推送到 GitHub：

   ```powershell
   git push
   ```

5. GitHub Pages 会自动部署，通常几十秒到几分钟后生效。
6. 用最终 URL 验证页面是否能打开。

## 本地预览

简单页面可以直接双击 HTML 文件打开。涉及拖拽、动画或资源路径时，建议在项目根目录启动本地 HTTP 服务：

```powershell
python -m http.server 8000 --bind 127.0.0.1
```

然后访问：

```text
http://127.0.0.1:8000/capsule-001.html
```

## 当前页面

- `index.html`: 主页，包含第一个附加网页入口。
- `capsule-001.html`: 第一个附加网页。气球绑着信纸，向下拉后放飞，经过云和照片占位，最后气球爆开并展开信纸。
- `paper-note-template.txt`: 纸质字条里附加链接的文字模板。

## 给后续 agent 的注意事项

- 保持所有链接相对路径可用，例如从主页链接到 `capsule-001.html`。
- 新增页面后，同步更新 `index.html` 的入口和本 README 的“当前页面”列表。
- 不要把网页当作纸质字条的替代品；用户已经写了纸质字条，网页只是部分纸条上的链接附加内容。
- 公开仓库和 GitHub Pages 页面都是公开可访问的，不要放真实住址、手机号、身份证、私密账号或其他敏感信息。
- 照片资源尽量压缩，避免大文件影响手机加载。
- 不要改仓库名、默认分支或 GitHub Pages 设置，除非用户明确要求。
