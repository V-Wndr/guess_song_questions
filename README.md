# 歌单库

## 概述
本仓库用于存储歌单文件，所有歌单均以 `.xlsx` 格式保存。每个文件代表一个歌单，包含歌曲名称及其别称。通过统一的模板格式，系统能够自动识别并加载文件内容。

## 文件要求
- **文件格式**：必须为 `.xlsx`。
- **模板结构**：
  - **第一行**：列标题，仅占位，无实际解析功能。
  - **第二行及以后**：每一行代表一首歌，包含歌曲名称和可选的别称。

### 示例模板
| Phigros by 空游  | 歌曲名称        | 别称1    | 别称2   | 更多别称 |
|-----|-----------------|---------|---------|----------|
| 1   | Cthugha         | 克图格亚 | 火神    |          |
| 2   | Palescreen      | 白屏     | 歌剧院  |          |

## 如何修改模板
1. **保持模板结构不变**：
   - 第一行除了A1，不作解析，仅为占位。A1前半标识题库范围，后半标识作者
   - 从第二行开始，每一行必须包含歌曲名称，别称为可选项。

2. **新增歌曲**：
   - 在模板中新增一行，填写：
     - **歌曲名称**（必填）。
     - **别称**（从第三列开始，可选，支持多个）。

3. **删除歌曲**：
   - 删除对应行即可。

4. **修改歌曲信息**：
   - 修改对应行的歌曲名称或别称。

## 注意事项
- 歌曲名称（第二列）为必填字段，不能为空。
- 别称字段可选，支持留空。
- 文件格式必须是 `.xlsx`，其他格式无法识别。
