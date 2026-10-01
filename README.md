# AI-Agent-Team-Marketing
Dự án phát triển hệ thống **AI Agent** tự động hóa quy trình lên kế hoạch và sáng tạo nội dung cho các chiến dịch Marketing.
---

## Hướng dẫn triển khai & Khởi chạy (Deployment & Usage)

Để người nhận có thể cấu hình và chạy luồng công việc (flow) chính xác như phiên bản gốc, vui lòng thực hiện đầy đủ các bước hướng dẫn dưới đây:

### 1️  Nhập (Import) dự án vào CrewAI Studio
* **Bước 1:** Đăng nhập vào tài khoản [CrewAI Studio](https://crewai.com).
* **Bước 2:** Chọn tính năng **Import** và tải lên file `.zip` của flow. Hệ thống sẽ tự động đồng bộ toàn bộ cấu hình hệ thống bao gồm: *Agents, Crews và State*.

### 2️⃣ Cấu hình Tích hợp (Integrations)
Do các khóa bảo mật và quyền truy cập gắn liền với tài khoản cá nhân, người nhận bắt buộc phải tự kết nối thủ công các dịch vụ sau trong mục **Integrations / Connections**:

## | Dịch vụ tích hợp | Thành phần sử dụng | Mục đích |
| **Facebook (OAuth)** | `publish_and_analyze` | Cấp quyền đăng bài tự động lên Facebook Page. |
| **DALL-E / OpenAI** | `design_visuals` | Kích hoạt tác vụ tạo hình ảnh minh họa bằng AI. |

### 3️⃣ Cấu hình Mô hình ngôn ngữ (LLM Setup)
* Đảm bảo tài khoản Studio đã kết nối sẵn với các nhà cung cấp LLM mong muốn (OpenAI, Anthropic, v.v.).
* Nếu hệ thống đang sử dụng mô hình nội bộ của tổ chức, tài khoản của người nhận cần phải có quyền truy cập tương đương vào tổ chức đó.

### 4️⃣ Khởi chạy & Nhập tham số đầu vào (Kickoff Inputs)
Khi nhấn **Run**, hệ thống sẽ yêu cầu cung cấp đầy đủ các tham số cấu hình bắt buộc sau:

## | Tham số (Field) | Nội dung mô tả / Ví dụ |
| `brand_identity` | *"TechGenius — thương hiệu SaaS, tông giọng thân thiện..."* |
| `brand_pillars` | *"Education, Community, Product, Brand Story"* |
| `target_audience` | *"Founders, startup operators, từ 25-40 tuổi..."* |
| `core_goals` | *"Engagement, Brand Awareness"* |
| `target_period` | *"October 2026"* |

---

## ✅ Checklist kiểm tra nhanh trước khi bấm RUN 🚀
- Đã Import file `.zip` vào CrewAI Studio thành công.
- Đã kết nối tài khoản Facebook cá nhân qua OAuth.
- Đã cấu hình và kích hoạt OpenAI / LLM provider.
- Đã điền đầy đủ và chính xác các trường dữ liệu đầu vào (Kickoff Inputs).

**Prompt:**
<img width="688" height="634" alt="image" src="https://github.com/user-attachments/assets/a09a9d62-9430-46fa-aee2-25b5c7abee55" />

## Note:
* **Phạm vi dữ liệu:** Hiện tại hệ thống đang được cấu hình Prompt để chạy thử nghiệm dữ liệu trong giai đoạn ngắn từ ngày **01/10/2026 đến 05/10/2026**.
* **Kế hoạch cập nhật:** Một số luồng thông tin nghiệp vụ chưa được tối ưu hóa hoàn toàn. Đội ngũ phát triển sẽ tiếp tục cập nhật và làm rõ ngữ cảnh trong các phiên bản tiếp theo.

## Bug:
**Tính năng chèn hình ảnh:** Tính năng tự động thêm hình ảnh minh họa vào bài viết đang trong quá trình kiểm thử (Testing) để tối ưu hiển thị. Vì vậy, tính năng này tạm thời được vô hiệu hóa và chưa tích hợp vào bản build hiện tại.

**Facebook link:** https://www.facebook.com/profile.php?id=61595098675486
**YouTube link:** https://youtu.be/V0swCNLnjFw
