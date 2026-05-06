### 3.1 Workshop 1 — Chấm RICE

**Output:** Bảng RICE 5 dòng + 2x2 Value-Effort Matrix.

---

# RICE Matrix

| Feature | Reach | Impact | Confidence | Effort (PM) | Score |
|---|---:|---:|---:|---:|---:|
| Challenge mode (AI opponent) | 500 | 3 | 0.5 | 3 | 250 |
| Coach feedback theo từng luận điểm | 400 | 2 | 0.5 | 2 | 200 |
| Opponent difficulty control | 250 | 1 | 0.5 | 1.5 | 83 |
| Argument rewrite suggestion | 300 | 2 | 0.8 | 1.5 | 320 |
| Full debate format (timer / role / speech order) | 150 | 0.5 | 0.5 | 4 | 9.4 |

---

# 2x2 Value-Effort Matrix

```text
              Effort
            Low              High
          ┌────────────────┬────────────────────┐
     High │ Quick Wins    │ Strategic Bets     │
          │               │                    │
          │ Argument      │ Challenge Mode     │
          │ Rewrite       │ (AI Opponent)      │
   Value  │ Suggestion    │                    │
          ├────────────────┼────────────────────┤
     Low  │ Fill-ins      │ Non-starters       │
          │               │                    │
          │ Opponent      │ Full Debate        │
          │ Difficulty    │ Format             │
          │ Control       │                    │
          └────────────────┴────────────────────┘
```

---

# Priority Analysis

| Quadrant | Feature | Reason |
|---|---|---|
| Quick Wins | Argument Rewrite Suggestion | Outcome measurable rõ, effort thấp, giúp validate learning loop nhanh |
| Strategic Bets | Challenge Mode (AI Opponent) | Core moat của sản phẩm, difficult to replicate, tạo long-term differentiation |
| Fill-ins | Opponent Difficulty Control | Improve UX nhưng chưa directly solve PMF risk |
| Non-starters | Full Debate Format | Complexity cao nhưng chưa giúp validate core value |

