# 🗺️ 俄乌战争战线图 · Ukraine Frontline Map

选择日期，查看俄乌战争实时战线变化。数据源自 **DeepStateMap**，每日自动更新。

## 🚀 一分钟部署到 GitHub Pages（完全免费）

### 前提
- 有一个 GitHub 账号（没有的话去 [github.com](https://github.com) 注册，1 分钟）

### 步骤

**① 创建新仓库**
- 登录 GitHub，点右上角 `+` → `New repository`
- 仓库名填 `ukraine-frontline-map`（或其他你喜欢的名字）
- 选 **Public**（公开，这样别人才能访问）
- 点 `Create repository`

**② 上传文件**
```bash
# 在电脑上操作（或者在 GitHub 网页端直接上传也行）
git clone https://github.com/你的用户名/ukraine-frontline-map.git
cd ukraine-frontline-map
# 把 index.html 复制到这个目录
git add index.html
git commit -m "初始化：俄乌战争战线图"
git push
```

不想用命令行？直接在 GitHub 仓库页面点 `Add file` → `Upload files`，把 `index.html` 拖进去就行。

**③ 开启 GitHub Pages**
- 进仓库 → `Settings` → `Pages`
- `Source` 选 `Deploy from a branch`
- `Branch` 选 `main`，目录选 `/ (root)`
- 点 `Save`
- 等 1-2 分钟，页面顶部会出现一行蓝字：`Your site is live at https://你的用户名.github.io/ukraine-frontline-map/`

**搞定！** 复制那个链接发给任何人就能打开。

## 📖 使用说明

| 操作 | 说明 |
|------|------|
| 📅 选日期 | 顶栏日期选择器，点开日历选任意日期 |
| 🔗 分享链接 | 选好日期后直接复制浏览器地址栏的链接发给别人 |
| 🔄 今日 | 点「今日」按钮回到最新数据 |
| 🗺️ 缩放 | 鼠标滚轮 / 双指手势 |
| ⌨️ 按 R | 重置地图视角到乌克兰全境 |

## 📊 数据说明

- **数据来源**：DeepStateMap（开源情报分析，乌克兰军方多源交叉验证）
- **数据范围**：2024年7月8日 ~ 至今（每日更新）
- **红色区域**：俄罗斯占领/控制区域
- **面积数据**：基于 GeoJSON 计算，仅供参考

## 🛠 技术栈

- Leaflet.js（地图引擎）
- Turf.js（地理空间计算）
- CartoDB（深色底图）
- GitHub Pages（免费托管）

## 📄 许可

本项目仅用于信息展示，数据版权归 DeepStateMap 所有。
