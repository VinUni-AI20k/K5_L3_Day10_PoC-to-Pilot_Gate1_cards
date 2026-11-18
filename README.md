# LAB 10 · Thẻ sự cố (S1–S8) · From PoC to Pilot (Gate 1)

Repo riêng tư. Lab Coach mời học viên vào repo này (quyền Read) ở phút phát thẻ. **Mỗi bàn chỉ lấy đúng thư mục thẻ của bàn mình** (số thẻ Lab Coach đã ghi cho bàn), không lấy thẻ của bàn khác.

## Lấy thẻ vào repo của bàn

Chạy ở thư mục gốc repo của bàn, nhánh `main`, đã commit hết. Thay `S1` bằng số thẻ của bàn (hai chỗ):

```bash
git fetch https://github.com/VinUni-AI20k/K5_L3_Day10_PoC-to-Pilot_Gate1_cards.git main && git checkout FETCH_HEAD -- incidents/S1 && git commit -m "Nhận thẻ S1"
```

Lệnh chỉ chép thư mục `incidents/S1/` (4 file: `card.md`, `card.json`, `tickets.jsonl`, `world_patch.json`) vào repo của bàn, không gộp lịch sử của repo này. Sau đó đọc `incidents/S1/card.md` rồi chạy `python3 -m lab10.grade --incident S1` (mốc prepared, câu 3.0).

Không sửa các file trong `incidents/`: chúng bị khoá bằng hash.

## Cấu trúc

```
incidents/S1/ … incidents/S8/   mỗi thư mục = một gói thẻ, đúng đường dẫn repo của bàn cần
```
