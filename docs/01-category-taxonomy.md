# 01 - 分类体系（大类 → 板块 → 模块）

## 设计原则

- **大类（Category）**：按行业领域划分，对应 YAML 二级菜单
- **板块（Sector）**：大类内的一级分组，对应 YAML ThirdGroup
- **模块（Module）**：板块内的二级分组（可选），对应 YAML NestedGroup
- 层级：`大类 → 板块 → 模块`，模块可省略

## 完整分类树

### highway（公路标准）— 已完成

| 板块 | 模块 |
|---|---|
| overview（总体） | — |
| general（通用） | basics / safety / green / smart / project |
| construction（建设） | survey / bridge-tunnel / route / subgrade / pavement / bridge / tunnel / traffic / expansion / drawings / test / inspection / construction / supervision / cost |
| management（管理） | — |
| maintenance（养护） | comprehensive / inspection / design / construction / cost |
| operation（运营） | toll / emergency / v2x |

### railway（铁路标准）

| 板块 | 模块 |
|---|---|
| overview（总体） | — |
| design（设计） | line / subgrade / track / bridge / tunnel / station |
| construction（施工） | — |
| supervision（监理） | — |
| test（试验检测） | — |
| maintenance（养护维修） | — |
| operation（运营） | — |

### municipal（市政标准）

| 板块 | 模块 |
|---|---|
| road（道路） | — |
| bridge（桥梁） | — |
| drainage（给排水） | — |
| gas（燃气） | — |
| heat（热力） | — |
| power（电力） | — |
| green（园林环卫） | — |

### survey（测绘通用）

| 板块 | 模块 |
|---|---|
| general（基础测绘） | — |
| engineering（工程测量） | — |
| geodesy（大地测量） | — |
| gnss（卫星定位） | — |
| mapping（地图制图） | — |
| remote-sensing（遥感） | — |

### national（通用国标）

| 板块 | 模块 |
|---|---|
| structure（结构） | — |
| foundation（地基基础） | — |
| seismic（抗震） | — |
| material（材料） | — |
| safety（安全） | — |
| management（管理） | — |

### water（水利标准）

| 板块 | 模块 |
|---|---|
| design（设计） | — |
| construction（施工） | — |
| maintenance（养护） | — |
| operation（运营） | — |

### bridge（桥梁标准）

| 板块 | 模块 |
|---|---|
| design（设计） | — |
| construction（施工） | — |
| maintenance（养护） | — |
| test（检测） | — |

### sizheng（四证标准）

| 板块 | 模块 |
|---|---|
| land（建设用地规划许可证） | — |
| planning（建设工程规划许可证） | — |
| construction（施工许可证） | — |
| property（不动产权证） | — |

## 新增大类流程

1. 在此文件登记新大类（大类码、中文、标准前缀）
2. 定义板块-模块结构
3. 在 `03-release-matrix.md` 添加 Release 列表
4. 创建对应空 Release 骨架
5. 在 YAML 中添加二级菜单
