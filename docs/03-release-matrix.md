# 03 - Release 划分矩阵（全大类）

## 总览

| 大类 | Release 数 | 状态 |
|---|---|---|
| highway | 30 | ✅ 已填充 |
| railway | 12 | ⏳ 空骨架 |
| municipal | 7 | ⏳ 空骨架 |
| survey | 6 | ⏳ 空骨架 |
| national | 6 | ⏳ 空骨架 |
| water | 4 | ⏳ 空骨架 |
| bridge | 4 | ⏳ 空骨架 |
| sizheng | 4 | ⏳ 空骨架 |
| **合计** | **73** | |

## highway（公路标准）— 30 个

| Release Tag | 板块-模块 |
|---|---|
| highway-overview-v1 | 总体 |
| highway-general-basics-v1 | 通用-基础 |
| highway-general-safety-v1 | 通用-安全 |
| highway-general-green-v1 | 通用-绿色 |
| highway-general-smart-v1 | 通用-智慧 |
| highway-general-project-v1 | 通用-项目管理 |
| highway-construction-survey-v1 | 建设-勘测 |
| highway-construction-bridge-tunnel-v1 | 建设-桥隧 |
| highway-construction-route-v1 | 建设-路线 |
| highway-construction-subgrade-v1 | 建设-路基 |
| highway-construction-pavement-v1 | 建设-路面 |
| highway-construction-bridge-v1 | 建设-桥涵 |
| highway-construction-tunnel-v1 | 建设-隧道 |
| highway-construction-traffic-v1 | 建设-交安 |
| highway-construction-expansion-v1 | 建设-改扩建 |
| highway-construction-drawings-v1 | 建设-通用图 |
| highway-construction-test-v1 | 建设-试验 |
| highway-construction-inspection-v1 | 建设-检测 |
| highway-construction-construction-v1 | 建设-施工 |
| highway-construction-supervision-v1 | 建设-监理 |
| highway-construction-cost-v1 | 建设-造价 |
| highway-management-v1 | 管理 |
| highway-maintenance-comprehensive-v1 | 养护-综合 |
| highway-maintenance-inspection-v1 | 养护-检测评价 |
| highway-maintenance-design-v1 | 养护-养护设计 |
| highway-maintenance-construction-v1 | 养护-养护施工 |
| highway-maintenance-cost-v1 | 养护-造价 |
| highway-operation-toll-v1 | 运营-收费服务 |
| highway-operation-emergency-v1 | 运营-应急处置 |
| highway-operation-v2x-v1 | 运营-车路协同 |

## railway（铁路标准）— 12 个

| Release Tag | 板块-模块 |
|---|---|
| railway-overview-v1 | 总体 |
| railway-design-line-v1 | 设计-线路 |
| railway-design-subgrade-v1 | 设计-路基 |
| railway-design-track-v1 | 设计-轨道 |
| railway-design-bridge-v1 | 设计-桥涵 |
| railway-design-tunnel-v1 | 设计-隧道 |
| railway-design-station-v1 | 设计-站场 |
| railway-construction-v1 | 施工 |
| railway-supervision-v1 | 监理 |
| railway-test-v1 | 试验检测 |
| railway-maintenance-v1 | 养护维修 |
| railway-operation-v1 | 运营 |

## municipal（市政标准）— 7 个

| Release Tag | 板块 |
|---|---|
| municipal-road-v1 | 道路 |
| municipal-bridge-v1 | 桥梁 |
| municipal-drainage-v1 | 给排水 |
| municipal-gas-v1 | 燃气 |
| municipal-heat-v1 | 热力 |
| municipal-power-v1 | 电力 |
| municipal-green-v1 | 园林环卫 |

## survey（测绘通用）— 6 个

| Release Tag | 板块 |
|---|---|
| survey-general-v1 | 基础测绘 |
| survey-engineering-v1 | 工程测量 |
| survey-geodesy-v1 | 大地测量 |
| survey-gnss-v1 | 卫星定位 |
| survey-mapping-v1 | 地图制图 |
| survey-remote-sensing-v1 | 遥感 |

## national（通用国标）— 6 个

| Release Tag | 板块 |
|---|---|
| national-structure-v1 | 结构 |
| national-foundation-v1 | 地基基础 |
| national-seismic-v1 | 抗震 |
| national-material-v1 | 材料 |
| national-safety-v1 | 安全 |
| national-management-v1 | 管理 |

## water（水利标准）— 4 个

| Release Tag | 板块 |
|---|---|
| water-design-v1 | 设计 |
| water-construction-v1 | 施工 |
| water-maintenance-v1 | 养护 |
| water-operation-v1 | 运营 |

## bridge（桥梁标准）— 4 个

| Release Tag | 板块 |
|---|---|
| bridge-design-v1 | 设计 |
| bridge-construction-v1 | 施工 |
| bridge-maintenance-v1 | 养护 |
| bridge-test-v1 | 检测 |

## sizheng（四证标准）— 4 个

| Release Tag | 板块 |
|---|---|
| sizheng-land-v1 | 建设用地规划许可证 |
| sizheng-planning-v1 | 建设工程规划许可证 |
| sizheng-construction-v1 | 施工许可证 |
| sizheng-property-v1 | 不动产权证 |

## 新增 Release 流程

1. 在此矩阵中登记新 Release Tag
2. 通过 `gh release create` 创建空 Release
3. 在 YAML 中添加对应 ThirdGroup
