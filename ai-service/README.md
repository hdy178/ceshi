# AI Service

负责将结构化人生状态转换为叙事文本。

当前版本先提供：

- `/health` 健康检查
- `/narrate` 根据凡人 / 修仙模式生成剧情
- `/epitaph` 为死亡人生生成墓志铭

默认使用 SiliconFlow 的 OpenAI 兼容接口：

```powershell
$env:SILICONFLOW_API_KEY="你的 SiliconFlow Key"
$env:SILICONFLOW_BASE_URL="https://api.siliconflow.cn/v1"
$env:SILICONFLOW_MODEL="Pro/zai-org/GLM-4.7"

python -m uvicorn app.main:app --host 127.0.0.1 --port 8000
```

没有配置 `SILICONFLOW_API_KEY` 时，会使用本地兜底叙事。
