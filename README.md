# GitHub Pages 胶囊链接发布步骤

这个文件夹已经包含最简单的网页文件：`index.html`。

## 1. 在 GitHub 创建仓库

1. 打开 https://github.com 并登录。
2. 点击右上角 `+`，选择 `New repository`。
3. 仓库名填写 `love-capsule`。
4. 选择 `Public`。
5. 可以勾选 `Add a README file`，也可以不勾选。
6. 点击 `Create repository`。

## 2. 上传网页文件

把这个文件夹里的 `index.html` 上传到仓库根目录。

如果你想连说明文件也一起保存，可以同时上传 `README.md` 和 `paper-note-template.txt`。

## 3. 开启 GitHub Pages

1. 进入仓库页面。
2. 点击 `Settings`。
3. 左侧点击 `Pages`。
4. 在 `Build and deployment` 中选择：
   - `Source`: `Deploy from a branch`
   - `Branch`: `main`
   - Folder: `/root`
5. 点击 `Save`。

## 4. 获取网站地址

等待 1 到 10 分钟后，刷新 `Settings` -> `Pages`。

你的网站地址是：

```text
https://nosleeeeeep.github.io/love-capsule/
```

她打开这个地址会直接看到网页，不会进入 GitHub 仓库界面。

## 5. 生成二维码

搜索 `网址生成二维码`，把上面的网站地址粘进去，保存生成的二维码。

## 6. 写进胶囊纸条

纸条可以使用 `paper-note-template.txt` 里的格式。

为了长期可用：

- 不要删除 GitHub 仓库。
- 不要改仓库名。
- 不要关闭 GitHub Pages。
- 二维码下面最好手写一份网址，避免二维码磨损。
