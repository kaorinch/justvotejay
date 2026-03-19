<!DOCTYPE html>

<html lang="zh-TW" style="background:#0f1520;">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TAG EVENT PLAYBOOK — #JustVoteJay</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Noto+Serif+TC:wght@200;300;400&display=swap" rel="stylesheet">
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

```
*, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

html {
  background: #0f1520 !important;
  min-height: 100%;
}

body {
  background: #0f1520 !important;
  color: var(--text-main);
  font-family: 'Noto Serif TC', serif;
  font-weight: 300;
  line-height: 1.8;
  min-height: 100vh;
  width: 100%;
}

.page {
  max-width: 900px;
  margin: 0 auto;
  padding: 48px 24px 60px;
}

.hero {
  text-align: center;
  padding: 52px 24px 40px;
  border-bottom: 1px solid var(--border);
}

.brand {
  font-family: 'Cormorant Garamond', serif;
  font-weight: 300;
  font-size: 12px;
  letter-spacing: 0.35em;
  color: var(--gold);
  text-transform: uppercase;
  margin-bottom: 20px;
}

.hero-title {
  font-family: 'Cormorant Garamond', serif;
  font-weight: 300;
  font-size: 15px;
  letter-spacing: 0.4em;
  color: var(--text-main);
  text-transform: uppercase;
  margin-bottom: 32px;
}

.hero-tagline {
  font-family: 'Cormorant Garamond', serif;
  font-style: italic;
  font-size: clamp(28px, 5vw, 44px);
  color: var(--gold-light);
  font-weight: 300;
  line-height: 1.3;
  margin-bottom: 28px;
}

.hero-tagline .diamond {
  color: var(--gold);
  font-style: normal;
  margin: 0 12px;
  font-size: 0.75em;
}

.hero-divider {
  width: 60px;
  height: 1px;
  background: var(--gold-dim);
  margin: 0 auto;
}

.card {
  background: var(--bg-card);
  border: 1px solid var(--border);
  border-radius: 4px;
  padding: 32px 36px;
  margin: 20px 0;
}

.card-title {
  font-family: 'Cormorant Garamond', serif;
  font-size: 18px;
  font-weight: 400;
  color: var(--gold-light);
  margin-bottom: 16px;
}

.card p {
  color: var(--text-main);
  font-size: 14px;
  line-height: 1.9;
  margin-bottom: 6px;
}

.phase-block {
  border-left: 2px solid var(--border);
  padding: 20px 24px;
  margin: 16px 0;
  background: var(--bg-card2);
  border-radius: 0 4px 4px 0;
}

.phase-header {
  font-size: 13px;
  color: var(--text-sub);
  margin-bottom: 10px;
  display: flex;
  align-items: center;
  gap: 10px;
  flex-wrap: wrap;
}

.phase-name { font-weight: 400; color: var(--text-main); font-size: 14px; }
.phase-target { color: var(--gold-dim); font-size: 12px; }

.phase-desc {
  font-size: 13.5px;
  color: var(--text-main);
  line-height: 1.85;
  margin-bottom: 14px;
}

.tags { display: flex; gap: 8px; flex-wrap: wrap; }

.tag {
  background: rgba(42, 61, 90, 0.6);
  border: 1px solid var(--border);
  color: var(--text-sub);
  font-size: 11px;
  padding: 4px 12px;
  border-radius: 2px;
}

.total-box {
  background: rgba(201, 168, 76, 0.08);
  border: 1px solid var(--gold-dim);
  border-radius: 4px;
  text-align: center;
  padding: 20px 24px;
  margin-top: 20px;
}

.total-main {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(20px, 4vw, 28px);
  font-weight: 300;
  color: var(--gold-light);
  letter-spacing: 0.05em;
}

.total-sub { font-size: 12px; color: var(--text-sub); margin-top: 4px; }

.post-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
  margin-top: 16px;
}

@media (max-width: 600px) {
  .post-grid { grid-template-columns: 1fr; }
  .rules-grid { grid-template-columns: 1fr; }
}

.post-category { margin-bottom: 16px; }
.post-cat-label { font-size: 12px; color: var(--text-sub); margin-bottom: 10px; }
.post-cat-label span { color: var(--gold-dim); margin-right: 6px; }

.post-item {
  background: var(--bg-card2);
  border: 1px solid var(--border);
  border-radius: 3px;
  padding: 12px 14px;
  font-size: 13px;
  color: var(--text-main);
  line-height: 1.7;
  margin-bottom: 8px;
}

.rules-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 24px;
  margin-top: 16px;
}

.rules-col-title { font-size: 14px; font-weight: 400; margin-bottom: 16px; }
.rules-col-title.do { color: var(--green); }
.rules-col-title.dont { color: var(--red); }

.rule-item {
  display: flex;
  align-items: flex-start;
  gap: 10px;
  font-size: 13px;
  color: var(--text-main);
  line-height: 1.7;
  margin-bottom: 14px;
}

.rule-icon { flex-shrink: 0; margin-top: 3px; font-size: 12px; }
.rule-icon.do { color: var(--green); }
.rule-icon.dont { color: var(--red); }

.footer {
  text-align: center;
  padding: 36px 0 20px;
  border-top: 1px solid var(--border);
  margin-top: 20px;
  font-family: 'Cormorant Garamond', serif;
  font-size: 12px;
  letter-spacing: 0.3em;
  color: var(--gold-dim);
  text-transform: uppercase;
}
```

  </style>
