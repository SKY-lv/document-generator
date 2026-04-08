# Document Generator Agent Skill

> AI-powered document generation and templating

## 功能

- **合同生成** - 销售/雇佣/NDA合同模板
- **报告生成** - 周报/月报/项目报告
- **提案撰写** - 商业提案、项目计划
- **文档转换** - Markdown/Word/PDF互转
- **模板管理** - 自定义模板库

## 使用场景

```
用户: 帮我生成一份NDA合同
Agent: [调用document-generator skill生成NDA模板]
```

## 工具函数

### `generate_document(type, params)`

生成文档。

```python
{
    "type": "nda",
    "params": {
        "party_a": "甲方公司",
        "party_b": "乙方公司",
        "effective_date": "2026-04-08",
        "duration": "2 years"
    },
    "format": "docx"
}
```

### `from_template(template_id, data)`

模板填充。

### `convert_document(file, target_format)`

格式转换。

## 配置

```json
{
    "templates_dir": "./templates",
    "output_dir": "./output",
    "formats": ["docx", "pdf", "md"]
}
```

## 安装

```bash
clawhub install SKY-lv/document-generator
```

## License

MIT
