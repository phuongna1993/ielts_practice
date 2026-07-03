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

## 1. Bảng so sánh từng câu

> 🔴 ~~gạch ngang~~ = chỗ chép sai · ✅ **in đậm** = từ đúng

| Câu | Đáp án (chuẩn) | Bạn chép | Sửa lỗi |
|---|---|---|---|
| **1** (B/M) | …câu đáp án, **bôi đậm** chỗ quan trọng… | …bản chép, ~~gạch ngang~~ chỗ sai… | ~~từ sai~~→**từ đúng** /IPA/ 🔴nhóm lỗi |
| **2** (G/W) | … | … | … |

(lặp lại cho từng câu; câu nào đúng/gần đúng thì khen ✅)
(Với lỗi **nghe nhầm** và **connected speech**, luôn kèm phiên âm IPA của từ/cụm đúng, đánh dấu 🔴 để người học biết đây là lỗi nghe cần ưu tiên luyện.)

---

## 2. Bảng chi tiết từng lỗi

Tách **mỗi lỗi thành một dòng** để người học dễ tra cứu và luyện lại.

| Câu | Từ bạn chép (sai) | Từ đúng | Phiên âm IPA | Nhóm lỗi | Giải thích ngắn |
|---|---|---|---|---|---|
| 1 | từ sai | từ đúng | /.../ | 🔴 Nghe nhầm / Ngữ pháp / Mạo từ / Chính tả / 🟡 Từ vựng | giải thích 1 dòng |

**Chú thích màu:** 🔴 = lỗi nghe (nghe nhầm/nối âm – ưu tiên luyện) · 🟡 = từ vựng chưa biết · còn lại = ngữ pháp/mạo từ/chính tả.

📊 Kết bằng **một dòng thống kê**: tổng số lỗi, số lỗi nghe 🔴 và nhóm cần ưu tiên luyện.

---

## 3. Tổng hợp các nhóm lỗi cần khắc phục

1. **<Nhóm lỗi lặp nhiều nhất>** — liệt kê các câu mắc phải.
2. **Ngữ pháp & hòa hợp chủ–vị** — ...
3. **Mạo từ** — ...
4. **Chính tả** — ...
5. **Connected speech (nối âm) cần luyện lại** — trích các cụm khó.

## 4. Bảng từ vựng mới (chi tiết)

Mỗi từ kèm **từ loại, IPA, nghĩa, đồng nghĩa/liên quan, cụm đi kèm (collocations) và 1 ví dụ**.

| Từ | Từ loại | Phiên âm | Nghĩa | Đồng nghĩa / Liên quan | Cụm đi kèm | Ví dụ |
|---|---|---|---|---|---|---|
| binoculars | n. (số nhiều) | /bɪˈnɒkjələz/ | ống nhòm | field glasses; *cf.* telescope | *a pair of binoculars* | *She used **binoculars** to watch the birds.* |

Sau bảng, thêm **💡 Word cluster**: gom các từ cùng chủ đề bài nghe thành một sơ đồ ngắn để người học dễ nhớ và dễ đoán âm lần sau.

## 5. Lời khuyên

<3–4 lời khuyên cụ thể, gắn với lỗi thực tế trong bài. Khen phần làm tốt để tạo động lực.>

---

## 6. Bản dịch tiếng Việt (theo đáp án chuẩn)

<Dịch toàn bộ transcript chuẩn sang tiếng Việt, giữ nhãn người nói (M/W hoặc B/G).>

---

## 7. Đáp án chuẩn (highlight chỗ bạn sai)

> **Chú thích:** 🔴 **chữ tô đậm** + 🔴 = chỗ bạn chép sai · ~~(từ bạn đã chép)~~ đặt ngay sau · ⬜ **[bỏ sót]** = chỗ thiếu · ✅ = câu/cụm chép đúng.

<Viết lại TOÀN BỘ transcript chuẩn theo dòng, giữ nhãn người nói. Ngay tại mỗi chỗ sai, đặt từ đúng dạng 🔴**từ đúng**🔴 rồi kèm ngay sau ~~(từ bạn đã chép)~~. Chỗ thiếu đánh dấu ⬜**[bỏ sót]**. Câu/cụm chép đúng đánh dấu ✅ ở cuối câu.>

> <Một dòng tổng kết cuối: chỉ ra nhóm từ vấp nhiều nhất và khen phần làm tốt.>
```

Khi người dùng yêu cầu "lưu lại", xuất bản hoàn chỉnh (đủ 7 phần) ra file `unit_<n>_result.md` trong thư mục skill này.

## Nguyên tắc chấm điểm (thang 10)

- Bắt đầu từ 10, trừ điểm theo mức độ ảnh hưởng đến nghĩa:
  - Lỗi làm **sai nghĩa cả cụm/câu** (nghe nhầm nặng, mất mệnh đề): trừ nhiều.
  - Lỗi **ngữ pháp/mạo từ/chính tả** không đổi nghĩa: trừ ít.
- Nắm được **bố cục và ý chính** vẫn được ghi nhận điểm nền.
- Tham chiếu cách chấm và độ chi tiết ở bài mẫu: [unit_4_result.md](unit_4_result.md).

## Ghi chú

- Toàn bộ phần nhận xét, lời khuyên viết bằng **tiếng Việt**; giữ nguyên tiếng Anh ở phần trích dẫn từ/câu.
- Giọng văn khích lệ, chỉ ra điểm mạnh trước khi nêu điểm cần cải thiện.
- **Phiên âm IPA** dùng chuẩn Anh-Anh (RP), đặt giữa hai dấu gạch chéo `/.../`. Bắt buộc có ở: (1) cột "Phiên âm" của bảng từ vựng, (2) các từ/cụm bị nghe nhầm hoặc nối âm trong phần so sánh và bảng chi tiết lỗi. Có thể kèm phiên âm phần còn lại nếu giúp người học.
- **Định dạng bảng:** phần so sánh từng câu và phần lỗi đều trình bày dạng **bảng**. Trong bảng dùng `~~gạch ngang~~` cho chỗ chép sai và **in đậm** cho từ đúng để dễ nhìn.
