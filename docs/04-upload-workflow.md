# 04 - 新增规范标准操作流程（SOP）

## 完整流程

### 步骤 1：确定分类

- 查 `01-category-taxonomy.md` 确定大类、板块、模块
- 查 `03-release-matrix.md` 确认对应 Release Tag 是否已存在

### 步骤 2：生成 Tag

按 `02-naming-convention.md` 规则：
1. 清洗标准编号（去空格、全角转半角、处理 `/` 和括号）
2. 组合菜单项 Tag = `{Release前缀}_{清洗后编号}`
3. 校验同 Release 内无重名

### 步骤 3：加密 PDF

```powershell
# 使用 QuickTools 加密工具（或项目内置加密脚本）
# 输出文件名 = {菜单项Tag}.enc
```

### 步骤 4：上传到 Release

```powershell
$gh = "C:\Program Files\GitHub CLI\gh.exe"
& $gh release upload {ReleaseTag} "{菜单项Tag}.enc" --repo wzhgno/QuickTools-standards
```

### 步骤 5：更新 YAML

在 `FeatureConfig.yaml` 对应三级分组下添加菜单项：

```yaml
- Id: "item_resources_XX_YY_ZZ"
  ParentId: "group_resources_XX_YY"
  CustomName: "规范中文名"
  Tooltip: "编号 规范中文名"
  LicenseLevel: "Free"
  FunctionStrategy: "StandardDocumentViewer"
  Tag: "{菜单项Tag}"
  Draggable: true
  DropZone: ["group_*", "item_*"]
```

### 步骤 6：重新生成 T4 + 编译

```powershell
# 重新运行 T4 模板生成 UIConfig.g.cs 和 LicenseMapping.g.cs
# 用 MSBuild 编译验证
```

## 批量新增规范

当一次新增多条规范时：
1. 按板块-模块分组
2. 同组内按编号排序
3. 统一生成 Tag、加密、上传
4. 批量更新 YAML
5. 一次性重跑 T4 + 编译

## 校验清单

每次新增完成后检查：
- [ ] Release 存在且 Tag 正确
- [ ] `.enc` 文件已上传到对应 Release
- [ ] YAML 菜单项 Tag 与文件名一致
- [ ] 下载 URL 可访问
- [ ] T4 重新生成
- [ ] 编译通过
