# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 08
- **Họ tên:** Mai Việt Dũng
- **Lớp:** CNTT1
- **Link repository Pha2:**https://github.com/maivietdung45-create/HN-KS26-CNTT1_PromptAI_H02_Pha1-Pha2
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** ChatGPT

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt lịch khám ra JSON

**KET QUA AI**

```text
[\
&#x20; {\
&#x20;   "ma_dich_vu": "TRAMRANG",\
&#x20;   "ngay_hen": "2026-12-17",\
&#x20;   "nguoi_lon": 2,\
&#x20;   "tre_em": 1,\
&#x20;   "khung_gio": "chieu",\
&#x20;   "ghi_chu": null\
&#x20; },\
&#x20; {\
&#x20;   "ma_dich_vu": "CAOVOI",\
&#x20;   "ngay_hen": "2027-01-06",\
&#x20;   "nguoi_lon": 3,\
&#x20;   "tre_em": 0,\
&#x20;   "khung_gio": null,\
&#x20;   "ghi_chu": "Một người bị tiểu đường"\
&#x20; },\
&#x20; {\
&#x20;   "ma_dich_vu": "TAYTRANG",\
&#x20;   "ngay_hen": null,\
&#x20;   "nguoi_lon": 4,\
&#x20;   "tre_em": 0,\
&#x20;   "khung_gio": "sang",\
&#x20;   "ghi_chu": "Một người dị ứng thuốc tê"\
&#x20; }\
]
```

**Link trò chuyện:** https://chatgpt.com/share/6b07e546-3314-83ec-a06e-c501a5547d17

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
**1. Tiền người lớn:**

6 × 350.000 = **2.100.000 đồng**

**2. Tiền trẻ em:**

- Trẻ 7 tuổi: 350.000 × 80% = 280.000 đồng.
- Trẻ 11 tuổi: 350.000 × 80% = 280.000 đồng.
- Trẻ 4 tuổi: Miễn phí = 0 đồng.

Tổng tiền trẻ em: 280.000 + 280.000 + 0 = **560.000 đồng**

**3. Tiền dịch vụ:**

2.100.000 + 560.000 = **2.660.000 đồng**

**4. Giảm giá nhóm:**

Nhóm có 6 người lớn (từ 5 người lớn trở lên), được giảm 10%.

2.660.000 × 10% = 266.000 đồng.

Tiền dịch vụ sau giảm:

2.660.000 - 266.000 = **2.394.000 đồng**

**5. Phí chụp X-quang:**

3 × 150.000 = **450.000 đồng**

**6. Tổng tiền:**

2.394.000 + 450.000 = **2.844.000 đồng**

[RESULT: 2.844.000 đồng]
```

**Link trò chuyện:** https://chatgpt.com/share/6b07e5e8-a598-83ec-b657-709abe819c7c

### b) Kiểm tra kết quả AI

Đúng

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{"loai_su_co":"tre_hen","so_khach":3,"so_lan_hen_bi_tre":2,"tom_tat":"Gia đình 3 người phải chờ hơn 1 tiếng trong cả 2 lần hẹn; không phàn nàn về bác sĩ Nam."}
```

**Link trò chuyện:** https://chatgpt.com/share/6b07e64f-c650-83ec-90a2-266352f5894b

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
| Tiêu chí             | Điểm     | Minh chứng                                                                                                        | Đề xuất sửa                                                                             |
| -------------------- | -------- | ----------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| Đúng thông tin (50%) | 1/5      | Giá 450.000 đồng/răng sai (giá chuẩn 500.000 đồng/răng). Chính sách miễn phí sau 8 tháng sai (chỉ được giảm 50%). | Sửa giá thành 500.000 đồng/răng. Bong sau 8 tháng được hỗ trợ làm lại với mức giảm 50%. |
| Đầy đủ (30%)         | 1/3      | Đã trả lời cả hai câu hỏi nhưng chưa mời khách cung cấp ngày hẹn và khung giờ để đặt lịch.                        | Bổ sung lời mời khách cung cấp ngày hẹn và khung giờ mong muốn.                         |
| Giọng điệu (20%)     | 1/2      | Có lời nói lịch sự nhưng dùng từ suồng sã như "free", "nha", "inbox".                                             | Sử dụng cách diễn đạt chuyên nghiệp, lịch sự hơn.                                       |
| **Tổng điểm**        | **3/10** |                                                                                                                   |                                                                                         |
```

**Link trò chuyện:** https://chatgpt.com/share/6b07e69f-73f0-83ec-a187-5ebe30a404d8
