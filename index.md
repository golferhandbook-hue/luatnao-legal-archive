---
layout: default
title: "Kho Kiến Thức & Hỏi Đáp Pháp Luật Việt Nam - LuatNao.vn"
---

<div style="background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%); color: #ffffff; padding: 28px 24px; border-radius: 12px; margin-bottom: 30px; box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.3); border: 1px solid rgba(255, 255, 255, 0.1);">
  <h2 style="margin-top: 0; color: #38bdf8; font-size: 1.6rem; display: flex; align-items: center; gap: 8px;">
    ⚖️ LuatNao Legal Intelligence AI
  </h2>
  <p style="font-size: 1.05rem; line-height: 1.6; color: #cbd5e1; margin-bottom: 18px;">
    Hệ thống lưu trữ và tra cứu kiến thức pháp luật Việt Nam thời gian thực. Được hỗ trợ bởi trí tuệ nhân tạo (AI) phân tích và đối chiếu đa tầng các Nghị định, Thông tư, mức xử phạt và quy định hiện hành.
  </p>
  <div style="display: flex; gap: 12px; flex-wrap: wrap;">
    <a href="https://luatnao.vn" style="display: inline-flex; align-items: center; background: #0284c7; color: #ffffff; padding: 10px 20px; border-radius: 8px; text-decoration: none; font-weight: bold; box-shadow: 0 4px 12px rgba(2, 132, 199, 0.4);">
      🚀 Tra cứu & Tư vấn AI trực tuyến miễn phí tại LuatNao.vn →
    </a>
  </div>
</div>

## 📚 Danh Mục Hỏi Đáp Pháp Luật Mới Nhất / 최근 법률 가이드 & Q&A

{% if site.posts.size > 0 %}
<div style="display: grid; gap: 16px; margin-top: 20px;">
{% for post in site.posts limit:50 %}
  <div style="border: 1px solid #e2e8f0; border-radius: 10px; padding: 18px 20px; background: #ffffff; box-shadow: 0 2px 6px rgba(0,0,0,0.04); transition: transform 0.2s ease;">
    <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 8px;">
      <span style="font-size: 0.8rem; background: #e0f2fe; color: #0369a1; padding: 3px 8px; border-radius: 4px; font-weight: 600;">
        {{ post.categories | join: ', ' | default: 'Pháp Luật' }}
      </span>
      <span style="font-size: 0.8rem; color: #64748b;">
        📅 {{ post.date | date: "%Y-%m-%d" }}
      </span>
    </div>
    <h3 style="margin: 0 0 10px 0; font-size: 1.2rem;">
      <a href="{{ post.url | relative_url }}" style="color: #0f172a; text-decoration: none; font-weight: 700;">
        {{ post.title }}
      </a>
    </h3>
    <p style="margin: 0; color: #475569; font-size: 0.95rem; line-height: 1.5;">
      {{ post.description | default: post.excerpt | strip_html | truncatewords: 30 }}
    </p>
    <div style="margin-top: 12px; display: flex; justify-content: space-between; align-items: center;">
      <a href="{{ post.url | relative_url }}" style="color: #0284c7; font-size: 0.9rem; font-weight: 600; text-decoration: none;">
        Đọc chi tiết bài viết →
      </a>
      <a href="https://luatnao.vn" style="color: #64748b; font-size: 0.85rem; text-decoration: none;">
        ⚖️ Hỏi AI vụ việc này
      </a>
    </div>
  </div>
{% endfor %}
</div>
{% else %}
<p style="color: #64748b; font-style: italic;">
  Hiện tại chưa có bài viết nào được đăng tải. Các bài viết hỏi đáp pháp luật sẽ tự động hiển thị tại đây khi hệ thống cập nhật.
</p>
{% endif %}

---

## 🏷️ Các Chủ Đề Quan Tâm / 주요 법률 분야
* 🚗 **Giao Thông Đường Bộ**: Mức phạt vi phạm tốc độ, nồng độ cồn, trừ điểm GPLX theo quy định mới nhất.
* 💼 **Lao Động & Tiền Lương**: Hợp đồng lao động, chấm dứt HĐLĐ, trợ cấp thôi việc, bảo hiểm xã hội.
* 🏢 **Đầu Tư FDI & Doanh Nghiệp**: Thành lập công ty vốn nước ngoài, thay đổi giấy phép, thuế doanh nghiệp.

---
*(Kho kiến thức pháp luật được tự động cập nhật bởi [LuatNao.vn](https://luatnao.vn) AI Engine)*
