# G9.1 Mindmap — 3 lỗi AI + cách nộp

## File cần nộp / đưa vào report

| File | Vai trò |
| --- | --- |
| `qa_qc_mindmap_AI_draft.md` (+ `.png` nếu có) | Output AI (sai) |
| `qa_qc_mindmap_corrected.md` (+ `.png` nếu có) | Bản bạn sửa |
| `AI-02` Artifact A1 | Đã điền sẵn |

## 3 mistakes (copy vào báo cáo)

1. **ISTQB Advanced bắt buộc cho mọi Manual QA** → Sai. Thực tế: Foundation / kinh nghiệm là phổ biến; Advanced tùy lộ trình.
2. **Software không có QC; chỉ Selenium; chỉ Waterfall 2026** → Sai. Vẫn có QC/release gate; nhiều tool (Playwright, Cypress…); Agile/DevOps phổ biến.
3. **Không cần exploratory; AI role = copy-paste prompt** → Sai. Exploratory vẫn quan trọng; AI-augmented QA gồm review output, LLM eval, agentic testing.

## Export PNG (nếu Moodle thích ảnh)

1. Mở https://mermaid.live  
2. Dán nội dung file `.mmd`  
3. Actions → PNG → lưu:
   - `qa_qc_mindmap_AI_draft.png`
   - `qa_qc_mindmap_corrected.png`

Hoặc dùng CLI (đã có trong project nếu chạy được):

```bash
npx @mermaid-js/mermaid-cli -i mindmap/qa_qc_mindmap_AI_draft.mmd -o mindmap/qa_qc_mindmap_AI_draft.png
npx @mermaid-js/mermaid-cli -i mindmap/qa_qc_mindmap_corrected.mmd -o mindmap/qa_qc_mindmap_corrected.png
```
