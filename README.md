# TCL PowerIN 660 视频预览

首页按顺序列出 12 个操作视频主题。每个主题都有独立链接，视频待上传时页面显示 `Video coming soon.`。

## 上传视频

在 GitHub 打开下表对应的目录，选择 **Add file → Upload files**。按表中的文件名上传 MP4，并提交到 `main`。启用 GitHub Pages 后，工作流会自动截取视频首帧附近的画面作封面，并发布原始 MP4。同名替换时，视频地址会随内容更新，主题页链接保持稳定。

| # | 页面 | 仓库内视频路径 |
|---|---|---|
| 1 | [Turbo Fast Cooling](./turbo-fast-cooling/) | `turbo-fast-cooling/turbo-fast-cooling.mp4` |
| 2 | [90° Wide-Angel Airflow](./90-wide-angle-airflow/) | `90-wide-angle-airflow/90-wide-angle-airflow.mp4` |
| 3 | [Customized Airflow Ⅰ](./customized-airflow-1/) | `customized-airflow-1/customized-airflow-1.mp4` |
| 4 | [Customized Airflow Ⅱ](./customized-airflow-2/) | `customized-airflow-2/customized-airflow-2.mp4` |
| 5 | [Smart Energy Saving](./smart-energy-saving/) | `smart-energy-saving/smart-energy-saving.mp4` |
| 6 | [Vertical Swing](./vertical-swing/) | `vertical-swing/vertical-swing.mp4` |
| 7 | [Easy Cleaning](./easy-cleaning/) | `easy-cleaning/easy-cleaning.mp4` |
| 8 | [Self-Cleaning](./self-cleaning/) | `self-cleaning/self-cleaning.mp4` |
| 9 | [APP Connection](./app-connection/) | `app-connection/app-connection.mp4` |
| 10 | [GEN Mode](./gen-mode/) | `gen-mode/gen-mode.mp4` |
| 11 | [Arrive / Leave Home Mode](./arrive-leave-home-mode/) | `arrive-leave-home-mode/arrive-leave-home-mode.mp4` |
| 12 | [Negative Ionic Generator](./negative-ionic-generator/) | `negative-ionic-generator/negative-ionic-generator.mp4` |

## 本地预览

在仓库根目录执行下列命令，打开 <http://localhost:8000/>。使用 Python 3，输出目录须不存在或为空。已有视频时需要 FFmpeg 生成封面。

```sh
python3 build_pages.py _site
python3 -m http.server 8000 --directory _site
```

## GitHub Pages

在仓库的 **Settings → Pages** 中将 **Source** 设为 **GitHub Actions**。首次可在 **Actions** 中手动运行 **Publish TCL PowerIN 660 to Pages**，后续提交到 `main` 时自动运行。仓库使用的账户方案和可见性须支持 GitHub Pages。

页面和播放器基于 [voxin-evo-t4](https://github.com/TCL-Air-Conditioner/voxin-evo-t4) 的模板。
