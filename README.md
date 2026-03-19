<!DOCTYPE html>

<html lang="zh-TW">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TAG EVENT PLAYBOOK — #JustVoteJay</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300&family=Noto+Serif+TC:wght@300;400;600&display=swap" rel="stylesheet">
<style>
  :root {
    --bg-dark: #0f1520;
    --bg-card: #162035;
    --bg-card2: #1a2640;
    --gold: #c9a84c;
    --gold-light: #e0c46a;
    --gold-dim: #a07830;
    --text-main: #dce8f0;
    --text-sub: #8eacc0;
    --border: #2a3d5a;
    --green: #6abf8a;
    --red: #d96060;
  }

- { margin: 0; padding: 0; box-sizing: border-box; }

body {
background-color: var(–bg-dark);
color: var(–text-main);
font-family: ‘Noto Serif TC’, serif;
font-weight: 300;
line-height: 1.8;
min-height: 100vh;
}

/* ===== PAGE 1 ===== */
.page {
max-width: 900px;
margin: 0 auto;
padding: 48px 24px 60px;
}

/* ===== PAGE 2 HERO ===== */
.hero {
text-align: center;
padding: 52px 24px 40px;
border-bottom: 1px solid var(–border);
margin-bottom: 0;
}

.brand {
font-family: ‘Cormorant Garamond’, serif;
font-weight: 300;
font-size: 12px;
letter-spacing: 0.35em;
color: var(–gold);
text-transform: uppercase;
margin-bottom: 20px;
}

.brand .diamond { margin: 0 8px; }

.hero-title {
font-family: ‘Cormorant Garamond’, serif;
font-size: clamp(14px, 2.5vw, 18px);
letter-spacing: 0.3em;
text-transform: uppercase;
color: var(–text-sub);
margin-bottom: 28px;
}

.hero-event {
font-family: ‘Cormorant Garamond’, serif;
font-size: clamp(30px, 6vw, 52px);
font-weight: 300;
font-style: italic;
color: var(–gold-light);
line-height: 1.2;
letter-spacing: 0.02em;
}

.hero-event span {
color: var(–text-main);
font-style: normal;
font-weight: 600;
}

.hero-divider {
width: 80px;
height: 1px;
background: var(–gold-dim);
margin: 28px auto 0;
}

/* ===== SECTION CARD ===== */
.section-card {
background: var(–bg-card);
border: 1px solid var(–border);
border-radius: 4px;
padding: 32px 36px;
margin-bottom: 24px;
}

.section-title {
font-family: ‘Cormorant Garamond’, serif;
font-size: 22px;
font-weight: 600;
color: var(–gold-light);
margin-bottom: 16px;
display: flex;
align-items: center;
gap: 10px;
}

.section-title .diamond { color: var(–gold); font-size: 16px; }

.section-body {
font-size: 14px;
color: var(–text-main);
line-height: 1.9;
}

/* ===== TIME BLOCKS ===== */
.time-block {
border-left: 2px solid var(–gold-dim);
padding: 18px 20px;
margin-bottom: 16px;
background: var(–bg-card2);
border-radius: 0 4px 4px 0;
}

.time-block:last-child { margin-bottom: 0; }

.time-header {
display: flex;
align-items: center;
gap: 12px;
margin-bottom: 10px;
flex-wrap: wrap;
}

.time-range {
font-family: ‘Cormorant Garamond’, serif;
font-size: 13px;
font-weight: 400;
color: var(–text-sub);
letter-spacing: 0.05em;
}

.phase-name {
font-size: 14px;
font-weight: 600;
color: var(–text-main);
}

.phase-target {
font-size: 12px;
color: var(–gold);
margin-left: auto;
}

.phase-target .emoji { margin-right: 4px; }

.time-desc {
font-size: 13.5px;
color: var(–text-main);
line-height: 1.85;
margin-bottom: 12px;
}

.tags {
display: flex;
gap: 8px;
flex-wrap: wrap;
}

.tag {
font-size: 11.5px;
padding: 3px 10px;
border-radius: 2px;
letter-spacing: 0.03em;
}

