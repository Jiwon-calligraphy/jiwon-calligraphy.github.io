/* ===== 基础整体风格：日系 · 清新 · 留白 ===== */
body {
  margin: 0;
  padding: 0;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI",
               "Noto Sans SC", "PingFang SC", "Hiragino Sans GB",
               "Microsoft YaHei", sans-serif;
  background: #f5f7fb;              /* 很淡的雾感蓝灰 */
  color: #333;
  line-height: 1.8;
}

/* GitHub Pages 渲染 markdown 时常用的容器类名 */
.markdown-body {
  max-width: 860px;
  margin: 40px auto;
  padding: 32px 20px 48px;
  background: #fcfcff;
  border-radius: 18px;
  box-shadow: 0 16px 40px rgba(15, 23, 42, 0.06);
}

/* 标题：日系一点的低饱和墨绿色 */
.markdown-body h1,
.markdown-body h2,
.markdown-body h3 {
  font-weight: 600;
  color: #1b3a3f;
}

.markdown-body h1 {
  font-size: 1.9rem;
  margin-bottom: 1rem;
}

.markdown-body h2 {
  margin-top: 2.2rem;
  margin-bottom: 0.8rem;
}

/* 小标题前加点日系感的分隔线 */
.markdown-body h2::before {
  content: " ";
  display: inline-block;
  width: 8px;
  height: 8px;
  margin-right: 6px;
  border-radius: 999px;
  background: #87b1c9;
}

/* 文本链接：淡蓝色 + 轻微下划线 */
.markdown-body a {
  color: #2f6f9f;
  text-decoration: none;
  border-bottom: 1px solid rgba(47, 111, 159, 0.25);
}
.markdown-body a:hover {
  border-bottom-color: rgba(47, 111, 159, 0.6);
}

/* ===== 作品宫格布局 ===== */
.gallery {
  margin-top: 1.5rem;
  display: grid;
  gap: 20px;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
}

.work-card {
  background: #ffffff;
  border-radius: 16px;
  padding: 10px;
  box-shadow: 0 10px 24px rgba(15, 23, 42, 0.06);
  transition: transform 0.15s ease-out, box-shadow 0.15s ease-out;
}

.work-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 16px 32px rgba(15, 23, 42, 0.10);
}

.work-card img {
  width: 100%;
  display: block;
  border-radius: 12px;
}

/* 作品下的小字说明 */
.work-caption {
  margin-top: 6px;
  font-size: 0.85rem;
  color: #666;
}

/* 返回首页链接 */
.back-home {
  margin-top: 2.5rem;
  text-align: center;
  font-size: 0.9rem;
}
.back-home a {
  border-bottom: none;
  color: #7a8aa0;
}
.back-home a:hover {
  color: #2f6f9f;
}
