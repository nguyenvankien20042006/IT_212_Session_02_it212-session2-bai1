## Đáp án: Phương án C

### 1. Vì sao phương án C là tối ưu nhất?

Phương án C là lựa chọn tối ưu nhất vì sử dụng đúng công cụ cho từng loại công việc, tận dụng tối đa khả năng xử lý ngữ cảnh (Context Window) của AI và giảm thiểu việc chuyển đổi ngữ cảnh (Context Switching) trong quá trình phát triển phần mềm.

#### a. Viết tài liệu hướng dẫn API bằng Web Chat

Web Chat (ChatGPT, Claude, Gemini...) có thế mạnh trong việc:

- Phân tích yêu cầu nghiệp vụ.
- Soạn thảo tài liệu kỹ thuật.
- Tạo nội dung Markdown có cấu trúc rõ ràng.

Đối với tài liệu API Guide, AI không cần truy cập toàn bộ mã nguồn dự án mà chủ yếu cần hiểu yêu cầu nghiệp vụ và cách sử dụng API. Vì vậy Web Chat là công cụ phù hợp nhất cho nhiệm vụ này.

#### b. Refactor lớp Book bằng Agentic/Repository-wide Assistant

Việc tái cấu trúc lớp `Book` liên quan đến nhiều tệp:

- `Book.java`
- `BookService.java`
- `BookController.java`
- `BookRepository.java`

Các tệp này có mối liên hệ chặt chẽ với nhau. Trợ lý lập trình cấp cao (Agentic Assistant) có khả năng:

- Phân tích toàn bộ repository.
- Hiểu mối quan hệ giữa các thành phần trong dự án.
- Tự động cập nhật đồng bộ các thay đổi trên nhiều tệp.
- Giảm nguy cơ bỏ sót hoặc tạo lỗi không tương thích.

Điều này giúp tận dụng tối đa ngữ cảnh của toàn bộ dự án và nâng cao độ chính xác khi refactor.

#### c. Sửa lỗi cú pháp bằng Inline Code Assistant

Các lỗi như:

- Thiếu dấu chấm phẩy `;`
- Sai kiểu dữ liệu
- Lỗi cú pháp đơn giản

chỉ cần xem vài dòng mã xung quanh là có thể xử lý được.

Inline Code Assistant hoạt động trực tiếp trong IDE nên:

- Phản hồi nhanh.
- Không cần rời khỏi môi trường lập trình.
- Không cần sao chép mã nguồn sang công cụ khác.

Đây là lựa chọn hiệu quả nhất cho các lỗi nhỏ.

---

### 2. Tối ưu về Context Window và Context Switching

#### Tối ưu Context Window

Mỗi công cụ được giao đúng nhiệm vụ phù hợp với phạm vi ngữ cảnh cần xử lý:

| Tác vụ          | Phạm vi ngữ cảnh cần thiết           | Công cụ phù hợp   |
| --------------- | ------------------------------------ | ----------------- |
| Viết API Guide  | Yêu cầu nghiệp vụ và mô tả API       | Web Chat          |
| Refactor Book   | Toàn bộ dự án và nhiều tệp liên quan | Agentic Assistant |
| Sửa lỗi cú pháp | Một vài dòng mã nguồn                | Inline Assistant  |

Nhờ đó AI luôn được cung cấp đúng lượng thông tin cần thiết để đưa ra kết quả chính xác.

#### Giảm Context Switching

Phương án C giúp giảm đáng kể việc:

- Chuyển đổi giữa nhiều cửa sổ làm việc.
- Sao chép mã nguồn qua lại.
- Cung cấp lại ngữ cảnh cho AI nhiều lần.

Kết quả là:

- Tăng năng suất làm việc.
- Giảm sai sót.
- Duy trì luồng tư duy của lập trình viên.

---

### 3. Nhược điểm của phương án A

#### Sử dụng Web Chat cho cả 3 tác vụ

**Hạn chế:**

1. Phải liên tục sao chép mã nguồn giữa IDE và trình duyệt.
2. Gây nhiều Context Switching làm giảm hiệu suất làm việc.
3. AI khó nắm được toàn bộ cấu trúc dự án khi refactor nhiều tệp.
4. Dễ bỏ sót các thay đổi liên quan giữa các file.
5. Không hiệu quả cho các lỗi cú pháp nhỏ vì thao tác quá nhiều.

=> Phương án A làm giảm năng suất và tăng nguy cơ sai sót.

---

### 4. Nhược điểm của phương án B

#### Sử dụng Inline Code Assistant cho cả 3 tác vụ

**Hạn chế:**

1. Không mạnh trong việc soạn thảo tài liệu dài và có cấu trúc như API Guide.
2. Khả năng quan sát toàn bộ repository thường hạn chế hơn Agentic Assistant.
3. Việc refactor trên nhiều tệp phụ thuộc lẫn nhau có thể không đầy đủ hoặc thiếu đồng bộ.
4. Không tận dụng được thế mạnh chuyên biệt của từng loại công cụ AI.

=> Phương án B phù hợp cho hỗ trợ viết mã và sửa lỗi nhanh nhưng chưa tối ưu cho tài liệu kỹ thuật và refactor quy mô lớn.

---

## Kết luận

Phương án **C** là lựa chọn tối ưu nhất vì sử dụng đúng công cụ cho đúng nhiệm vụ:

- **Web Chat** để soạn thảo tài liệu API.
- **Agentic/Repository-wide Assistant** để refactor đồng bộ nhiều tệp trong dự án.
- **Inline Code Assistant** để sửa lỗi cú pháp nhanh chóng.

Cách tiếp cận này tận dụng hiệu quả phạm vi ngữ cảnh của từng công cụ, giảm thiểu Context Switching và mang lại năng suất lập trình cao nhất.