.tag-red { background: rgba(200,80,80,0.15); color: #e08080; border: 1px solid rgba(200,80,80,0.3); }
.tag-blue { background: rgba(80,130,200,0.15); color: #80b0e0; border: 1px solid rgba(80,130,200,0.3); }
.tag-green { background: rgba(80,180,120,0.15); color: #80d0a0; border: 1px solid rgba(80,180,120,0.3); }

/* ===== TOTAL BOX ===== */
.total-box {
background: var(–bg-card2);
border: 1px solid var(–gold-dim);
border-radius: 4px;
padding: 20px 24px;
text-align: center;
margin-top: 20px;
}

.total-main {
font-family: ‘Cormorant Garamond’, serif;
font-size: 26px;
font-weight: 600;
color: var(–gold-light);
letter-spacing: 0.05em;
}

.total-sub {
font-size: 12px;
color: var(–text-sub);
margin-top: 6px;
}

/* ===== POST EXAMPLES ===== */
.post-grid {
display: grid;
grid-template-columns: 1fr 1fr;
gap: 20px;
margin-top: 8px;
}

@media (max-width: 600px) {
.post-grid { grid-template-columns: 1fr; }
}

.post-col {}

.post-col-title {
font-size: 12.5px;
color: var(–gold);
letter-spacing: 0.08em;
margin-bottom: 10px;
display: flex;
align-items: center;
gap: 6px;
}

.post-col-title .num {
font-family: ‘Cormorant Garamond’, serif;
font-size: 14px;
color: var(–gold-dim);
}

.post-item {
background: var(–bg-dark);
border: 1px solid var(–border);
border-radius: 3px;
padding: 10px 14px;
font-size: 13px;
color: var(–text-main);
line-height: 1.7;
margin-bottom: 8px;
}

.post-item:last-child { margin-bottom: 0; }

.post-note {
font-size: 12px;
color: var(–text-sub);
margin-bottom: 14px;
line-height: 1.7;
}

/* ===== DOS AND DON’TS ===== */
.dos-donts {
display: grid;
grid-template-columns: 1fr 1fr;
gap: 24px;
margin-top: 8px;
}

@media (max-width: 600px) {
.dos-donts { grid-template-columns: 1fr; }
}

.dos-col-title {
font-size: 16px;
font-weight: 600;
margin-bottom: 14px;
display: flex;
align-items: center;
gap: 8px;
}

.dos-col-title.green { color: var(–green); }
.dos-col-title.red { color: var(–red); }

.list-item {
font-size: 13.5px;
color: var(–text-main);
line-height: 1.85;
margin-bottom: 8px;
display: flex;
align-items: flex-start;
gap: 8px;
}

.list-icon {
flex-shrink: 0;
font-size: 13px;
margin-top: 3px;
}

.list-icon.green { color: var(–green); }
.list-icon.red { color: var(–red); }

/* ===== FOOTER ===== */
.footer {
text-align: center;
padding: 28px 0 20px;
font-family: ‘Cormorant Garamond’, serif;
font-size: 12px;
letter-spacing: 0.3em;
color: var(–gold-dim);
text-transform: uppercase;
}

.page-break {
border: none;
border-top: 1px solid var(–border);
margin: 0;
}
</style>

</head>
<body>

<!-- ========== PAGE 2 CONTENT (HERO) ========== -->

<div class="hero">
  <div class="brand">JAYBIRDS <span class="diamond">✦</span> #JUSTVOTEJAY</div>
  <div class="hero-title">TAG EVENT PLAYBOOK</div>
  <div class="hero-event">
    #JustVoteJay <span style="color:var(--gold); font-style:normal;">✦</span>
    <span>3/26(Thu.) 18:00〜19:00</span>
  </div>
  <div class="hero-divider"></div>
</div>

<div class="page">

  <!-- 什麼是標籤活動 -->

  <div class="section-card">
    <div class="section-title"><span class="diamond">✦</span> 什麼是標籤活動</div>
    <div class="section-body">
      在指定時間內，所有人同時加上相同的主題標籤發文，藉此衝上 X（Twitter）熱門趨勢的活動。<br>
      本次目的是擴大對 莊宗傑的認知度。在播出前透過 X 廣傳他的名字，讓更多人收看節目。
    </div>
  </div>

  <!-- 各時段行動方式 -->

  <div class="section-card">
    <div class="section-title"><span class="diamond">✦</span> 各時段行動方式</div>

```
<div class="time-block">
  <div class="time-header">
    <span class="time-range">18:00〜18:10</span>
    <span class="phase-name">🚀 初動階段</span>
    <span class="phase-target"><span class="emoji">🎯</span>目標：每人 10〜15 則貼文</span>
  </div>
  <div class="time-desc">
    這 10 分鐘決定一切。將事先準備好的草稿一口氣發出。<br>
    趨勢演算法會偵測最初的急速上升，因此全員集中行動至關重要。
  </div>
  <div class="tags">
    <span class="tag tag-red">禁止圖片・影片・表情符號</span>
    <span class="tag tag-blue">僅限純文字</span>
  </div>
</div>

<div class="time-block">
  <div class="time-header">
    <span class="time-range">18:10〜18:40</span>
    <span class="phase-name">📣 推廣階段</span>
    <span class="phase-target"><span class="emoji">🎯</span>目標：每人 15〜20 則貼文</span>
  </div>
  <div class="time-desc">
    開放使用圖片・影片。以「讓第一次認識 莊宗傑 的人也能了解他」的心情發文。<br>
    若已進入熱門趨勢，貼文將觸及圈外人士，請避免只有圈內人才懂的內容。
  </div>
  <div class="tags">
    <span class="tag tag-green">可使用圖片・影片</span>
    <span class="tag tag-blue">以推廣貼文為主</span>
  </div>
</div>

<div class="time-block">
  <div class="time-header">
    <span class="time-range">18:40〜19:00</span>
    <span class="phase-name">🏁 收尾階段</span>
    <span class="phase-target"><span class="emoji">🎯</span>目標：每人 5〜10 則貼文</span>
  </div>
  <div class="time-desc">
    堅持到最後，不要中途離開。這段時間容易鬆懈，請由支援帳號發出提醒。
  </div>
</div>

<div class="total-box">
  <div class="total-main">每人 30〜45 則　全體 1,500〜2,250 則</div>
  <div class="total-sub">在 1 小時內累積這個數字，進入趨勢的可能性將大幅提升</div>
</div>
```

  </div>

  <div class="footer">JAYBIRDS ✦ #JustVoteJay</div>
</div>

<hr class="page-break">

<!-- ========== PAGE 1 CONTENT ========== -->

<div class="page">

  <!-- 貼文範例 -->

  <div class="section-card">
    <div class="section-title"><span class="diamond">✦</span> 貼文範例</div>
    <p class="post-note">大量轉貼相同文章可能被判定為垃圾訊息，請更換措辭後使用。</p>

```
<div class="post-grid">
  <!-- 左欄 -->
  <div class="post-col">

    <div class="post-col-title"><span class="num">①</span> 喜歡上他的契機</div>
    <div class="post-item">第一次看到 莊宗傑 的瞬間，眼睛就再也移不開了 #JustVoteJay</div>
    <div class="post-item">看了那場表演，在幾秒內就完全淪陷了 #JustVoteJay</div>

    <div class="post-col-title" style="margin-top:16px;"><span class="num">③</span> 用文字表達情感</div>
    <div class="post-item">一想到 莊宗傑，心情自然就變好了 #JustVoteJay</div>
    <div class="post-item">支持他，讓我自己也變得更積極向前 #JustVoteJay</div>

    <div class="post-col-title" style="margin-top:16px;"><span class="num">⑤</span> 短句・簡文（適合初動階段）</div>
    <div class="post-item">莊宗傑 的笑容太迷人了 #JustVoteJay</div>
    <div class="post-item">莊宗傑 的表演讓人太期待 #JustVoteJay</div>
    <div class="post-item">我在為 莊宗傑 應援 #JustVoteJay</div>

  </div>

  <!-- 右欄 -->
  <div class="post-col">

    <div class="post-col-title"><span class="num">②</span> 具體喜歡的地方</div>
    <div class="post-item">莊宗傑 對舞蹈細節的講究太厲害了 #JustVoteJay</div>
    <div class="post-item">歌聲溫柔卻有力，一直聽都不膩 #JustVoteJay</div>

    <div class="post-col-title" style="margin-top:16px;"><span class="num">④</span> 對播出的期待・吸引新觀眾</div>
    <div class="post-item">今晚的 Produce 101 Japan Shinsekai，有個叫 莊宗傑 的練習生，一定要看！ #JustVoteJay</div>
    <div class="post-item">今晚播出，請大家認識一下 莊宗傑！ #JustVoteJay</div>

    <div class="post-col-title" style="margin-top:16px;"><span class="num">⑥</span> ENGLISH</div>
    <div class="post-item">I can't stop watching 莊宗傑, he's everything #JustVoteJay</div>
    <div class="post-item">莊宗傑's performance tonight, don't miss it #JustVoteJay</div>

  </div>
</div>
```

  </div>

  <!-- 注意事項 -->

  <div class="section-card">
    <div class="section-title"><span class="diamond">✦</span> 參加注意事項</div>

```
<div class="dos-donts">
  <!-- DO -->
  <div>
    <div class="dos-col-title green">✓ 請務必做到</div>
    <div class="list-item"><span class="list-icon green">✓</span><span>事先至少準備 10〜15 則草稿備用</span></div>
    <div class="list-item"><span class="list-icon green">✓</span><span>一到 18:00 立即開始發文</span></div>
    <div class="list-item"><span class="list-icon green">✓</span><span>1 小時內盡量不要離開</span></div>
    <div class="list-item"><span class="list-icon green">✓</span><span>用自己的話改寫，以多樣化的文章發文</span></div>
  </div>

  <!-- DON'T -->
  <div>
    <div class="dos-col-title red">✗ 請絕對避免</div>
    <div class="list-item"><span class="list-icon red">✗</span><span>18:00 之前使用標籤（會降低初動熱度／最重要）</span></div>
    <div class="list-item"><span class="list-icon red">✗</span><span>直接複製貼上相同文章連續發文（垃圾訊息風險）</span></div>
    <div class="list-item"><span class="list-icon red">✗</span><span>同時使用 2 個以上的標籤（只集中使用 1 個）</span></div>
    <div class="list-item"><span class="list-icon red">✗</span><span>加入標點符號・表情符號（初動階段尤其禁止）</span></div>
    <div class="list-item"><span class="list-icon red">✗</span><span>在 18:10 之前使用圖片・影片</span></div>
    <div class="list-item"><span class="list-icon red">✗</span><span>引用非互追帳號的貼文（不會反映在趨勢中）</span></div>
    <div class="list-item"><span class="list-icon red">✗</span><span>使用多個帳號參加（違反 X 使用規則）</span></div>
  </div>
</div>
```

  </div>

  <div class="footer">JAYBIRDS ✦ #JustVoteJay</div>
</div>

</body>
</html>
