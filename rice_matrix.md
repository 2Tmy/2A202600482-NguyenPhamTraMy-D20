# Workshop 1 — RICE Matrix

## 1. Chọn 5 Core Features từ PRD

Dựa trên PRD Day 17:

1. Challenge mode (AI opponent debate)
2. Coach mode feedback theo từng luận điểm
3. Opponent difficulty control
4. Argument rewrite suggestion
5. Full debate format (timer / role / speech order)

---

## 2. RICE Matrix

| Feature | Reach (user/quý) | Impact | Confidence | Effort (PM) | RICE Score | Notes |
|---|---:|---:|---:|---:|---:|---|
| Challenge mode (AI opponent) | 500 | 3 | 0.5 | 3 | 250 | Core value proposition nhưng chưa validate retention |
| Coach feedback theo từng luận điểm | 400 | 2 | 0.5 | 2 | 200 | Strong learning value nhưng chưa biết user trust AI không |
| Opponent difficulty control | 250 | 1 | 0.5 | 1.5 | 83 | Improve engagement nhưng chưa critical |
| Argument rewrite suggestion | 300 | 2 | 0.8 | 1.5 | 320 | Closest tới measurable learning outcome |
| Full debate format (timer / role / speech order) | 150 | 0.5 | 0.5 | 4 | 9.4 | Nice-to-have, không validate core value |

---

## 3. Giải thích Logic Chấm Điểm

### 3.1 Challenge Mode (AI Opponent)
Reach = 500
- Không thể assume toàn bộ user sẽ dùng feature
- Theo handbook:
  > Chỉ khoảng 20–40% user dùng feature mới trong quý đầu
- Đã discount optimistic estimate xuống realistic adoption.

Impact = 3
- Đây là feature định nghĩa sản phẩm
- Nếu opponent không đủ “khó”, toàn bộ product mất value.

Confidence = 50%
- Chưa có pilot retention thật
- Handbook quy định:
  > Chưa test = 50% MAX

Effort = 3 PM
Bao gồm:
- multi-turn reasoning
- stance consistency
- rebuttal quality
- prompt iteration
- QA và fallback UX

---

### 3.2 Coach Feedback Theo Từng Luận Điểm
Impact = 2
- Tạo learning loop rõ ràng
- Nhưng chưa phải moat mạnh bằng Challenge mode.

Confidence = 50%
Open question trong submission:
> “User có tin AI coach không?”

=> chưa validate trust.

Effort = 2 PM
Bao gồm:
- feedback generation
- logic detection
- rewrite suggestion
- UX correction flow

---

### 3.3 Opponent Difficulty Control
Impact = 1
- Improve UX
- Nhưng không directly solve PMF risk.

Confidence = 50%
- Chưa biết user thực sự cần adjust độ khó nhiều đến mức nào.

Effort = 1.5 PM
- Chủ yếu là prompt orchestration và state control.

---

### 3.4 Argument Rewrite Suggestion

Impact = 2
- Giúp user cải thiện argument ngay sau feedback
- Tạo learning outcome measurable.

Confidence = 80%
- Product đã define metric:
  > % argument được rewrite sau feedback
- Learning loop khá rõ ràng
- Nhưng chưa có pilot data thật nên chưa thể 100%.

Effort = 1.5 PM
- Chủ yếu prompt refinement
- Ít infrastructure hơn Challenge mode.

---

### 3.5 Full Debate Format

(timer / role / speech order)

Impact = 0.5
- Nice-to-have
- Không giúp validate core PMF.

Confidence = 50%
- Chưa có evidence user cần full BP/WSD structure.

Effort = 4 PM
Bao gồm:
- timer system
- role management
- speech order
- state synchronization
- UX complexity

=> effort cao nhưng value thấp.

---

## 4. 2x2 Value–Effort Matrix

### Quick Win
> Argument Rewrite Suggestion

- High value
- Low effort
- Outcome measurable rõ
- Build learning loop nhanh

=> nên làm trước.

---

### Strategic Bet
> Challenge Mode (AI Opponent)

- High value
- High effort
- Nếu làm tốt sẽ tạo moat dài hạn
- Harder to copy hơn basic coach feedback

=> đầu tư dài hạn.

---

### Fill-in
> Opponent Difficulty Control

- UX improvement
- Không critical cho PMF
- Có thể làm sau khi core loop ổn định.

---

### Non-starter
> Full Debate Format

(timer / role / speech order)

- Complexity cao
- Không validate core value
- Dễ làm founder distracted bởi “feature sophistication”

=> nên bỏ khỏi milestone đầu.

---
## 5. Pass/Fail 

### Pass Signals

- Có feature Confidence < 80%
- Có Non-starter rõ ràng
- Effort realistic
- Có Quick Win + Strategic Bet

---