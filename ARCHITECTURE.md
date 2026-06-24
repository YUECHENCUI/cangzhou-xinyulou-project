# 信誉楼·港湾生活中心项目 - 架构文档

## 当前状态

- `index.html`: 当前单文件版本（所有内容在一个文件中）
- `v1.0.html`, `v2.0-*.html`: 历史版本

## 推荐的架构方案

### 目录结构

```
cangzhou-xinyulou-project/
├── src/                          # 源代码目录
│   ├── assets/
│   │   ├── images/               # 图片资源
│   │   │   ├── hero/
│   │   │   ├── project/
│   │   │   └── architecture/
│   │   └── styles/               # 样式文件
│   │       ├── main.css          # 基础样式
│   │       ├── nav.css           # 导航样式
│   │       ├── slides.css        # 幻灯片基础样式
│   │       ├── hero.css          # Hero样式
│   │       ├── intro.css         # 引言样式
│   │       ├── era.css           # 时代演进样式
│   │       ├── evolution.css     # 进化表样式
│   │       ├── anaya.css         # 阿那亚分析样式
│   │       ├── project-intro.css # 项目介绍样式
│   │       ├── brand.css         # 品牌样式
│   │       ├── positioning.css   # 定位样式
│   │       ├── ip.css            # 三大IP样式
│   │       ├── arch.css          # 建筑样式
│   │       ├── program.css       # 项目业态样式
│   │       ├── conclusion.css    # 结语样式
│   │       ├── image-slide.css   # 图片幻灯片样式
│   │       ├── scroll-hint.css   # 滚动指示样式
│   │       ├── responsive.css    # 响应式样式
│   │       └── all.css           # 样式入口文件
│   ├── sections/                 # HTML 章节组件
│   │   ├── 01-cover.html
│   │   ├── 02-hero.html
│   │   ├── 03-intro.html
│   │   ├── 04-era1.html
│   │   ├── 05-era2.html
│   │   ├── 06-era3.html
│   │   ├── 07-evolution.html
│   │   ├── 08-image1.html
│   │   ├── 09-era4.html
│   │   ├── 10-project-intro.html
│   │   ├── 11-image2.html
│   │   ├── 12-brand.html
│   │   ├── 13-positioning.html
│   │   ├── 14-image3.html
│   │   ├── 15-ip.html
│   │   ├── 16-arch.html
│   │   ├── 17-program.html
│   │   └── 18-conclusion.html
│   ├── scripts/
│   │   └── main.js
│   └── index.html                # 主入口文件
├── dist/                         # 构建输出目录
├── package.json                  # 项目配置
├── vite.config.js                # Vite 配置
└── README.md
```

### 快速迁移方案

#### 方案一：渐进式重构（推荐）

1. 保留原 `index.html` 作为备份和参考
2. 创建新的模块化结构
3. 逐步迁移内容

#### 方案二：使用构建工具

```bash
# 1. 安装依赖
npm install

# 2. 开发模式
npm run dev

# 3. 构建生产版本
npm run build
```

### 下一步行动

1. **HTML 组件化**: 拆分各幻灯片为独立文件
2. **脚本模块化**: 将页面交互逻辑移至 `src/scripts/`
3. **内容管理**: 考虑将文本内容抽取为 JSON

---

*文件创建于 2026年6月*
