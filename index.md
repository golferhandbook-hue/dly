---
layout: default
title: "나오의 투자 썰 - 실전 투자 심리 & 팩폭 명언 아카이브"
description: "실전 단타·스캘핑 심리전, 뼈 때리는 팩폭 명언, 매일의 주식 인텔리전스를 기록하는 나오의 실전 투자 썰 아카이브"
---

<!-- ── 상단 커스텀 스타일 (디자인 시스템 & 페이징 UI) ── -->
<style>
  :root {
    --brand-primary: #2563eb;
    --brand-primary-hover: #1d4ed8;
    --brand-dark: #0f172a;
    --brand-gradient: linear-gradient(135deg, #1e3a8a 0%, #2563eb 100%);
    --card-bg: #ffffff;
    --card-border: #e2e8f0;
    --text-main: #0f172a;
    --text-muted: #64748b;
  }

  /* 글로벌 네비게이션 헤더 */
  .archive-nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 14px;
    padding: 16px 24px;
    background: #0f172a;
    border-radius: 14px;
    margin-bottom: 26px;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
    border: 1px solid rgba(255, 255, 255, 0.08);
  }
  .archive-brand {
    display: flex;
    align-items: center;
    gap: 12px;
    text-decoration: none;
  }
  .archive-brand-icon {
    font-size: 28px;
    filter: drop-shadow(0 2px 6px rgba(0, 0, 0, 0.3));
    transition: transform 0.2s ease;
  }
  .archive-brand:hover .archive-brand-icon {
    transform: scale(1.1);
  }
  .archive-brand-text {
    font-size: 19px;
    font-weight: 800;
    color: #ffffff;
    letter-spacing: -0.02em;
  }
  .archive-brand-badge {
    font-size: 10.5px;
    font-weight: 700;
    background: rgba(37, 99, 235, 0.3);
    color: #60a5fa;
    border: 1px solid rgba(59, 130, 246, 0.5);
    padding: 3px 8px;
    border-radius: 6px;
    text-transform: uppercase;
    letter-spacing: 0.04em;
  }
  .archive-nav-links {
    display: flex;
    align-items: center;
    gap: 6px;
    flex-wrap: wrap;
  }
  .archive-nav-link {
    color: #94a3b8;
    text-decoration: none;
    font-size: 13.5px;
    font-weight: 600;
    padding: 7px 14px;
    border-radius: 8px;
    transition: all 0.2s;
  }
  .archive-nav-link:hover, .archive-nav-link.active {
    color: #ffffff;
    background: rgba(255, 255, 255, 0.12);
  }
  .btn-header-cta {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    background: linear-gradient(135deg, #2563eb 0%, #1d4ed8 100%);
    color: #ffffff !important;
    text-decoration: none;
    font-size: 13px;
    font-weight: 700;
    padding: 8px 16px;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(37, 99, 235, 0.4);
    transition: all 0.2s;
  }
  .btn-header-cta:hover {
    transform: translateY(-1px);
    box-shadow: 0 4px 16px rgba(37, 99, 235, 0.6);
  }

  /* 검색 및 필터 구획 */
  .search-section {
    background: #ffffff;
    border: 1px solid #e2e8f0;
    border-radius: 14px;
    padding: 22px;
    margin-bottom: 28px;
    box-shadow: 0 4px 20px -4px rgba(0, 0, 0, 0.05);
  }
  .search-input-wrap {
    position: relative;
    margin-bottom: 16px;
  }
  .search-input-wrap input {
    width: 100%;
    box-sizing: border-box;
    padding: 13px 16px 13px 44px;
    font-size: 15px;
    border: 2px solid #cbd5e1;
    border-radius: 10px;
    outline: none;
    transition: border-color 0.2s;
  }
  .search-input-wrap input:focus {
    border-color: #2563eb;
    box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.15);
  }
  .search-icon {
    position: absolute;
    left: 14px;
    top: 50%;
    transform: translateY(-50%);
    font-size: 18px;
    color: #94a3b8;
  }
  .filter-chips {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    align-items: center;
  }
  .filter-chip {
    background: #f1f5f9;
    border: 1px solid #e2e8f0;
    color: #475569;
    font-size: 12.5px;
    font-weight: 600;
    padding: 6px 13px;
    border-radius: 20px;
    cursor: pointer;
    transition: all 0.15s;
    user-select: none;
  }
  .filter-chip:hover {
    background: #e2e8f0;
    color: #0f172a;
  }
  .filter-chip.active {
    background: #2563eb;
    border-color: #2563eb;
    color: #ffffff;
  }
  .search-count-bar {
    margin-top: 14px;
    font-size: 13px;
    color: #64748b;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 8px;
    font-weight: 500;
  }

  /* 카드 그리드 */
  .posts-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
    gap: 20px;
    margin-bottom: 36px;
    min-height: 200px;
  }
  .post-card {
    background: #ffffff;
    border: 1px solid #e2e8f0;
    border-radius: 14px;
    padding: 20px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    transition: all 0.2s cubic-bezier(0.16, 1, 0.3, 1);
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.04);
  }
  .post-card:hover {
    transform: translateY(-4px);
    border-color: #93c5fd;
    box-shadow: 0 12px 28px -4px rgba(37, 99, 235, 0.14);
  }
  .post-card-meta {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 12px;
  }
  .post-category-badge {
    background: #eff6ff;
    color: #1d4ed8;
    border: 1px solid #bfdbfe;
    font-size: 11.5px;
    font-weight: 700;
    padding: 3px 9px;
    border-radius: 6px;
    text-transform: uppercase;
  }
  .post-date {
    font-size: 12.5px;
    color: #94a3b8;
    font-weight: 500;
  }
  .post-card-title {
    font-size: 17px;
    font-weight: 800;
    color: #0f172a;
    line-height: 1.45;
    margin-bottom: 10px;
  }
  .post-card-title a {
    color: inherit;
    text-decoration: none;
  }
  .post-card-title a:hover {
    color: #2563eb;
  }
  .post-card-desc {
    font-size: 13.5px;
    color: #64748b;
    line-height: 1.6;
    margin-bottom: 16px;
    display: -webkit-box;
    -webkit-line-clamp: 3;
    -webkit-box-orient: vertical;
    overflow: hidden;
  }
  .post-card-tags {
    display: flex;
    gap: 5px;
    flex-wrap: wrap;
    margin-bottom: 14px;
  }
  .post-tag {
    font-size: 11px;
    color: #64748b;
    background: #f8fafc;
    border: 1px solid #e2e8f0;
    padding: 2px 7px;
    border-radius: 4px;
  }
  .post-card-footer {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-top: 1px solid #f1f5f9;
    padding-top: 12px;
    margin-top: auto;
  }
  .post-card-link {
    font-size: 13.5px;
    font-weight: 700;
    color: #2563eb;
    text-decoration: none;
  }
  .post-card-link:hover {
    text-decoration: underline;
  }

  /* 페이징 컨트롤 바 */
  .pagination-container {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 6px;
    margin: 36px 0 24px 0;
    flex-wrap: wrap;
    user-select: none;
  }
  .page-btn {
    min-width: 38px;
    height: 38px;
    padding: 0 12px;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    font-size: 13.5px;
    font-weight: 600;
    color: #334155;
    background: #ffffff;
    border: 1px solid #cbd5e1;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.15s ease;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.04);
  }
  .page-btn:hover:not(:disabled) {
    background: #f1f5f9;
    border-color: #94a3b8;
    color: #0f172a;
    transform: translateY(-1px);
  }
  .page-btn.active {
    background: #2563eb;
    border-color: #2563eb;
    color: #ffffff;
    font-weight: 700;
    box-shadow: 0 2px 8px rgba(37, 99, 235, 0.35);
  }
  .page-btn:disabled {
    opacity: 0.45;
    cursor: not-allowed;
    background: #f8fafc;
    border-color: #e2e8f0;
    color: #94a3b8;
  }

  /* 하단 푸터 & 방문자 카운터 */
  .archive-footer {
    margin-top: 50px;
    padding: 32px 24px;
    background: #0f172a;
    border-radius: 16px;
    color: #94a3b8;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: 18px;
    border: 1px solid rgba(255, 255, 255, 0.08);
  }
  .visitor-counter-bar {
    display: flex;
    align-items: center;
    gap: 12px;
    flex-wrap: wrap;
    justify-content: center;
    background: rgba(255, 255, 255, 0.06);
    padding: 10px 20px;
    border-radius: 24px;
    border: 1px solid rgba(255, 255, 255, 0.12);
  }
  .no-results-box {
    grid-column: 1 / -1;
    text-align: center;
    padding: 48px 20px;
    background: #f8fafc;
    border: 1px dashed #cbd5e1;
    border-radius: 12px;
    display: none;
  }
