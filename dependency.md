### 3.4 Workshop 4 — Dependency Map 

---

# Dependency Map

| Dependency | Tier | Worst-case Scenario | Plan B | Cost |
|---|---|---|---|---|
| OpenAI API | 🔴 Tier 1 | OpenAI siết rate limit hoặc tăng giá mạnh khiến Challenge mode unusable | LLM abstraction layer để switch sang Claude/Gemini + caching common prompts | 2-3 tuần dev + testing |
| Debate Quality | 🟡 Tier 2 | AI rebuttal generic, feedback không actionable → user churn nhanh | Structured prompting + evaluation pipeline + transcript review workflow | 2 tuần setup + ongoing iteration |
| Cost Scaling | 🟡 Tier 2 | Inference cost tăng quá nhanh do multi-turn debate sessions | Hybrid model routing + token optimization + session limits | 1-2 tuần implementation |

---

# Critical Path

```text
Prompt Architecture
        ↓
LLM Integration
        ↓
Challenge Mode Stability
        ↓
Coach Feedback Quality
        ↓
Beta Testing
        ↓
Launch
```

---

# Non-critical Tasks

| Task | Lý do |
|---|---|
| UI polish | Không block PMF |
| Animation / effects | Có thể làm sau |
| Dashboard improvements | Không ảnh hưởng core AI loop |
| Full BP/WSD simulation | Không cần cho initial validation |

---

# Cascading Failure Analysis

| Scenario | Risk | Mitigation |
|---|---|---|
| OpenAI rate limit + token cost tăng cùng lúc | Challenge mode unusable, burn rate tăng mạnh | Switch provider + reduce response length + lightweight mode + session limits |
