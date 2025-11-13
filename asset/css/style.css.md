/* ---- 全局基础 ---- */
*,
*::before,
*::after {
  box-sizing: border-box;
}

body {
  margin: 0;
  padding: 0;
  font-family: system-ui, -apple-system, BlinkMacSystemFont,
    "Segoe UI", "Noto Sans SC", "PingFang SC", sans-serif;
  background: #f7f5f0;          /* 米白偏暖，日系纸张感 */
  color: #2f3437;               /* 深灰，而不是纯黑 */
  line-height: 1.7;
}

/* 页面内容宽度控制 */
.page-wrapper {
  max-width: 960px;
  margin: 0 auto;
  padding: 32px 16px 64px;
}

/* ---- 标题、分割线 ---- */
h1, h2, h3 {
  font-weight: 500;
  letter-spacing: 0.04em;
  color: #262626;
}

h1 {
  font-size: 1.9rem;
  margin-bottom: 1rem;
}

h2 {
  font-size: 1.4rem;
  margin-top: 2.5rem;
  border-left: 4px solid #9cc3d5;  /* 淡蓝竖线 */
  padding-left: 0.75rem;
}

h3 {
  font-size: 1.1rem;
  margin-top: 1.5rem;
}

/* 小号浅灰标题说明 */
.section-note {
  font-size: 0.9rem;
  color: #8a8a8a;
}

/* ---- 链接 ---- */
a {
  color: #6c93b0;
  text-decoration: none;
  border-bottom: 1px solid rgba(108,147,176,0.3);
}

a:hover {
  border-bottom-color: rgba(108,147,176,0.8);
}

/* ---- 简历首页布局 ---- */
.resume-header {
  margin-bottom: 2rem;
  padding-bottom: 1.2rem;
  border-bottom: 1px solid #e3ded2;
}

.resume-title {
  font-size: 2.1rem;
  margin: 0 0 0.4rem;
}

.resume-subtitle {
  font-size: 1rem;
  color: #777;
}

/* 列表微调 */
ul {
  padding-left: 1.3rem;
}

/* ---- 作品集画廊 ---- */
.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 18px;
  margin-top: 1.5rem;
}

.gallery-item {
  background: #fdfcf8;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0,0,0,0.06);
  transition: transform 0.18s ease-out, box-shadow 0.18s ease-out;
}

.gallery-item img {
  display: block;
  width: 100%;
  height: auto;
}

.gallery-item-caption {
  padding: 10px 12px 12px;
  font-size: 0.9rem;
  color: #666;
}

/* hover 效果：轻微抬起 */
.gallery-item:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.08);
}

/* 返回首页按钮 */
.back-link {
  margin-top: 2rem;
  font-size: 0.95rem;
}

/* 手机端微调 */
@media (max-width: 600px) {
  .page-wrapper {
    padding: 20px 14px 48px;
  }
  h1 {
    font-size: 1.6rem;
  }
}