</style>

<!-- ── 1. 글로벌 네비게이션 헤더 ── -->
<nav class="archive-nav">
  <a href="{{ site.baseurl }}/" class="archive-brand">
    <span class="archive-brand-icon">📈</span>
    <div>
      <span class="archive-brand-text">나오의 투자 썰</span>
      <span class="archive-brand-badge">DAILY ARCHIVE</span>
    </div>
  </a>

  <div class="archive-nav-links">
    <a href="#" class="archive-nav-link active" onclick="setCategoryFilter('all', this); return false;">🏠 전체 썰</a>
    <a href="#" class="archive-nav-link" onclick="setCategoryFilter('팩폭명언', this); return false;">⚡ 팩폭 명언</a>
    <a href="#" class="archive-nav-link" onclick="setCategoryFilter('투자심리', this); return false;">🧠 매매 심리</a>
    <a href="#" class="archive-nav-link" onclick="setCategoryFilter('종목분석', this); return false;">🔍 종목 분석</a>
  </div>

  <a href="https://github.com/golferhandbook-hue/dly" target="_blank" rel="noopener" class="btn-header-cta">
    🐙 GitHub Repo →
  </a>
</nav>

<!-- ── 2. 검색 및 퀵 태그 필터 바 ── -->
<div class="search-section">
  <div class="search-input-wrap">
    <span class="search-icon">🔍</span>
    <input type="text" id="liveSearchInput" placeholder="종목명, 키워드, 명언 검색... (예: 레메디, 스카이랩스, 손절, 복리, 스캘퍼)" oninput="handleLiveSearch()" />
  </div>

  <div class="filter-chips">
    <span style="font-size: 12px; font-weight: 700; color: #475569; margin-right: 4px;">🏷️ 빠른 필터:</span>
    <span class="filter-chip active" onclick="setTagFilter('all', this)">전체</span>
    <span class="filter-chip" onclick="setTagFilter('팩폭명언', this)">#팩폭명언</span>
    <span class="filter-chip" onclick="setTagFilter('투자심리', this)">#투자심리</span>
    <span class="filter-chip" onclick="setTagFilter('단타', this)">#단타스캘핑</span>
    <span class="filter-chip" onclick="setTagFilter('레메디', this)">#레메디</span>
    <span class="filter-chip" onclick="setTagFilter('스카이랩스', this)">#스카이랩스</span>
    <span class="filter-chip" onclick="setTagFilter('손절', this)">#손절원칙</span>
  </div>

  <div class="search-count-bar">
    <span id="searchResultCount">투자 썰을 불러오는 중...</span>
    <span>⚡ 매일 장 마감 후 자동 업데이트</span>
  </div>
