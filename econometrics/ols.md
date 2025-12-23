<style>
/* 画面が広いときだけ2カラム（左メニュー＋本文） */
.layout {
  display: grid;
  grid-template-columns: 240px 1fr;
  gap: 20px;
  align-items: start;
}
.sidebar {
  position: sticky;
  top: 16px;
  padding: 14px;
  border: 1px solid #ddd;
  border-radius: 12px;
  background: #fff;
}
.sidebar a { text-decoration: none; }
.sidebar ul { margin: 0; padding-left: 18px; }
.sidebar .title { font-weight: 700; margin-bottom: 10px; }
.content { min-width: 0; }

/* スマホでは1カラムにする */
@media (max-width: 900px) {
  .layout { grid-template-columns: 1fr; }
  .sidebar { position: static; }
}
</style>

<script>
window.MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']],
    displayMath: [['$$', '$$']]
  }
};
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<div class="layout">

<nav class="sidebar">
  <div class="title">計量経済学</div>
  <ul>
    <li><a href="./index.html">トップ</a></li>
    <li><a href="./ols.html">OLS</a></li>
    <li><a href="./iv.html">IV</a></li>
  </ul>
  <hr>
  <div class="title">OLS 目次</div>
  <ul>
    <li><a href="#モデル">モデル</a></li>
    <li><a href="#推定量">推定量</a></li>
  </ul>
</nav>

<div class="content">

# 最小二乗法（OLS）

## モデル
$$
y = X\beta + u
$$

## 推定量
$$
\hat{\beta} = (X'X)^{-1}X'y
$$
</div>
</div>
