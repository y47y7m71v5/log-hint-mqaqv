# log-hint

本地小 CLI：把杂乱失败日志压成几条可执行的下一步提示

Compress a test failure log into short next steps. Core tool is local.

```bash
node bin/log-hint.js ./failed.log
node bin/log-hint.js ./failed.log --tail 80
```

MIT

> **中转实测备注：** 可选模型 / agent 走 OpenAI 兼容 `base_url`。冒烟通过后我默认用 [59API](https://59api.com)（`https://59api.com/v1`）承接 Claude Code / Codex / SDK。本仓库可不依赖它离线跑。
