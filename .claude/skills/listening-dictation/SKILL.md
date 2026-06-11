---
name: listening-dictation
description: Chấm bài luyện nghe chép chính tả (dictation) tiếng Anh. Dùng khi người dùng dán "đáp án bài nghe" (transcript chuẩn) và "nội dung tôi nghe được" (bản chép tay), yêu cầu so sánh, chấm điểm thang 10, tổng hợp lỗi, liệt kê từ vựng mới và đưa lời khuyên.
---

# Listening Dictation Check

Skill này chấm bài luyện nghe chép chính tả (dictation) tiếng Anh và xuất kết quả bằng **tiếng Việt** theo định dạng cố định.

## Đầu vào

Người dùng cung cấp 2 khối nội dung:

1. **Đáp án bài nghe** — transcript chuẩn (đúng).
2. **Nội dung tôi nghe được và chép lại** — bản người dùng tự chép khi nghe.

Nếu thiếu một trong hai khối, hãy hỏi lại trước khi chấm.

## Cách thực hiện

Đối chiếu **từng câu** giữa đáp án và bản chép. Với mỗi điểm khác biệt, phân loại lỗi vào một trong các nhóm:

- **Nghe nhầm từ/cụm** (mishearing) — nghe sai âm thành từ khác (vd: *cents* → *percent*, *new laws* → *news*).
- **Connected speech** — nối âm/nuốt âm khiến mất từ (vd: *Will I be able to* nghe như *Realize*).
- **Ngữ pháp** — thì, hòa hợp chủ–vị, số ít/nhiều (vd: *has* → *have*, *want* → *wants*).
- **Mạo từ** — thiếu/thừa *a/the*.
- **Chính tả** — viết sai chính tả (vd: *tomorow*, *enviroment*).
- **Từ vựng chuyên đề** — từ thuộc chủ đề bài nghe mà người dùng không nhận ra (vd: *binoculars*, *feathers*, *nest*).

## Định dạng output (bắt buộc theo thứ tự)

```
# <Tên bài> – Listening Dictation Check

## Điểm số: **X / 10**

<1–2 câu nhận xét tổng quan: nắm được ý chính nào, lỗi lặp lại nhiều nhất là gì>

---

## So sánh từng câu

### Câu 1
- **Đáp án:** *...*
- **Bạn chép:** ...
- **Lỗi:**
  - `từ sai` → **từ đúng** /phiên âm IPA/ (giải thích ngắn nhóm lỗi)
  - ...

(lặp lại cho từng câu; câu nào đúng/gần đúng thì khen ✅)
(Với lỗi **nghe nhầm** và **connected speech**, luôn kèm phiên âm IPA của từ/cụm đúng để người học biết phát âm chuẩn, vd: *binoculars* /bɪˈnɒkjələz/.)

---

## Tổng hợp các nhóm lỗi cần khắc phục

1. **<Nhóm lỗi lặp nhiều nhất>** — liệt kê các câu mắc phải.
2. **Ngữ pháp & hòa hợp chủ–vị** — ...
3. **Mạo từ** — ...
4. **Chính tả** — ...
5. **Connected speech (nối âm) cần luyện lại** — trích các cụm khó.

## Từ vựng mới (không nghe được)

| Từ | Phiên âm | Nghĩa | Ví dụ |
|---|---|---|---|
| binoculars | /bɪˈnɒkjələz/ | ống nhòm | *She used **binoculars** to watch the birds.* |

(mỗi từ kèm đúng 1 câu ví dụ)

## Lời khuyên

<3–4 lời khuyên cụ thể, gắn với lỗi thực tế trong bài. Khen phần làm tốt để tạo động lực.>

---

## Bản dịch tiếng Việt (theo đáp án chuẩn)

<Dịch toàn bộ transcript chuẩn sang tiếng Việt, giữ nhãn người nói (M/W hoặc B/G).>
```

## Nguyên tắc chấm điểm (thang 10)

- Bắt đầu từ 10, trừ điểm theo mức độ ảnh hưởng đến nghĩa:
  - Lỗi làm **sai nghĩa cả cụm/câu** (nghe nhầm nặng, mất mệnh đề): trừ nhiều.
  - Lỗi **ngữ pháp/mạo từ/chính tả** không đổi nghĩa: trừ ít.
- Nắm được **bố cục và ý chính** vẫn được ghi nhận điểm nền.
- Tham chiếu cách chấm và độ chi tiết ở các bài mẫu: [unit_2.md](unit_2.md), [unit_3.md](unit_3.md).

## Ghi chú

- Toàn bộ phần nhận xét, lời khuyên viết bằng **tiếng Việt**; giữ nguyên tiếng Anh ở phần trích dẫn từ/câu.
- Giọng văn khích lệ, chỉ ra điểm mạnh trước khi nêu điểm cần cải thiện.
- **Phiên âm IPA** dùng chuẩn Anh-Anh (RP), đặt giữa hai dấu gạch chéo `/.../`. Bắt buộc có ở: (1) cột "Phiên âm" của bảng từ vựng, (2) các từ/cụm bị nghe nhầm hoặc nối âm trong phần so sánh. Có thể kèm phiên âm phần còn lại nếu giúp người học.
