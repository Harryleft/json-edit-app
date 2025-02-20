# JSONEditorApp

## 简介
`JSONEditorApp` 是一个基于 `tkinter` 的图形用户界面应用程序，用于查看和编辑专业课章节知识点的 JSON 文件。用户可以通过该应用程序添加、删除章节和知识点，并编辑知识点的详细信息。
里面有两个脚本：
- csv_to_json.py:支持用户通过外部CSV文件创建知识点，然后可通过本脚本将其转换为`json_edit_app`支持的JSON格式，示例格式如下：
```csv
章节,知识点,知识点详情
第一章,知识点1,知识点1的详细信息
第一章,知识点2,知识点2的详细信息
第二章,知识点1,知识点1的详细信息
第二章,知识点2,知识点2的详细信息
```
- json_edit.py：支持用户对JSON文件中的知识点进行增删改查功能，示例格式如下：
```json
{
    "第一章": {
        "知识点1": "知识点1的详细信息",
        "知识点2": "知识点2的详细信息"
    },
    "第二章": {
        "知识点1": "知识点1的详细信息",
        "知识点2": "知识点2的详细信息"
    }
}
```

## 功能
- 加载 JSON 文件
- 保存 JSON 文件
- 添加章节
- 删除章节
- 添加知识点
- 删除知识点
- 编辑知识点详情
- 自动保存知识点详情

## 安装
```bash
pip install -r requirements.txt
```

## 使用方法

### 运行应用程序
在终端中运行以下命令启动应用程序：
```bash
python json_edit.py
```

### 用户界面介绍
- **章节列表**：显示所有章节。用户可以选择、添加或删除章节。
- **知识点列表**：显示选定章节中的所有知识点。用户可以选择、添加或删除知识点。
- **知识点详情**：显示和编辑选定知识点的详细信息。

### 加载 JSON 文件
1. 点击“载入 JSON”按钮。
2. 选择要加载的 JSON 文件。

### 保存 JSON 文件
1. 点击“保存 JSON”按钮。
2. 选择保存文件的位置和文件名。

### 添加章节
1. 点击“添加章节”按钮。
2. 输入章节名称。

### 删除章节
1. 选择要删除的章节。
2. 点击“删除章节”按钮。
3. 确认删除操作。

### 添加知识点
1. 选择一个章节。
2. 点击“添加知识点”按钮。
3. 输入知识点名称和详细信息。

### 删除知识点
1. 选择要删除的知识点。
2. 点击“删除知识点”按钮。
3. 确认删除操作。

### 编辑知识点详情
1. 选择一个知识点。
2. 在“知识点详情”文本框中编辑详细信息。
3. 编辑内容会自动保存，或点击“保存知识点”按钮手动保存。
