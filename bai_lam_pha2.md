# BÀI LÀM PHA 2 (ĐỀ LUYỆN TẬP CHỦ ĐỀ TÀI CHÍNH CÁ NHÂN)

- **Họ tên:** Nguyễn Vũ Long
- **Lớp:** HN-KS26-CNTT3
- **Link repository Pha2:** [GitHub](https://github.com/vulong1712/HN-KS26-CNTT3-Nguyen_Vu_Long-SS8-BAITHI)
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** Gemini

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đăng ký hội thảo ra JSON

**KET QUA AI**

```text
[
  {
    "ma_goi": "DT",
    "ngay_hoi_thao": "2026-12-20",
    "nguoi_lon": 2,
    "tre_em": 1,
    "hang_ve": "thuong",
    "ghi_chu": null
  },
  {
    "ma_goi": "CB",
    "ngay_hoi_thao": "2027-01-10",
    "nguoi_lon": 3,
    "tre_em": 0,
    "hang_ve": "thuong",
    "ghi_chu": "một người dùng xe lăn cần lối đi riêng"
  },
  {
    "ma_goi": "VIP",
    "ngay_hoi_thao": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "hang_ve": "vip",
    "ghi_chu": "một anh mắt kém cần ngồi bàn đầu gần màn hình chiếu"
  }
]
```

**Link trò chuyện:** <https://share.gemini.google/gwYeF7kZaeml>

## 4.3. Báo giá vé hội thảo bằng Chain-of-Thought

**KET QUA AI**

```text
<bang_gia_ve>
BẢNG GIÁ VÉ HỘI THẢO TÀI CHÍNH (đồng/người lớn)
CB – Gói Cơ Bản: 1.000.000
DT – Gói Đầu Tư: 1.500.000
VIP – Gói VIP: 3.000.000
</bang_gia_ve>

<quy_tac_tinh_gia>
QUY TẮC TÍNH GIÁ

1. Trẻ em từ 6 đến 12 tuổi (tham gia lớp "Bé tập quản lý tiền") tính 50% giá người lớn. Trẻ dưới 6 tuổi miễn phí.
2. Nhóm từ 4 người lớn trở lên được giảm 10% trên tiền vé (tiền người lớn + tiền trẻ em).
3. Phụ thu bộ sổ tay lập kế hoạch tài chính cá nhân: 200.000 đồng/bộ. Phụ thu không được giảm giá.
4. Tổng tiền = tiền vé sau giảm + phụ thu.
</quy_tac_tinh_gia>

<yeu_cau_bao_gia>
YÊU CẦU BÁO GIÁ
Nhóm đồng nghiệp đăng ký đi học buổi hội thảo cuối tuần, chọn gói DT (Gói Đầu Tư), gồm 4 người lớn, 2 trẻ em (8 tuổi và 11 tuổi) và 1 bé 4 tuổi. Nhóm đặt mua thêm 2 bộ sổ tay lập kế hoạch tài chính cá nhân.
</yeu_cau_bao_gia>

**Tính toán chi tiết từng bước:**

1. **Tiền người lớn:**
Nhóm chọn gói DT có đơn giá 1.500.000 đồng/người lớn cho 4 người lớn.
Phép tính: $4 \times 1.500.000 = 6.000.000\text{ đồng}$
2. **Tiền trẻ em:**
Có 2 trẻ em (8 tuổi và 11 tuổi) thuộc diện từ 6 đến 12 tuổi nên tính 50% giá vé người lớn ($1.500.000 \times 50\% = 750.000\text{ đồng/trẻ}$), và 1 bé 4 tuổi (dưới 6 tuổi) được miễn phí ($0\text{ đồng}$).
Phép tính: $(2 \times 1.500.000 \times 50\%) + (1 \times 0) = 1.500.000\text{ đồng}$
3. **Tiền vé:**
Tổng tiền vé trước khi áp dụng giảm giá bằng tiền người lớn cộng tiền trẻ em.
Phép tính: $6.000.000 + 1.500.000 = 7.500.000\text{ đồng}$
4. **Giảm giá nhóm:**
Nhóm có 4 người lớn nên đủ điều kiện giảm 10% trên tổng tiền vé.
Phép tính: $7.500.000 \times 10\% = 750.000\text{ đồng}$
5. **Phụ thu sổ tay:**
Nhóm đặt thêm 2 bộ sổ tay với giá 200.000 đồng/bộ (không áp dụng giảm giá).
Phép tính: $2 \times 200.000 = 400.000\text{ đồng}$
6. **Tổng tiền:**
Tổng số tiền khách hàng cần thanh toán bằng tiền vé sau giảm giá cộng với phụ thu sổ tay.
Phép tính: $(7.500.000 - 750.000) + 400.000 = 6.750.000 + 400.000 = 7.150.000\text{ đồng}$

[RESULT: 7.150.000 đồng]
```

**Link trò chuyện:** <https://share.gemini.google/c202JoWyRNGu>

### b) Kiểm tra kết quả AI

Kết luận: AI tính ĐÚNG hoàn toàn các bước và kết quả cuối cùng [RESULT: 7.150.000 đồng]

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
"loai_su_co": "sai_khu_vuc",
"so_khach": 2,
"so_hiep_bi_anh_huong": 2,
"tom_tat": "Khách hàng gói DT bị xếp ngồi ghế phụ không có bàn viết trong 2 phiên học đầu."
}
```

**Link trò chuyện:** <https://share.gemini.google/D13YmZdwuWbH>

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

| Tiêu chí | Điểm | Minh chứng | Đề xuất sửa |
| --- | --- | --- | --- |
| **Đúng thông tin (50%)** | 5.0/5.0 | Nhân viên đã cung cấp đầy đủ số liệu cụ thể cho cả hai hạng mục theo yêu cầu: giá vé (*"1.200.000đ/người"*) và chính sách hủy vé (*"báo huỷ trước 4 ngày thì bên em hoàn lại đủ 100% tiền vé"*). *(Lưu ý: Điểm tối đa được ghi nhận với điều kiện các con số này trùng khớp với dữ liệu gốc của Ban tổ chức).* | Không có lỗi về số liệu (giữ nguyên thông tin giá vé và thời hạn hoàn hủy nếu đúng quy định hiện hành). |
| **Đầy đủ (30%)** | 1.5/3.0 | **Đạt:** Trả lời đủ 2 câu hỏi về giá và chính sách hủy.<br>

<br>**Lỗi thiếu thông tin:**<br>

<br>- **Câu bị lỗi:** *"Anh/chị báo huỷ trước 4 ngày thì bên em hoàn lại đủ 100% tiền vé nha, cứ yên tâm chốt đơn đi ạ!"*<br>

<br>- **Lý do sai:** Kết thúc câu trả lời nhưng bỏ sót bước khai thác thông tin cần thiết từ khách hàng (không mời khách cung cấp **ngày hội thảo** và **số lượng vé** muốn đăng ký). | Bổ sung lời mời cung cấp thông tin ở cuối tin nhắn:<br>

<br>*"Để bên em hỗ trợ giữ chỗ chính xác, anh/chị vui lòng cho em xin thông tin về ngày tham dự hội thảo và số lượng vé mình muốn đăng ký nhé ạ."* |
| **Giọng điệu (20%)** | 0.5/2.0 | **Lỗi 1 (Ngôn từ suồng sã):**<br>

<br>- **Câu bị lỗi:** *"Dạ chào anh/chị nha!"*, *"Vé gói Đầu Tư bên em giá chỉ 1.200.000đ/người thôi"*, *"cứ yên tâm chốt đơn đi ạ!"*<br>

<br>- **Lý do sai:** Dùng các từ ngữ thiếu tính trang trọng trong tư vấn dịch vụ tài chính/giáo dục (*"nha"*, *"thôi"*, *"chốt đơn"*).<br>

<br>

<br>**Lỗi 2 (Hứa hẹn lợi nhuận quá đà):**<br>

<br>- **Câu bị lỗi:** *"...đi học về đầu tư chứng khoán lời khủng luôn ạ."*<br>

<br>- **Lý do sai:** Cam kết lợi nhuận phi thực tế (*"lời khủng luôn"*), vi phạm nghiêm trọng chuẩn mực tư vấn đầu tư và dễ gây khiếu nại về sau. | - **Sửa câu chào & báo giá:** *"Dạ em chào anh/chị. Hiện tại vé gói Đầu Tư bên em có mức giá là 1.200.000đ/người ạ."*<br>

<br>- **Sửa nội dung khóa học:** *"Chương trình sẽ cung cấp kiến thức và phương pháp đầu tư chứng khoán bài bản giúp anh/chị tối ưu hiệu quả giao dịch."*<br>

<br>- **Sửa câu trấn an:** *"Trường hợp anh/chị báo hủy trước 4 ngày diễn ra sự kiện, bên em sẽ hoàn lại 100% chi phí vé nên anh/chị hoàn toàn có thể yên tâm đăng ký ạ."* |
| **Tổng điểm** | **7.0/10** | **Nhận xét chung:** Nhân viên nắm được thông tin cơ bản nhưng thiếu kỹ năng điều hướng hội thoại (quên hỏi ngày và số lượng vé), đồng thời mắc lỗi nghiêm trọng về giọng điệu (suồng sã và thổi phồng cam kết lợi nhuận). | Yêu cầu nhân viên điều chỉnh lại mẫu phản hồi theo toàn bộ phần đề xuất sửa nêu trên trước khi gửi khách hàng. |

**Link trò chuyện:** <https://share.gemini.google/tbwTWSo2bbcH>
