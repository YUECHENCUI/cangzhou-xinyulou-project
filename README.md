# 信誉楼·港湾生活中心

项目概念设计提案

## 项目概述

这是信誉楼沧州总部店的项目概念设计提案网站，讲述了从「货的时代」到「归属的时代」的商业演进，以及信誉楼如何将四十年积累的信任关系转化为空间、服务、内容与公共生活。

## 当前文件结构

```
cangzhou-xinyulou-project/
├── index.html                                    # 主文件（当前完整版本）
├── v1.0.html                                     # 历史版本
├── v2.0-xinyulou-presentation-harbor-with-images.html  # 历史版本
├── v2.0-xinyulou_harbor_life_center_updated.md  # 历史文档
├── xinyu-lou-commercial-evolution.md            # 历史文档
├── package.json                                  # 项目配置
├── vite.config.js                                # Vite 配置
├── ARCHITECTURE.md                               # 架构文档
├── README.md                                     # 本文件
└── src/                                          # 新架构目录（开发中）
    ├── assets/styles/                            # 样式文件
    └── sections/                                 # 章节组件
```

## 使用方法

### 直接使用（当前）

直接在浏览器中打开 `index.html` 即可查看演示。

### 使用 Vite 开发服务器（新架构）

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev

# 构建生产版本
npm run build
```

## 架构重构进度

- [x] 创建新的目录结构
- [x] 初始化项目配置文件 (package.json, vite.config.js)
- [x] 完成样式文件拆分
- [x] 创建架构文档
- [x] 将 Base64 图片提取为 AVIF/WebP 资源
- [ ] 拆分 HTML 章节

## 详细文档

请参见 `ARCHITECTURE.md` 了解完整的架构设计方案。
