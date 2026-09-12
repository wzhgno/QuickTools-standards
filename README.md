# QuickTools 标准规范资源库

工程建设行业标准规范的加密分发仓库，配合 QuickTools 桌面端使用。

## 仓库结构

```
QuickTools-standards/
├── README.md                     # 本文件（总索引）
├── docs/
│   ├── 01-category-taxonomy.md   # 大类-板块-模块分类体系
│   ├── 02-naming-convention.md   # Tag/Release/文件名命名规则
│   ├── 03-release-matrix.md      # 全大类 Release 划分矩阵
│   └── 04-upload-workflow.md     # 新增规范的标准操作流程
├── highway/                      # 公路标准（JTG 系列）
├── railway/                      # 铁路标准（TB 系列）
├── municipal/                    # 市政标准（CJJ 系列）
├── survey/                       # 测绘通用（GB 测绘类）
├── national/                     # 通用国标（GB 通用类）
├── water/                        # 水利标准（SL 系列）
├── bridge/                       # 桥梁标准（专项）
└── sizheng/                      # 四证标准
```

## 标准大类总览

| 大类码 | 中文 | 标准前缀 | Release 数 | 状态 |
|---|---|---|---|---|
| highway | 公路标准 | JTG | 30 | ✅ 已填充 179 项 |
| railway | 铁路标准 | TB | 12 | ⏳ 空骨架 |
| municipal | 市政标准 | CJJ | 7 | ⏳ 空骨架 |
| survey | 测绘通用 | GB 测绘 | 6 | ⏳ 空骨架 |
| national | 通用国标 | GB 通用 | 6 | ⏳ 空骨架 |
| water | 水利标准 | SL | 4 | ⏳ 空骨架 |
| bridge | 桥梁标准 | 专项 | 4 | ⏳ 空骨架 |
| sizheng | 四证标准 | 四证 | 4 | ⏳ 空骨架 |

**合计：73 个 Release**

## 下载 URL 规则

```
https://github.com/wzhgno/QuickTools-standards/releases/download/{ReleaseTag}/{Tag}.enc
```

- `ReleaseTag` = `{大类}-{板块}-{模块}-v{版本}`，如 `highway-general-basics-v1`
- `Tag` = `{Release前缀}_{标准编号}`，如 `highway-general-basics_JTGB01-2014`

## 快速链接

- [分类体系](./docs/01-category-taxonomy.md)
- [命名规则](./docs/02-naming-convention.md)
- [Release 矩阵](./docs/03-release-matrix.md)
- [上传流程](./docs/04-upload-workflow.md)