</div>

<!-- ── 3. 실전 투자 썰 카드 그리드 ── -->
<div class="posts-grid" id="postsGrid">

{% for post in site.posts %}
  <article class="post-card" 
    data-title="{{ post.title | downcase | escape }}"
    data-desc="{{ post.description | default: post.excerpt | strip_html | strip_newlines | downcase | escape }}"
    data-categories="{{ post.categories | join: ' ' | downcase | escape }}"
    data-tags="{{ post.tags | join: ' ' | downcase | escape }}"
  >
    <div>
      <div class="post-card-meta">
        <span class="post-category-badge">{{ post.categories | first | default: "실전투자썰" }}</span>
        <span class="post-date">📅 {{ post.date | date: "%Y-%m-%d" }}</span>
      </div>

      <h3 class="post-card-title">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>

      <div class="post-card-desc">
        {{ post.description | default: post.excerpt | strip_html | strip_newlines | truncate: 140 }}
      </div>

      {% if post.tags %}
      <div class="post-card-tags">
        {% for tag in post.tags limit:4 %}
        <span class="post-tag">#{{ tag }}</span>
        {% endfor %}
      </div>
      {% endif %}
    </div>

    <div class="post-card-footer">
      <a href="{{ post.url | relative_url }}" class="post-card-link">투자 썰 읽기 →</a>
      <span style="font-size: 11.5px; color: #94a3b8;">✍️ {{ post.author | default: "나오" }}</span>
    </div>
  </article>
  {% endfor %}

  <div class="no-results-box" id="noResultsBox">
    <div style="font-size: 32px; margin-bottom: 8px;">🔍</div>
    <strong style="color: #0f172a; font-size: 16px;">일치하는 투자 썰이 없습니다.</strong>
    <p style="color: #64748b; font-size: 13.5px; margin: 6px 0 0 0;">다른 검색어나 태그를 선택해 보세요.</p>
  </div>

</div>

<!-- ── 4. 스마트 페이징 컨트롤 바 ── -->
<div class="pagination-container" id="paginationContainer"></div>

