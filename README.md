# pnpm-utils-demo

基于pnpm workspace创建工具库demo项目

# 目录结构

项目采用 Monorepo 进行代码管理，下面展示了主要目录结构

```shell
root
├── docs                     # 文档
│   ├── guide                # 指引文档
│   │   └── index.md
│   └── packages
│            └── core        # 函数展示文档
│                └── getDevice
                       └── index.md # 函数方法文档
├── packages
│   ├──  core                # 主工具函数 Utils 集合
│   │   ├── getDevice
│   │   ├── getxxxx
│   │   └── 其它
│   └── shared               # 主工具函数公用方法集合
│       ├── is               # 方法集合
│       ├── xx
│       └── 其它              # 其它
└── playground               # 本地开发调试操场
```

工具函数目录结构 (以`getDevice`为例)：

```shell
# packages/core/getDevice
core
└──getDevice
   ├── index.test.ts         # 单元测试
   └── index.ts              # 函数方法入口
```
