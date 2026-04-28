<div align="center">

# :fire: 本质安全智能施工防火系统

**Intrinsically Safe Intelligent Construction Fire Prevention System**

基于"本质安全"理念的香港城市更新中建筑施工火灾智能预警方案设计

<br/>

![](https://img.shields.io/badge/理念-本质安全-FF6F61?style=for-the-badge&labelColor=2D2D2D)
![](https://img.shields.io/badge/场景-香港城市更新-4A90D9?style=for-the-badge&labelColor=2D2D2D)
![](https://img.shields.io/badge/技术-AI%20%2B%20IoT%20%2B%20LSTM-50C878?style=for-the-badge&labelColor=2D2D2D)

![](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![](https://img.shields.io/badge/NFPA_72-合规-FF4500?style=flat-square)
![](https://img.shields.io/badge/GB_50116-合规-FF4500?style=flat-square)

<br/>

</div>

<br/>

---


https://github.com/user-attachments/assets/ac7fc1e6-cce4-49e5-9a86-1229488d1e6a



## :bookmark_tabs: 目录

<details open>
<summary><b>展开 / 收起</b></summary>
<br/>

- [:fire: 本质安全智能施工防火系统](#fire-本质安全智能施工防火系统)
  - [:bookmark\_tabs: 目录](#bookmark_tabs-目录)
  - [:star2: 项目简介](#star2-项目简介)
  - [:brain: 核心理念](#brain-核心理念)
  - [:building\_construction: 系统架构](#building_construction-系统架构)
  - [:jigsaw: 三层管控体系](#jigsaw-三层管控体系)
    - [:one: 第一层：风险隔离 `Risk Isolation`](#one-第一层风险隔离-risk-isolation)
    - [:two: 第二层：过程控制 `Process Control`](#two-第二层过程控制-process-control)
    - [:three: 第三层：感知预警 `Perception & Warning`](#three-第三层感知预警-perception--warning)
  - [:open\_file\_folder: 目录结构](#open_file_folder-目录结构)
  - [:wrench: 技术栈](#wrench-技术栈)
  - [:rocket: 快速开始](#rocket-快速开始)
  - [:movie\_camera: 演示流程](#movie_camera-演示流程)
    - [:one: 第一层 — 风险隔离](#one-第一层--风险隔离)
    - [:two: 第二层 — 过程控制](#two-第二层--过程控制)
    - [:three: 第三层 — 感知预警](#three-第三层--感知预警)
  - [:scroll: 合规参考](#scroll-合规参考)
  - [:balance\_scale: 声明](#balance_scale-声明)

</details>

<br/>

---

## :star2: 项目简介

本系统是一个面向**香港城市更新建筑施工场景**的火灾智能预警交互式演示系统（Demo），以 **"宏福苑城市更新项目"** 为实际案例，展示如何通过 AI 视觉识别、多传感器融合和 LSTM 预测模型，构建 **"先预防 → 再控制 → 后感知"** 的三层防火管控体系。

<br/>

---

## :brain: 核心理念

> **本质安全**：在火灾三要素（火源、可燃物、人员）共存之前，通过空间隔离和智能监控将其分离，将安全关口前移。

```
传统消防：  火灾发生 → 被动响应 → 事后扑救
                  ↓
本质安全：  风险识别 → 主动隔离 → 源头消除
```

| 传统模式 | 本质安全模式 |
|:--------:|:----------:|
| 事后灭火 | 事前预防 |
| 人工巡查 | AI 智能识别 |
| 单一传感器 | 多传感器融合 |
| 经验判断 | LSTM 预测模型 |

<br/>

---

## :building_construction: 系统架构

```
┌───────────────────────────────────────────────────────────┐
│                  本质安全智能施工防火系统                    │
├────────────────┬──────────────────┬───────────────────────┤
│   第一层        │    第二层         │    第三层              │
│   风险隔离      │    过程控制       │    感知预警            │
│                │                  │                       │
│  AI 视觉识别   │  动火作业审批     │  多传感器融合监测      │
│  区域冲突检测   │  安全检查清单     │  LSTM 风险预测        │
│  空间隔离管控   │  实时作业监控     │  紧急调度与处置        │
│                │                  │                       │
│   🔍 预防       │    🔒 控制        │    ⚡ 感知             │
└────────────────┴──────────────────┴───────────────────────┘
```

<br/>

---

## :jigsaw: 三层管控体系

### :one: 第一层：风险隔离 `Risk Isolation`

> 利用 AI 视觉识别施工现场区域布局，检测功能区之间的空间冲突

- :red_circle: **动火作业区** — 焊接、切割等产生明火的区域
- :orange_circle: **可燃材料堆放区** — 木材、油漆等易燃物存放区
- :large_blue_circle: **人员通行区** — 施工人员日常行走路线
- :green_circle: **疏散通道** — 紧急撤离通道
- :white_circle: **一般施工区** — 普通施工作业区域
- :purple_circle: **临时办公/休息区** — 工人休息与办公区域

**三级冲突检测**：

| 级别 | 状态 | 处置措施 |
|:---:|:---:|:------:|
| :yellow_circle: 轻度 | 黄灯提示 | 记录并提醒注意 |
| :orange_circle: 中度 | 橙色告警 | 通知安全负责人 |
| :red_circle: 严重 | 红灯锁定 | **自动禁止动火作业** |

---

### :two: 第二层：过程控制 `Process Control`

> 动火作业审批与开工前安全检查的全流程管理

**动火审批信息**：

| 项目 | 内容 |
|:---:|:---:|
| 作业位置 | A区外墙 6F |
| 作业类型 | 电焊作业 |
| 作业人员 | 张伟（焊工证 #2024-0892） |
| 监护人员 | 王强（安全员） |
| 作业时间 | 10:00 — 16:00 |
| 灭火器配置 | ABC干粉 ×2 |

**5 项安全检查清单**：

- [x] 周边可燃物是否清除
- [x] 灭火器是否到位
- [x] 监护人是否在岗
- [x] 疏散通道是否畅通
- [x] 作业区域是否已隔离

---

### :three: 第三层：感知预警 `Perception & Warning`

> 多传感器融合监测 + LSTM 预测模型 + 灾情处置闭环

**传感器融合**：

| 传感器 | 原理 | 灵敏度 |
|:------:|:----:|:------:|
| :thermometer: 温度传感器 | ΔT/Δt 差分温升算法 | ±0.5°C |
| :eye: VFDS 视觉火焰侦测 | 多光谱极早期烟火侦测 | 极早期 |
| :dash: ASD 进吸式烟雾探测 | 激光散射原理 | 0.003% obs/m |

**LSTM 预警分级**：

| 级别 | 触发条件 | 系统响应 |
|:---:|:-------:|:------:|
| :yellow_circle: 预警 | 单传感器异常 / LSTM > 30% | 橙色提示 |
| :orange_circle: 警告 | 多传感器交叉异常 / LSTM > 70% | 黄色警告 + 脉冲动画 |
| :red_circle: 紧急 | 确认火灾 / LSTM > 90% | 红色紧急 + 持续闪烁 + 自动调度 |

**处置闭环流程**：

```
灾情发生 → 热成像确认 → 紧急调度 → 现场处置 → 余火检查 → 30min 复检 → 二次巡查 → 复查照片上传
```

<br/>

---

## :open_file_folder: 目录结构

```
本质安全智能施工防火系统demo/
├── 点击这个文件打开系统demo.html          # :door: 主入口文件
├── README.md                              # :page_facing_up: 项目说明文档
│
├── layer1-risk-video.mp4                  # :movie_camera: 第一层风险扫描演示视频
├── layer2-complete-video.mp4              # :movie_camera: 第二层作业监控演示视频
│
├── css/                                   # :art: 样式文件
│   └── style.css                          #    └── 全局样式表
│
├── js/                                    # :gear: 脚本文件
│   ├── common.js                          #    ├── 公共工具类
│   ├── layer1-risk.js                     #    ├── 第一层：风险隔离逻辑
│   ├── layer2-process.js                  #    ├── 第二层：过程控制逻辑
│   └── layer3-perception.js               #    └── 第三层：感知预警逻辑
│
└── images/                                # :framed_picture: 图片资源
    ├── fire-zone-plan.png                 #    ├── 施工现场平面布局图
    ├── layer1-initial.png                 #    ├── 第一层初始监控画面
    ├── layer1-risk.png                    #    ├── 第一层风险检测结果
    ├── layer2-complete.png                #    ├── 第二层监控画面
    ├── layer3-hazard.png                  #    ├── 第三层隐患检测画面
    ├── layer3-thermal.png                 #    ├── 热成像照片
    ├── layer4-resolved.png                #    ├── 处置完毕画面
    ├── fire-warning-roadmap.png           #    ├── 火灾预警系统路线图
    ├── temperature-sensor.png             #    ├── 温度传感器详情图
    ├── vfds-sensor.png                    #    ├── VFDS传感器详情图
    └── asd-sensor.png                     #    └── ASD传感器详情图
```

<br/>

---

## :wrench: 技术栈

| 类别 | 技术 | 说明 |
|:---:|:---:|:---:|
| :globe_with_meridians: 前端 | HTML + CSS + JavaScript | 纯原生，零框架依赖 |
| :art: CSS 框架 | Tailwind CSS | CDN 引入，原子化样式 |
| :abc: 字体 | Rajdhani + Noto Sans SC | Google Fonts 中英混排 |
| :sparkles: 动画 | CSS Animations | shimmer / fadeIn / pulse-glow 等 20+ 种 |
| :straight_ruler: 布局 | CSS Grid + Flexbox | 响应式设计，移动端适配 |
| :movie_camera: 媒体 | MP4 + PNG | 视频演示 + 图片资源 |
| :scroll: 合规 | NFPA 72 / GB 50116 | 国际与国内消防标准 |

<br/>

---

## :rocket: 快速开始

本项目为纯静态前端页面，**无需安装任何依赖**。

```bash
# 1. 克隆项目
git clone <仓库地址>

# 2. 进入项目目录
cd 本质安全智能施工防火系统demo

# 3. 直接用浏览器打开入口文件
# Windows: 双击 "点击这个文件打开系统demo.html"
# macOS:   open "点击这个文件打开系统demo.html"
# Linux:   xdg-open "点击这个文件打开系统demo.html"
```

> :bulb: **提示**：需要网络连接以加载 CDN 资源（Tailwind CSS、Google Fonts）。推荐使用 Chrome / Edge / Firefox 现代浏览器。

<br/>

---

## :movie_camera: 演示流程

### :one: 第一层 — 风险隔离

```
[开始演示扫描] → 扫描线动画 → AI 区域识别 → 冲突检测结果弹窗 → 处置措施
```

1. 进入页面后默认展示第一层"风险隔离"
2. 点击 **「开始演示扫描」** 按钮
3. 观察红色扫描线动画对施工现场进行 AI 识别
4. 查看冲突检测结果弹窗及系统处置措施

### :two: 第二层 — 过程控制

```
[开始检测] → 逐项安全检查（5项） → 全部通过 → [允许作业] → 切换实时监控
```

1. 切换到第二层"过程控制"标签页
2. 点击 **「开始检测」** 按钮
3. 观察 5 项安全检查逐项自动完成（每项间隔 900ms）
4. 全部通过后点击 **「允许作业」** 批准动火

### :three: 第三层 — 感知预警

```
[灾情发生] → LSTM 概率攀升 → 传感器告警 → 热成像确认 → 紧急调度 → 处置闭环 → 30min 复检
```

1. 切换到第三层"感知预警"标签页
2. 点击 **「灾情发生」** 按钮
3. 观察 LSTM 概率从 0% 攀升至 86%，传感器数值同步变化
4. 查看热成像照片，确认灾情
5. 观察紧急调度动画（自动联系负责人）
6. 确认处置完毕，系统恢复正常状态

<br/>

---

## :scroll: 合规参考

| 标准 | 全称 | 适用范围 |
|:---:|:---:|:---:|
| **NFPA 72** | 美国国家火灾报警和信号规范 | 国际消防报警标准 |
| **GB 50116** | 火灾自动报警系统设计规范 | 中国国家标准 |

<br/>

---

## :balance_scale: 声明

  ▎ :information_source:
  ▎ 本项目为课程作业演示系统（Demo），所有数据均为模拟数据，仅用于展示系统设计理念和核心功能，不构成实际生产部署方案。

  ▎ :robot: AI 生成内容说明：本演示系统中的监控图片由 GPT-Image 2.0 生成，演示视频由 豆包（Doubao） 生成，均为 AI
  ▎ 辅助创作的模拟素材，仅供参考演示使用。


<div align="center">

**本质安全智能施工防火系统** · 2026

</div>