<!-- ── 5. 하단 푸터 & 방문자수 카운터 ── -->
<footer class="archive-footer">
  <div class="visitor-counter-bar">
    <span style="font-size: 14px; font-weight: 700; color: #ffffff;">👥 누적 방문자수</span>
    <img src="https://api.visitorbadge.io/api/visitors?path=ssul.studioexitt.net&label=VISITORS&labelColor=%230f172a&countColor=%232563eb&style=flat" 
         alt="나오의 투자 썰 누적 방문자 카운터" 
         style="vertical-align: middle; height: 22px;" />
  </div>

  <div>
    <strong style="color: #ffffff; font-size: 15px;">📈 나오의 투자 썰 (Nao's Investment Stories)</strong>
    <p style="margin: 6px 0 0 0; font-size: 13px; color: #94a3b8; line-height: 1.6;">
      개미 투자자들의 치열한 실전 매매 심리와 뼈 때리는 팩폭 명언을 매일 기록하는 실전 투자 아카이브.<br>
      "익절은 1% 먹고 튀면서 물리면 기도하는 '비자발적 장기 기부 천사'가 되지 맙시다."
    </p>
  </div>

  <div style="font-size: 12px; color: #64748b; border-top: 1px solid rgba(255,255,255,0.08); padding-top: 14px; width: 100%;">
    © 2026 나오의 투자 썰. All rights reserved. | Powered by AGY STUDIO
  </div>
</footer>

<!-- ── 6. 실시간 검색, 카테고리 필터링, 페이징 스크립트 ── -->
<script>
  const CARDS_PER_PAGE = 9;
  let currentPage = 1;
  let currentCategory = 'all';
  let currentTag = 'all';
  let matchedCards = [];

  function updatePagination() {
    const totalCards = matchedCards.length;
    const totalPages = Math.ceil(totalCards / CARDS_PER_PAGE) || 1;
    if (currentPage > totalPages) currentPage = totalPages;

    const allCards = Array.from(document.querySelectorAll('.post-card'));
    allCards.forEach(c => c.style.display = 'none');

    const startIndex = (currentPage - 1) * CARDS_PER_PAGE;
    const endIndex = startIndex + CARDS_PER_PAGE;
    const currentSlice = matchedCards.slice(startIndex, endIndex);

    currentSlice.forEach(card => card.style.display = 'flex');

    const countLabel = document.getElementById('searchResultCount');
    if (countLabel) {
      countLabel.innerHTML = `총 <strong>${totalCards}</strong>편의 투자 썰 중 <strong>${currentSlice.length}</strong>편 표시 (페이지 ${currentPage}/${totalPages})`;
    }

    const noResults = document.getElementById('noResultsBox');
    if (noResults) {
      noResults.style.display = totalCards === 0 ? 'block' : 'none';
    }

    renderPaginationControls(totalPages);
  }

  function renderPaginationControls(totalPages) {
    const container = document.getElementById('paginationContainer');
    if (!container) return;
    if (totalPages <= 1) {
      container.innerHTML = '';
      return;
    }

    let html = '';
    const prevDisabled = currentPage === 1 ? 'disabled' : '';
    html += `<button class="page-btn" ${prevDisabled} onclick="goToPage(${currentPage - 1})">« 이전</button>`;

    for (let i = 1; i <= totalPages; i++) {
      const isActive = i === currentPage ? 'active' : '';
      html += `<button class="page-btn ${isActive}" onclick="goToPage(${i})">${i}</button>`;
    }

    const nextDisabled = currentPage === totalPages ? 'disabled' : '';
    html += `<button class="page-btn" ${nextDisabled} onclick="goToPage(${currentPage + 1})">다음 »</button>`;

    container.innerHTML = html;
  }

  function goToPage(page) {
    currentPage = page;
    updatePagination();
    const target = document.getElementById('liveSearchInput') || document.getElementById('postsGrid');
    if (target) target.scrollIntoView({ behavior: 'smooth', block: 'start' });
  }

  function handleLiveSearch() {
    const query = (document.getElementById('liveSearchInput').value || '').toLowerCase().trim();
    const cards = Array.from(document.querySelectorAll('.post-card'));

    matchedCards = cards.filter(card => {
      const title = card.getAttribute('data-title') || '';
      const desc = card.getAttribute('data-desc') || '';
      const categories = card.getAttribute('data-categories') || '';
      const tags = card.getAttribute('data-tags') || '';

      const matchesQuery = !query || title.includes(query) || desc.includes(query) || tags.includes(query);
      const matchesCategory = currentCategory === 'all' || categories.includes(currentCategory) || tags.includes(currentCategory);
      const matchesTag = currentTag === 'all' || tags.includes(currentTag) || categories.includes(currentTag);

      return matchesQuery && matchesCategory && matchesTag;
    });

    currentPage = 1;
    updatePagination();
  }

  function setCategoryFilter(cat, elem) {
    currentCategory = cat.toLowerCase();
    document.querySelectorAll('.archive-nav-link').forEach(el => el.classList.remove('active'));
    if (elem) elem.classList.add('active');
    handleLiveSearch();
  }

  function setTagFilter(tag, elem) {
    currentTag = tag.toLowerCase();
    document.querySelectorAll('.filter-chip').forEach(el => el.classList.remove('active'));
    if (elem) elem.classList.add('active');
    handleLiveSearch();
  }

  document.addEventListener('DOMContentLoaded', () => {
    handleLiveSearch();
  });
  handleLiveSearch();
</script>
