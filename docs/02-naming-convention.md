# 02 - 命名规则（Tag / Release / 文件名）

## 1. Release Tag 命名

```
{大类}-{板块}-{模块}-v{版本号}
```

| 部分 | 说明 | 示例 |
|---|---|---|
| 大类 | 英文码，见分类体系 | `highway` |
| 板块 | 英文 | `general` |
| 模块 | 英文，无模块则省略 | `basics` |
| 版本 | `v1` 起，批量更新时递增 | `v1` |

**示例**：
- `highway-overview-v1`（无模块）
- `highway-general-basics-v1`（有模块）
- `railway-design-line-v1`

## 2. 菜单项 Tag 命名

```
{Release前缀}_{标准编号}
```

- `Release前缀` = Release Tag 去掉 `-v版本`
- `标准编号` = 清洗后的标准号

**示例**：
- `highway-overview_JTG1001-2017`
- `highway-general-basics_JTGB01-2014`
- `railway-design-line_TB10001-2017`

## 3. 标准编号清洗规则

| 原始 | 清洗后 | 规则 |
|---|---|---|
| `JTG B01—2014` | `JTGB01-2014` | 去空格，`—`→`-` |
| `JTG/T D81—2017` | `JTGTD81-2017` | `/` 去除，`T` 保留区分推荐性 |
| `建标〔2011〕124号` | `JTJ2011-124` | `建标`→`JTJ`，`〔〕`→`-`，去`号` |
| `JTG/T 3381-02—2020` | `JTGT3381-02-2020` | 同上 |
| `GB 50026` | `GB50026` | 去空格 |
| `GB/T 24356` | `GBT24356` | `/` 去除 |

**通用规则**：
1. 去除所有空格
2. `—`（全角破折号）和 `–` → `-`（半角连字符）
3. `/` 去除（但保留 `T` 以区分推荐性标准）
4. `〔〕` `（）` `()` 等括号去除，括号内内容保留
5. `号` 字去除
6. `建标` → `JTJ`（行业惯例映射）

## 4. 加密文件名

```
{菜单项Tag}.enc
```

**示例**：`highway-general-basics_JTGB01-2014.enc`

## 5. 下载 URL

```
https://github.com/wzhgno/QuickTools-standards/releases/download/{ReleaseTag}/{菜单项Tag}.enc
```

**示例**：
```
https://github.com/wzhgno/QuickTools-standards/releases/download/highway-general-basics-v1/highway-general-basics_JTGB01-2014.enc
```

## 6. 命名校验清单

新增规范时检查：
- [ ] Release Tag 符合 `{大类}-{板块}-{模块}-v{版本}` 格式
- [ ] 菜单项 Tag = `{Release前缀}_{清洗后标准编号}`
- [ ] 标准编号已按规则清洗（无空格、无全角符号、`/` 已处理）
- [ ] 加密文件名 = `{菜单项Tag}.enc`
- [ ] 同一 Release 内无重名 Tag
