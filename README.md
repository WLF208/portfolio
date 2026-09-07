# 王琨 · 嵌入式软件工程师作品集

单页作品集，面向 HR 和技术面试官展示嵌入式项目经历。页面上可以看到项目背景、技术栈、关键指标、架构链路和成果链接。

## 怎么看

- 在线作品集：<https://wlf208.github.io/portfolio/>
- 本地预览：双击 `index.html`
- 源码仓库：<https://github.com/WLF208/portfolio>

## 项目内容

1. 双闭环 PID 自平衡小车：MPU6050 姿态解算、串级 PID、编码器测速、WiFi 调试。
2. FreeRTOS + LVGL 示波器：ADC + DMA 采集、环形缓冲、FreeRTOS 任务划分、LVGL 波形显示。
3. Linux + Qt 车载副屏：CAN 总线数据解析、MVVM 架构、QML 仪表盘、OpenGL ES 渲染。

## 目录结构

```text
作品集/
├── index.html              网页入口
├── README.md               本说明文件
├── .nojekyll               GitHub Pages 标记
├── .gitignore              不上传规则
├── assets/js/              本地图标库
├── images/                 公开项目图片，会上传
└── private/                私有资料，不上传
```

## 公开内容和私有内容

会发布到 GitHub 的内容：

- `index.html`
- `images/` 里的项目照片、截图
- `assets/`
- `README.md`

不会发布的内容：

- `private/` 里的所有文件，例如简历、证书、设计原稿、Token

`private/作品集资料规划.md` 里有一份本地资料规划，按里面的清单准备素材即可。

## 日常更新

1. 把要公开的照片放到 `images/`
2. 编辑 `index.html` 替换示意图和链接
3. 双击 `index.html` 本地预览
4. 在作品集目录执行：

```powershell
git add .
git commit -m "更新作品集"
git push
```

5. 等 1-2 分钟，刷新在线链接查看

详细操作见 `作品集使用教程.md`。