</head>
<body>
  <div class="page">

```
<div class="hero">
  <div class="brand">JAYBIRDS ✦ #JUSTVOTEJAY</div>
  <div class="hero-title">TAG EVENT PLAYBOOK</div>
  <div class="hero-tagline">
    #JustVoteJay <span class="diamond">✦</span> 3/26（Thu.）18:00〜19:00
  </div>
  <div class="hero-divider"></div>
</div>

<div class="card">
  <div class="card-title">✦ 什麼是TAG活動</div>
  <p>所有參與者在指定時間內，同時使用相同的主題標籤發文，藉此衝上X（Twitter）的熱門趨勢。</p>
  <p>本次目的是提升莊宗傑的知名度。在節目播出前，透過X讓更多人認識莊宗傑，吸引更多觀眾收看。</p>
</div>

<div class="card">
  <div class="card-title">✦ 各時段行動策略</div>

  <div class="phase-block">
    <div class="phase-header">
      <span>18:00〜18:10</span>
      <span class="phase-name">初動階段</span>
      <span>🎯</span>
      <span class="phase-target">目標：每人 10〜15 則推文</span>
    </div>
    <div class="phase-desc">這10分鐘決定一切。一口氣發出預先準備好的草稿。趨勢演算法會偵測初期的急速上升，因此全員集中火力是最重要的事。</div>
    <div class="tags">
      <span class="tag">禁止圖片・影片・表情符號</span>
      <span class="tag">僅限短文字</span>
    </div>
  </div>

  <div class="phase-block">
    <div class="phase-header">
      <span>18:10〜18:40</span>
      <span class="phase-name">擴散階段</span>
      <span>🎯</span>
      <span class="phase-target">目標：每人 15〜20 則推文</span>
    </div>
    <div class="phase-desc">開放圖片與影片。以「讓初次認識莊宗傑的人也能了解」的心態發文。若已進入趨勢，貼文會被更多人看見，請避免只有粉絲才懂的內容。</div>
    <div class="tags">
      <span class="tag">圖片・影片 OK</span>
      <span class="tag">以布道型推文為主</span>
    </div>
  </div>

  <div class="phase-block">
    <div class="phase-header">
      <span>18:40〜19:00</span>
      <span class="phase-name">收尾階段</span>
      <span>🎯</span>
      <span class="phase-target">目標：每人 5〜10 則推文</span>
    </div>
    <div class="phase-desc">堅持到最後。這是容易鬆懈的時段，請由支援帳號發出提醒，保持熱度。</div>
  </div>

  <div class="total-box">
    <div class="total-main">每人 30〜45 則　全體 1,500〜2,250 則</div>
    <div class="total-sub">在1小時內累積這個數字，有助於提高進入熱門趨勢的可能性</div>
  </div>
</div>

<div class="card">
  <div class="card-title">✦ 推文範例</div>
  <p style="font-size:13px; color:var(--text-sub); margin-bottom:20px;">大量複製同一句話可能被判定為垃圾訊息，請變換用詞後使用。</p>

  <div class="post-grid">
    <div>
      <div class="post-category">
        <div class="post-cat-label"><span>①</span> 喜歡上他的契機</div>
        <div class="post-item">第一次看到莊宗傑的瞬間就無法移開視線 #JustVoteJay</div>
        <div class="post-item">看了那個表演，瞬間就淪陷了 #JustVoteJay</div>
      </div>
      <div class="post-category">
        <div class="post-cat-label"><span>③</span> 表達感情與心情</div>
        <div class="post-item">想到莊宗傑就自然地充滿活力 #JustVoteJay</div>
        <div class="post-item">支持他讓我自己也變得積極向上 #JustVoteJay</div>
      </div>
      <div class="post-category">
        <div class="post-cat-label"><span>⑤</span> 短句・一言（初動階段用）</div>
        <div class="post-item">莊宗傑的笑容太讓人心動 #JustVoteJay</div>
        <div class="post-item">莊宗傑的表演讓人太期待了 #JustVoteJay</div>
        <div class="post-item">我推莊宗傑 #JustVoteJay</div>
      </div>
    </div>
    <div>
      <div class="post-category">
        <div class="post-cat-label"><span>②</span> 具體喜歡的地方</div>
        <div class="post-item">莊宗傑對舞蹈每個細節的堅持太讓人著迷了 #JustVoteJay</div>
        <div class="post-item">歌聲溫柔卻有力量，讓人一直想聽下去 #JustVoteJay</div>
      </div>
      <div class="post-category">
        <div class="post-cat-label"><span>④</span> 對節目的期待・引導初次收看者</div>
        <div class="post-item">今晚的Produce 101 Japan Shinsekai有一位叫莊宗傑的練習生，請一定要看 #JustVoteJay</div>
        <div class="post-item">今晚有播出，請一定要認識莊宗傑 #JustVoteJay</div>
      </div>
      <div class="post-category">
        <div class="post-cat-label"><span>⑥</span> ENGLISH</div>
        <div class="post-item">I can't stop watching Chuang Jay, he's everything #JustVoteJay</div>
        <div class="post-item">Chuang Jay's performance tonight, don't miss it #JustVoteJay</div>
      </div>
    </div>
  </div>
</div>

<div class="card">
  <div class="card-title">✦ 參加注意事項</div>
  <div class="rules-grid">
    <div>
      <div class="rules-col-title do">✓　請做的事</div>
      <div class="rule-item"><span class="rule-icon do">✓</span><span>事先準備最少10〜15則草稿</span></div>
      <div class="rule-item"><span class="rule-icon do">✓</span><span>18:00一到立即開始發文</span></div>
      <div class="rule-item"><span class="rule-icon do">✓</span><span>盡量在1小時內不要離開</span></div>
      <div class="rule-item"><span class="rule-icon do">✓</span><span>換句話說，用多樣化的句子發文</span></div>
    </div>
    <div>
      <div class="rules-col-title dont">✕　請勿做的事</div>
      <div class="rule-item"><span class="rule-icon dont">✕</span><span>18:00前使用標籤（會分散初期的集中度，最重要）</span></div>
      <div class="rule-item"><span class="rule-icon dont">✕</span><span>直接複製貼上同一句話連續發文（有被判定垃圾訊息的風險）</span></div>
      <div class="rule-item"><span class="rule-icon dont">✕</span><span>同時附上2個以上的標籤（集中在1個）</span></div>
      <div class="rule-item"><span class="rule-icon dont">✕</span><span>加入標點符號・表情符號（初動階段尤其重要）</span></div>
      <div class="rule-item"><span class="rule-icon dont">✕</span><span>18:10前使用圖片・影片</span></div>
      <div class="rule-item"><span class="rule-icon dont">✕</span><span>引用非互相追蹤者的推文（不會反映在趨勢上）</span></div>
      <div class="rule-item"><span class="rule-icon dont">✕</span><span>用多個帳號參加（違反X使用規範）</span></div>
    </div>
  </div>
</div>

<div class="footer">JAYBIRDS ✦ #JustVoteJay</div>
```

  </div>
</body>
</html>
