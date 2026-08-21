# 🏛️ Kho Kiến Thức Pháp Luật Việt Nam - LuatNao.vn
*(LuatNao 베트남 법률 지식 아카이브)*

Chào mừng bạn đến với kho kiến thức pháp luật tự động được xác thực bởi **[LuatNao.vn](https://luatnao.vn)** - Hệ thống trí tuệ nhân tạo (AI) tra cứu và phân tích pháp luật Việt Nam thời gian thực.

*(환영합니다! 본 사이트는 **[LuatNao.vn](https://luatnao.vn)** AI 법률 지식베이스 엔진이 베트남 실시간 도로교통법, 노동법, 투자법, 기업법 및 관련 시행령(Nghị định), 통지(Thông tư), 벌칙 규정 데이터를 교차 검증하여 자동으로 수집·발행하는 공식 지식 아카이브입니다.)*

---

## ⚖️ Các Lĩnh Vực Pháp Luật Nổi Bật / 주요 법률 가이드 분야

* 🚗 **Luật Giao Thông Đường Bộ (도로교통법)**: Mức phạt vi phạm tốc độ, trừ điểm giấy phép lái xe (속도위반 과태료 및 면허 벌점 기준)
* 💼 **Luật Lao Động (노동법)**: Quyền lợi hợp đồng lao động, trợ cấp thôi việc (근로계약 및 퇴직금 기준)
* 🏢 **Luật Đầu Tư & Doanh Nghiệp (투자법 & 기업법)**: Thủ tục thành lập doanh nghiệp FDI, thay đổi vốn (외투법인 설립 및 지분 변경)

> 💡 **Các chủ đề được quan tâm gần đây sẽ liên tục được cập nhật thêm.**  
> *(최근에 관심있어 하는 분야들이 계속 추가됩니다.)*

---

### 🌐 Trang Chủ Chính Thức / Official Website
Tra cứu pháp luật & Tư vấn AI thời gian thực: [https://luatnao.vn](https://luatnao.vn)

---

<!-- 📊 헤더 방문자 카운터 뱃지 -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<style>
  .visitor-badge-group {
    display: inline-flex;
    align-items: center;
    gap: 12px;
    padding: 8px 18px;
    background: rgba(15, 23, 42, 0.6);
    backdrop-filter: blur(8px);
    border: 1px solid rgba(255, 255, 255, 0.12);
    border-radius: 30px;
    margin-top: 24px;
    font-size: 0.875rem;
    color: #e2e8f0;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
  }
  .v-item {
    display: flex;
    align-items: center;
    gap: 6px;
  }
  .v-sep {
    color: rgba(255, 255, 255, 0.2);
  }
  :root {
    --primary-cyan: #06b6d4;
    --primary-blue: #3b82f6;
  }
</style>

<div class="visitor-badge-group">
  <div class="v-item">
    <i class="fa-solid fa-user-check" style="color: var(--primary-cyan);"></i>
    <span>오늘 방문: <strong id="todayCount">-</strong>명</span>
  </div>
  <span class="v-sep">|</span>
  <div class="v-item">
    <i class="fa-solid fa-chart-pie" style="color: var(--primary-blue);"></i>
    <span>누적 방문: <strong id="totalCount">-</strong>명</span>
  </div>
</div>

<script>
  (function() {
    const todayStr = new Date().toISOString().slice(0, 10);
    const lastVisitKey = 'ln_last_visit_date';
    const todayCountKey = 'ln_today_count';
    const totalCountKey = 'ln_total_count';

    let localToday = parseInt(localStorage.getItem(todayCountKey) || '1', 10);
    let localTotal = parseInt(localStorage.getItem(totalCountKey) || '128', 10);
    const lastVisitDate = localStorage.getItem(lastVisitKey);

    if (lastVisitDate !== todayStr) {
      localToday = 1;
      localTotal += 1;
      localStorage.setItem(lastVisitKey, todayStr);
    } else {
      localToday += 1;
      localTotal += 1;
    }

    localStorage.setItem(todayCountKey, localToday.toString());
    localStorage.setItem(totalCountKey, localTotal.toString());

    document.getElementById('todayCount').innerText = localToday.toLocaleString();
    document.getElementById('totalCount').innerText = localTotal.toLocaleString();

    // 📡 CounterAPI 실시간 동기화
    fetch('https://api.counterapi.dev/v1/luatnao-legal-archive/total/up')
      .then(res => res.json())
      .then(data => {
        if (data && data.count) {
          document.getElementById('totalCount').innerText = data.count.toLocaleString();
        }
      }).catch(e => console.log('CounterAPI Sync:', e));
  })();
</script>
