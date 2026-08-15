# legado-tts-rules

阅读（Legado）App「替换净化」TTS 朗读规则集，网络导入 JSON（根为数组）。

| 文件 | 说明 |
|------|------|
| `tts-segment.json` | 长句/段落分段：`\n` 触发逐句 TTS 请求（保守/激进两档，默认激进） |
| `tts-multirole.json` | 净化 + 分段 + 拟声词同音替换：标点规范化 11 条、净化 5 条、长句/段落拆分 2 条、拟声词防破音同音替换 3 条（嗯→恩 / 嘻→希 / 咳→可，先例：Index-TTS#47、Legado#474） |

## 网络导入

Legado → 我的 → 替换净化 → 菜单 → 网络导入，粘贴 URL：

- **tts-multirole.json** raw：https://raw.githubusercontent.com/mike2023-5-31/legado-tts-rules/main/tts-multirole.json
- **tts-multirole.json** jsDelivr：https://cdn.jsdelivr.net/gh/mike2023-5-31/legado-tts-rules@main/tts-multirole.json
- **tts-segment.json** raw：https://raw.githubusercontent.com/mike2023-5-31/legado-tts-rules/main/tts-segment.json
- **tts-segment.json** jsDelivr：https://cdn.jsdelivr.net/gh/mike2023-5-31/legado-tts-rules@main/tts-segment.json

> tts-multirole.json 不含叠音词组/数字标题/慎选标记组；拟声词替换仅针对已知引起破音/杂音的语气词（嗯/嘻/咳），并保护 嘻哈、笑嘻嘻、咳嗽、咳血 等常用词。
