# 华南区｜营运四表完成情况看板

营运工作台内的独立 GitHub Pages 数据看板模块，视觉与交互参照现有品控稽核看板。

公开地址：`https://alan0715.github.io/ama-operations-workbench/operation-form-dashboard/`

## 数据顺序

区域 → 城市 → 门店。区域是首要分组与排序维度。

## 更新流程

1. 写入 `data/form-data.json`。
2. 执行 `node update-data.mjs` 生成浏览器数据文件。
3. 执行 `python3 publish_github_pages.py` 发布。
4. 执行 `python3 verify_github_pages.py` 验证公网与本地一致。
