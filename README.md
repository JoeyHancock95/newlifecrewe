<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>How's Your Posture? Week 5: Celebration</title>
<link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@700;900&family=Barlow:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --ice: #D8E8F0;
    --ice-dark: #B8D0E0;
    --wheat: #E8D5A0;
    --wheat-dark: #D4BC7A;
    --mint: #B8E0B0;
    --mint-dark: #90C888;
    --ink: #1A1A1A;
    --ink-light: #3A3A3A;
    --muted: #6A7A88;
    --cream: #F8F6F0;
    --ticker: #E0EAF0;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'Barlow', Arial, sans-serif;
    background: var(--cream);
    color: var(--ink);
    line-height: 1.7;
    font-size: 17px;
  }

  /* ── TICKER ── */
  .ticker-wrap {
    background: var(--ticker);
    overflow: hidden;
    padding: 8px 0;
    border-bottom: 1px solid var(--ice-dark);
  }
  .ticker-text {
    white-space: nowrap;
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 700;
    font-size: 13px;
    letter-spacing: 0.08em;
    color: var(--ink);
    animation: ticker 30s linear infinite;
    display: inline-block;
  }
  @keyframes ticker {
    0% { transform: translateX(100vw); }
    100% { transform: translateX(-100%); }
  }

  /* ── HEADER ── */
  .sermon-header {
    background: var(--ice);
    padding: 60px 48px 48px;
    border-bottom: 1px solid var(--ice-dark);
    position: relative;
    overflow: hidden;
  }
  .header-bg-text {
    position: absolute;
    bottom: -20px; right: -10px;
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 900;
    font-size: 180px;
    color: rgba(0,0,0,0.04);
    line-height: 1;
    text-transform: uppercase;
    pointer-events: none;
    letter-spacing: -0.02em;
  }
  .series-label {
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 700;
    font-size: 13px;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 12px;
  }
  .sermon-title {
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 900;
    font-size: clamp(48px, 7vw, 90px);
    text-transform: uppercase;
    color: var(--ink);
    line-height: 0.95;
    letter-spacing: -0.01em;
    margin-bottom: 20px;
  }
  .sermon-title span {
    display: block;
    font-size: clamp(28px, 4vw, 52px);
    color: var(--muted);
    font-weight: 700;
  }
  .sermon-meta {
    display: flex;
    gap: 24px;
    font-size: 13px;
    color: var(--muted);
    letter-spacing: 0.08em;
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    text-transform: uppercase;
  }

  /* ── LAYOUT ── */
  .content-wrap {
    max-width: 860px;
    margin: 0 auto;
    padding: 48px 48px 80px;
  }

  /* ── SECTION HEADERS ── */
  .section-label {
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 700;
    font-size: 11px;
    letter-spacing: 0.3em;
    color: var(--muted);
    text-transform: uppercase;
    margin-bottom: 6px;
    margin-top: 52px;
  }
  .section-title {
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 900;
    font-size: 32px;
    text-transform: uppercase;
    color: var(--ink);
    margin-bottom: 20px;
    padding-bottom: 14px;
    border-bottom: 3px solid var(--ink);
    letter-spacing: 0.02em;
  }

  /* ── POINT HEADERS ── */
  .point-block {
    background: var(--wheat);
    border-radius: 4px;
    padding: 28px 32px;
    margin: 40px 0 20px;
    position: relative;
    overflow: hidden;
  }
  .point-block::after {
    content: attr(data-num);
    position: absolute;
    right: 20px; bottom: -20px;
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 900;
    font-size: 140px;
    color: rgba(0,0,0,0.06);
    line-height: 1;
  }
  .point-label {
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: 11px;
    letter-spacing: 0.25em;
    color: var(--ink-light);
    text-transform: uppercase;
    margin-bottom: 8px;
    opacity: 0.6;
  }
  .point-title {
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 900;
    font-size: clamp(22px, 3.5vw, 36px);
    text-transform: uppercase;
    color: var(--ink);
    line-height: 1.0;
    letter-spacing: 0.01em;
    position: relative;
    z-index: 1;
  }

  /* ── BODY TEXT ── */
  p { margin-bottom: 14px; color: var(--ink-light); }

  /* ── SCRIPTURE BOX ── */
  .scripture-box {
    background: var(--ice);
    border-left: 4px solid var(--ink);
    padding: 20px 24px;
    margin: 24px 0;
    border-radius: 0 4px 4px 0;
  }
  .scripture-ref {
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: 11px;
    letter-spacing: 0.25em;
    color: var(--muted);
    text-transform: uppercase;
    margin-bottom: 10px;
  }
  .scripture-text {
    font-size: 17px;
    color: var(--ink);
    line-height: 1.8;
    font-style: italic;
  }

  /* ── QUOTE BOX ── */
  .quote-box {
    background: var(--mint);
    border-radius: 4px;
    padding: 24px 28px;
    margin: 28px 0;
    position: relative;
  }
  .quote-text {
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 700;
    font-size: clamp(18px, 2.5vw, 24px);
    text-transform: uppercase;
    color: var(--ink);
    line-height: 1.3;
    margin-bottom: 12px;
    letter-spacing: 0.01em;
  }
  .quote-attr {
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: 13px;
    color: var(--ink-light);
    letter-spacing: 0.15em;
    text-transform: uppercase;
    opacity: 0.7;
  }

  /* ── ILLUSTRATION BOX ── */
  .illustration-box {
    background: white;
    border: 1px solid var(--ice-dark);
    border-radius: 4px;
    padding: 24px 28px;
    margin: 24px 0;
    position: relative;
  }
  .illustration-box::before {
    content: 'ILLUSTRATION';
    position: absolute;
    top: -1px; left: 20px;
    background: var(--wheat-dark);
    color: var(--ink);
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: 9px;
    letter-spacing: 0.2em;
    padding: 3px 10px;
    border-radius: 0 0 4px 4px;
  }
  .illustration-box p { margin-top: 10px; }

  /* ── APPLICATION BOX ── */
  .application-box {
    background: var(--ice);
    border-radius: 4px;
    padding: 20px 24px;
    margin: 24px 0;
  }
  .application-label {
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: 10px;
    letter-spacing: 0.25em;
    color: var(--muted);
    text-transform: uppercase;
    margin-bottom: 8px;
  }

  /* ── QUESTIONS BOX ── */
  .questions-box {
    background: var(--wheat);
    border-radius: 4px;
    padding: 24px 28px;
    margin: 24px 0;
  }
  .questions-label {
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: 10px;
    letter-spacing: 0.25em;
    color: var(--ink-light);
    text-transform: uppercase;
    margin-bottom: 14px;
    opacity: 0.6;
  }
  .questions-box ol { padding-left: 20px; }
  .questions-box li { margin-bottom: 10px; color: var(--ink-light); }

  /* ── DIVIDER ── */
  .divider {
    display: flex;
    align-items: center;
    gap: 16px;
    margin: 48px 0;
    color: var(--ice-dark);
  }
  .divider::before, .divider::after {
    content: '';
    flex: 1;
    height: 2px;
    background: var(--ice-dark);
  }
  .divider-mark {
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 900;
    font-size: 18px;
    color: var(--ice-dark);
    letter-spacing: 0.1em;
  }

  /* ── POSTURE TAG ── */
  .posture-recap {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin: 20px 0;
  }
  .posture-tag {
    background: var(--ice);
    border: 2px solid var(--ice-dark);
    border-radius: 3px;
    padding: 6px 14px;
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: 13px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--ink-light);
  }
  .posture-tag.highlight {
    background: var(--wheat);
    border-color: var(--wheat-dark);
  }

  /* ── SLIDES SECTION ── */
  .slides-section {
    background: var(--ink);
    padding: 60px 0;
    margin-top: 48px;
  }
  .slides-header {
    text-align: center;
    margin-bottom: 40px;
  }
  .slides-header h2 {
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: 13px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: rgba(255,255,255,0.4);
  }
  .slides-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(380px, 1fr));
    gap: 20px;
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 40px;
  }

  /* ── SLIDE BASE ── */
  .slide {
    position: relative;
    width: 100%;
    aspect-ratio: 16 / 9;
    overflow: hidden;
    border-radius: 3px;
  }
  .slide-inner {
    position: absolute;
    inset: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 40px 60px;
    text-align: center;
  }
  .s-ticker {
    position: absolute;
    top: 0; left: 0; right: 0;
    background: rgba(0,0,0,0.08);
    padding: 6px 16px;
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 700;
    font-size: clamp(7px, 1vw, 11px);
    letter-spacing: 0.08em;
    color: rgba(0,0,0,0.35);
    white-space: nowrap;
    overflow: hidden;
  }
  .s-figure { display: none; }
  .s-tag {
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 700;
    font-size: clamp(9px, 1.2vw, 13px);
    letter-spacing: 0.25em;
    text-transform: uppercase;
    margin-bottom: 12px;
    text-align: center;
  }
  .s-title {
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 900;
    text-transform: uppercase;
    text-align: center;
    line-height: 0.95;
    letter-spacing: 0.01em;
  }
  .s-sub {
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: clamp(10px, 1.4vw, 15px);
    letter-spacing: 0.08em;
    text-transform: uppercase;
    text-align: center;
    margin-top: 12px;
    opacity: 0.6;
  }
  .s-ghost {
    position: absolute;
    bottom: -10px; right: 10px;
    font-family: 'Barlow Condensed', Impact, sans-serif;
    font-weight: 900;
    font-size: clamp(60px, 12vw, 130px);
    color: rgba(0,0,0,0.06);
    line-height: 1;
    letter-spacing: -0.02em;
    text-transform: uppercase;
  }

  /* SLIDE COLOURS */
  .slide-ice { background: var(--ice); }
  .slide-ice .s-tag { color: var(--muted); }
  .slide-ice .s-title { color: var(--ink); }
  .slide-ice .s-sub { color: var(--ink); }
  .slide-wheat { background: var(--wheat); }
  .slide-wheat .s-tag { color: rgba(0,0,0,0.5); }
  .slide-wheat .s-title { color: var(--ink); }
  .slide-wheat .s-sub { color: var(--ink); }
  .slide-mint { background: var(--mint); }
  .slide-mint .s-tag { color: rgba(0,0,0,0.5); }
  .slide-mint .s-title { color: var(--ink); }
  .slide-mint .s-sub { color: rgba(0,0,0,0.6); }

  @media (max-width: 600px) {
    .content-wrap { padding: 32px 20px 60px; }
    .sermon-header { padding: 36px 20px 28px; }
    .slides-grid { grid-template-columns: 1fr; padding: 0 16px; }
  }
</style>
</head>
<body>

<!-- TICKER -->
<div class="ticker-wrap">
  <div class="ticker-text">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
</div>

<!-- HEADER -->
<div class="sermon-header">
  <div class="header-bg-text">Celebration</div>
  <div class="series-label">How's Your Posture? — Week 5 of 5</div>
  <div class="sermon-title">
    Celebration
    <span>The Act of Lifting Our Eyes</span>
  </div>
  <div class="sermon-meta">
    <span>New Life Community Church</span>
    <span>Week 5</span>
    <span>Nehemiah 8 · Philippians 4 · 2 Chronicles 20 · Luke 15</span>
  </div>
</div>

<!-- CONTENT -->
<div class="content-wrap">

  <!-- SERIES RECAP -->
  <div class="section-label">Series Recap</div>
  <div class="section-title">Five Postures</div>

  <p>We've spent five weeks examining Kingdom Principles — postures that, when practised, transform us from the inside out. Here's the full set:</p>

  <div class="posture-recap">
    <div class="posture-tag">🙇 Humility — Bowing the Head</div>
    <div class="posture-tag">⬆️ Availability — Leaning Forward</div>
    <div class="posture-tag">🤲 Generosity — Opening the Hands</div>
    <div class="posture-tag">🙏 Surrender — Bending the Knee</div>
    <div class="posture-tag highlight">👀 Celebration — Lifting the Eyes</div>
  </div>

  <p>Celebration isn't the reward for getting the other four right — it's the fuel that keeps them alive. This morning, before we even get into the teaching, let's do what this posture calls us to do.</p>

  <div class="application-box">
    <div class="application-label">Opening Moment</div>
    <p>Invite the worship team up. Before moving into the message, take a moment to genuinely celebrate — worship God for who He is and what He's done. Let celebration be the first act, not the closing one.</p>
  </div>

  <div class="divider"><span class="divider-mark">✦</span></div>

  <!-- INTRODUCTION -->
  <div class="section-label">Introduction</div>
  <div class="section-title">More Than Balloons</div>

  <p>When we hear the word "Celebration", most of us immediately think of balloons, party hats and a good time. And while a good time is not off the table, the Kingdom Principle of Celebration goes far deeper than that.</p>

  <p><strong>Celebration, biblically speaking, is not a response to life going well — it's a response to who God is, regardless of our circumstances.</strong></p>

  <p>Here's the opening question to sit with: <em>When did you last genuinely celebrate what God has done — not at the end of something hard, but in the middle of it?</em></p>

  <div class="divider"><span class="divider-mark">✦</span></div>

  <!-- POINT 1 -->
  <div class="point-block" data-num="01">
    <div class="point-label">Point 1</div>
    <div class="point-title">Celebration is a Commanded Discipline,<br>Not a Spontaneous Feeling</div>
  </div>

  <p>Celebration is not optional. It's not something we do when we feel like it — it's something God built into the rhythms of His people through festivals, feasts and occasions. It is mandated. It is commanded.</p>

  <div class="scripture-box">
    <div class="scripture-ref">Nehemiah 8:9–12</div>
    <div class="scripture-text">"Do not mourn or weep... Do not grieve, for the joy of the Lord is your strength... Then all the people went away to eat and drink, to send portions of food and to celebrate with great joy, because they now understood the words that had been made known to them."</div>
  </div>

  <p>The context here is remarkable. The Book of the Law is being read publicly for the first time in decades after the walls of Jerusalem have been rebuilt in just 52 days. The people begin to weep in repentance as they hear God's Word. And what does Nehemiah do? He stops them and tells them to celebrate.</p>

  <div class="illustration-box">
    <p><strong>Illustration — The Two Soldiers</strong></p>
    <p>Imagine two soldiers, fighting on the same side of a war. They win. One celebrates — he throws his helmet in the air, embraces his comrades, shouts with joy. The other trudges home in silence, head down. Both won. But only one clearly knows it. Celebration is the practice of knowing what has been done for you. The silent soldier has the same victory — he just hasn't allowed himself to receive it. Many of us are walking around with won battles we haven't celebrated yet.</p>
  </div>

  <div class="scripture-box">
    <div class="scripture-ref">Philippians 4:4</div>
    <div class="scripture-text">"Rejoice in the Lord always. I will say it again: rejoice!"</div>
  </div>

  <p>Paul writes this from prison. Not from a comfortable study. Not after a successful church planting campaign. From chains. The command to rejoice doesn't come with a condition attached — it comes with a repeat. He says it twice. <em>Rejoice. Rejoice.</em> As if the first one didn't quite land.</p>

  <div class="scripture-box">
    <div class="scripture-ref">Psalm 118:24</div>
    <div class="scripture-text">"This is the day the Lord has made; let us rejoice and be glad in it."</div>
  </div>

  <div class="quote-box">
    <div class="quote-text">"Celebration is central to all the Spiritual Disciplines… Joy makes us strong. Without joyous celebration to infuse the other Disciplines, we will sooner or later abandon them."</div>
    <div class="quote-attr">— Richard Foster, Celebration of Discipline</div>
  </div>

  <div class="application-box">
    <div class="application-label">Application</div>
    <p>Celebration is an act of trust and obedience — especially when it doesn't come naturally. It's not about pretending life is fine. It's about anchoring your joy in someone bigger than your circumstances. If we only celebrate when we feel like it, we will rarely celebrate at all.</p>
  </div>

  <div class="questions-box">
    <div class="questions-label">Reflection Questions — Point 1</div>
    <ol>
      <li>Is your celebration of God dependent on your circumstances? What would change if it wasn't?</li>
      <li>Are there victories in your life — answered prayers, moments of grace — that you haven't yet properly celebrated?</li>
      <li>What does it look like practically to rejoice "always"? What are the obstacles for you personally?</li>
    </ol>
  </div>

  <div class="divider"><span class="divider-mark">✦</span></div>

  <!-- POINT 2 -->
  <div class="point-block" data-num="02">
    <div class="point-label">Point 2</div>
    <div class="point-title">Celebration is a Weapon,<br>Not Just a Feeling</div>
  </div>

  <p>In the Kingdom of God, celebration doesn't always follow the victory — it can precede it. Celebration is an active posture of faith, and it is one of the most powerful weapons we carry. When the enemy comes, how do we face it? In fear? In anger? Or in the joyous confidence that our God is greater?</p>

  <div class="scripture-box">
    <div class="scripture-ref">2 Chronicles 20:15–22</div>
    <div class="scripture-text">"Do not be afraid or discouraged because of this vast army. For the battle is not yours, but God's... As they began to sing and praise, the Lord set ambushes against the men of Ammon and Moab and Mount Seir who were invading Judah, and they were defeated."</div>
  </div>

  <p>The context: Judah is surrounded and massively outnumbered. King Jehoshaphat doesn't form a military strategy. He seeks God, and then does something extraordinary — he appoints singers to go <em>ahead</em> of the army. Not behind. Not beside. In front. The praise goes first.</p>

  <div class="illustration-box">
    <p><strong>Illustration — Paul and Silas in Prison (Acts 16)</strong></p>
    <p>Paul and Silas are imprisoned, beaten and chained in the darkest part of the jail. What do they do? At midnight — the lowest hour — they sing. They don't wait for daylight. They don't wait for rescue. They sing in the darkness. And when they sang, an earthquake came and the prison doors flew open. Celebration in the darkest place has the power to open prison doors. This is not metaphor — this is spiritual reality. Your praise is not just an emotional response. It is a force.</p>
  </div>

  <div class="quote-box">
    <div class="quote-text">"Joy, which was the small publicity of the pagan, is the gigantic secret of the Christian."</div>
    <div class="quote-attr">— G.K. Chesterton</div>
  </div>

  <p>The world doesn't understand the kind of joy believers carry. It's jealous of it — because it can't manufacture it. You and I carry something the world desperately wants and cannot buy. Our celebration is a testimony. It is a weapon. It is a witness.</p>

  <p><em>Key question: Are you waiting until the battle is won to celebrate? Or are you willing to sing through it?</em></p>

  <div class="application-box">
    <div class="application-label">Application</div>
    <p>Your celebration right now — in whatever you're facing — is not denial of the difficulty. It is a declaration of who wins. When Jehoshaphat sent the singers ahead, it wasn't because the battle was already over. It was because he believed it would be. That's faith expressed as praise.</p>
  </div>

  <div class="questions-box">
    <div class="questions-label">Reflection Questions — Point 2</div>
    <ol>
      <li>What battle are you currently in the middle of? What would it look like to send "the singers ahead"?</li>
      <li>Have you ever experienced a situation where choosing to praise in a dark moment shifted something — in you or around you?</li>
      <li>What's the difference between fake positivity and genuine faith-filled celebration?</li>
    </ol>
  </div>

  <div class="divider"><span class="divider-mark">✦</span></div>

  <!-- POINT 3 -->
  <div class="point-block" data-num="03">
    <div class="point-label">Point 3</div>
    <div class="point-title">Celebration is the Fruit<br>of the Other Four Postures</div>
  </div>

  <p>Celebration isn't a standalone principle. It is the natural overflow — the fruit — of a life shaped by humility, availability, generosity and surrender. You can't manufacture deep, sustaining celebration without the other postures. It is what a Kingdom life looks like from the outside.</p>

  <div class="scripture-box">
    <div class="scripture-ref">Luke 15:11–32 — The Parable of the Prodigal Son</div>
    <div class="scripture-text">"We had to celebrate and be glad, because this brother of yours was dead and is alive again; he was lost and is found." (v.32)</div>
  </div>

  <p>Notice: the Father doesn't simply forgive — he throws a party. Celebration is the Father's instinct. When grace is grasped, celebration is unavoidable. And the elder brother's refusal to celebrate reveals a heart that hasn't yet grasped grace. His posture is completely wrong — rigid, proud, closed.</p>

  <p>In this one parable, all five postures appear:</p>

  <div class="posture-recap">
    <div class="posture-tag">Humility — the son's return and confession</div>
    <div class="posture-tag">Availability — the Father runs to meet him</div>
    <div class="posture-tag">Generosity — the robe, the ring, the feast</div>
    <div class="posture-tag">Surrender — "make me like one of your servants"</div>
    <div class="posture-tag highlight">Celebration — the party the Father throws</div>
  </div>

  <p>Where the other postures are present, celebration comes. It is not forced — it flows. And this is true in our own lives:</p>

  <p><strong>When we walk in Humility</strong> and recognise that God is God and we are not, we find things to celebrate in His goodness and sovereignty.</p>
  <p><strong>When we live in Availability</strong> and say yes before we know the full picture, we begin to see God move in ways we never would have — and that gives us more to celebrate.</p>
  <p><strong>When we practise Generosity</strong> and open our hands, we witness God's provision and faithfulness — and celebration grows.</p>
  <p><strong>When we move into Surrender</strong> and say "not my will but yours", we experience a freedom the world cannot offer — and that too is cause for celebration.</p>

  <div class="quote-box">
    <div class="quote-text">"I think we delight to praise what we enjoy because the praise not merely expresses but completes the enjoyment; it is its appointed consummation."</div>
    <div class="quote-attr">— C.S. Lewis</div>
  </div>

  <div class="illustration-box">
    <p><strong>Illustration — The Pianist</strong></p>
    <p>Think of a concert pianist. They spend hours alone in a practice room — drilling scales, working through difficult passages, perfecting their craft in obscurity. Nobody sees that work. Nobody applauds the 7am practice session. But when they step onto the stage and play, the audience receives the joy of all those private hours. The celebration is the public sound of a private life. For us, our celebration — our joy, our praise — is the sound of the time we've spent privately with God, for God, being shaped by God. The audience of your life is receiving the fruit of your posture.</p>
  </div>

  <div class="application-box">
    <div class="application-label">Application</div>
    <p>Celebration is not the starting point — it's the destination. If you're finding it hard to celebrate, the question isn't "why can't I praise?" The question is "which of the other four postures needs attention?" Celebration flows from the others. Work on your posture, and celebration will follow.</p>
  </div>

  <div class="questions-box">
    <div class="questions-label">Reflection Questions — Point 3</div>
    <ol>
      <li>Of the five postures — Humility, Availability, Generosity, Surrender, Celebration — which is most natural for you? Which is hardest?</li>
      <li>Where in your life is the elder brother's posture showing up — a refusal to celebrate because of pride, bitterness or comparison?</li>
      <li>What would it look like for New Life as a whole to be a church that publicly celebrates what God is doing privately?</li>
    </ol>
  </div>

  <div class="divider"><span class="divider-mark">✦</span></div>

  <!-- CONCLUSION -->
  <div class="section-label">Conclusion</div>
  <div class="section-title">Let Everything That Has Breath</div>

  <p>Psalm 150 ends the entire book of Psalms with a single command: <em>Let everything that has breath praise the Lord.</em> Not "let those who feel like it." Not "let those whose circumstances are good." Everything. That. Has. Breath.</p>

  <p>If you're breathing this morning, you have reason to celebrate.</p>

  <p>Over these five weeks, we've moved through five Kingdom Principles. My prayer is that they haven't just been ideas — but that God has been pressing on something real in each of you. Before we move into our AGM and lunch, let's close this series the way it deserves to close: not with a summary, but with a celebration.</p>

  <div class="application-box">
    <div class="application-label">Closing Response</div>
    <p>Invite the congregation to stand. Pray together. Let the celebration that began this service also close it. And carry the question into the week ahead:</p>
    <p><em>What in your life today can you celebrate and praise God for?</em></p>
  </div>

  <div class="divider"><span class="divider-mark">✦</span></div>

  <div style="background: var(--wheat); border-radius: 4px; padding: 24px 28px; margin-top: 40px;">
    <div class="questions-label">Preacher's Notes</div>
    <p style="color: var(--ink-light); font-size: 15px; margin-bottom: 8px;"><strong>Opening worship moment:</strong> Don't treat this as an add-on — build it into the structure of the sermon. Let the congregation celebrate before you teach about celebration.</p>
    <p style="color: var(--ink-light); font-size: 15px; margin-bottom: 8px;"><strong>AGM context:</strong> The transition into the AGM is actually a gift — celebration flows naturally into community. Frame the AGM itself as a moment of corporate celebration.</p>
    <p style="color: var(--ink-light); font-size: 15px;"><strong>Tone:</strong> Joyful and warm throughout. This is the series finale — it should feel like a party that has theological depth, not a theology lecture with a party at the end.</p>
  </div>

</div>

<!-- SLIDES SECTION -->
<div class="slides-section">
  <div class="slides-header">
    <h2>Service Slides — How's Your Posture? Week 5</h2>
  </div>
  <div class="slides-grid">

    <!-- SLIDE 1 — Title -->
    <div class="slide slide-ice">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div class="s-ghost">CELEBRATION</div>
      <div style="text-align:center; position:relative; z-index:1;">
        <div class="s-tag" style="color:var(--muted);">How's Your Posture? — Week 5</div>
        <div class="s-title" style="font-size:clamp(40px,8vw,80px); color:var(--ink);">HOW'S YOUR<br>POSTURE?</div>
        <div class="s-title" style="font-size:clamp(28px,5vw,52px); color:var(--muted); margin-top:6px;">CELEBRATION</div>
        <div class="s-sub">Five Kingdom Principles That Will Transform You</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 2 — Point 1 wheat -->
    <div class="slide slide-wheat">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div class="s-ghost">01</div>
      <div style="text-align:center; position:relative; z-index:1;">
        <div class="s-tag">Point 1</div>
        <div class="s-title" style="font-size:clamp(22px,4vw,44px);">CELEBRATION IS A<br>COMMANDED DISCIPLINE,<br>NOT A SPONTANEOUS FEELING</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 3 — Scripture Nehemiah ice -->
    <div class="slide slide-ice">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div style="text-align:center; position:relative; z-index:1; max-width:85%;">
        <div class="s-tag" style="color:var(--muted);">Nehemiah 8:10</div>
        <div class="s-title" style="font-size:clamp(16px,2.8vw,30px); font-weight:700; text-transform:uppercase; line-height:1.4;">"DO NOT GRIEVE, FOR THE<br>JOY OF THE LORD<br>IS YOUR STRENGTH."</div>
        <div class="s-sub">Nehemiah 8:10</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 4 — Richard Foster quote mint -->
    <div class="slide slide-mint">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div style="text-align:center; position:relative; z-index:1; max-width:88%;">
        <div class="s-tag">Quote</div>
        <div class="s-title" style="font-size:clamp(14px,2.2vw,24px); line-height:1.35;">"CELEBRATION IS CENTRAL TO ALL THE SPIRITUAL DISCIPLINES… JOY MAKES US STRONG. WITHOUT JOYOUS CELEBRATION TO INFUSE THE OTHER DISCIPLINES, WE WILL SOONER OR LATER ABANDON THEM."</div>
        <div class="s-sub" style="margin-top:16px; opacity:1;">RICHARD FOSTER</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 5 — Point 2 wheat -->
    <div class="slide slide-wheat">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div class="s-ghost">02</div>
      <div style="text-align:center; position:relative; z-index:1;">
        <div class="s-tag">Point 2</div>
        <div class="s-title" style="font-size:clamp(24px,4.5vw,50px);">CELEBRATION IS<br>A WEAPON, NOT<br>JUST A FEELING</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 6 — Scripture 2 Chron ice -->
    <div class="slide slide-ice">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div style="text-align:center; position:relative; z-index:1; max-width:85%;">
        <div class="s-tag" style="color:var(--muted);">2 Chronicles 20:22</div>
        <div class="s-title" style="font-size:clamp(15px,2.6vw,28px); font-weight:700; line-height:1.4;">"AS THEY BEGAN TO SING AND PRAISE, THE LORD SET AMBUSHES AGAINST THE ENEMY, AND THEY WERE DEFEATED."</div>
        <div class="s-sub">2 Chronicles 20:22</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 7 — GK Chesterton mint -->
    <div class="slide slide-mint">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div style="text-align:center; position:relative; z-index:1; max-width:88%;">
        <div class="s-tag">Quote</div>
        <div class="s-title" style="font-size:clamp(16px,2.8vw,30px); line-height:1.35;">"JOY, WHICH WAS THE SMALL PUBLICITY OF THE PAGAN, IS THE GIGANTIC SECRET OF THE CHRISTIAN."</div>
        <div class="s-sub" style="margin-top:16px; opacity:1;">G.K. CHESTERTON</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 8 — Point 3 wheat -->
    <div class="slide slide-wheat">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div class="s-ghost">03</div>
      <div style="text-align:center; position:relative; z-index:1;">
        <div class="s-tag">Point 3</div>
        <div class="s-title" style="font-size:clamp(22px,4vw,44px);">CELEBRATION IS THE<br>FRUIT OF THE<br>OTHER FOUR POSTURES</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 9 — CS Lewis mint -->
    <div class="slide slide-mint">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div style="text-align:center; position:relative; z-index:1; max-width:88%;">
        <div class="s-tag">Quote</div>
        <div class="s-title" style="font-size:clamp(14px,2.2vw,24px); line-height:1.35;">"I THINK WE DELIGHT TO PRAISE WHAT WE ENJOY BECAUSE THE PRAISE NOT MERELY EXPRESSES BUT COMPLETES THE ENJOYMENT; IT IS ITS APPOINTED CONSUMMATION."</div>
        <div class="s-sub" style="margin-top:16px; opacity:1;">C.S. LEWIS</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 10 — Closing question ice -->
    <div class="slide slide-ice">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div class="s-ghost">?</div>
      <div style="text-align:center; position:relative; z-index:1; max-width:85%;">
        <div class="s-tag" style="color:var(--muted);">Reflection</div>
        <div class="s-title" style="font-size:clamp(20px,3.5vw,38px);">WHAT IN YOUR LIFE TODAY CAN YOU CELEBRATE AND PRAISE GOD FOR?</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 11 — Psalm 150 ice -->
    <div class="slide slide-ice">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div style="text-align:center; position:relative; z-index:1; max-width:85%;">
        <div class="s-tag" style="color:var(--muted);">Psalm 150:6</div>
        <div class="s-title" style="font-size:clamp(28px,5vw,56px);">"LET EVERYTHING<br>THAT HAS BREATH<br>PRAISE THE LORD."</div>
        <div class="s-sub">Psalm 150:6</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

    <!-- SLIDE 12 — Series close wheat -->
    <div class="slide slide-wheat">
      <div class="s-ticker">FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU. &nbsp;&nbsp;&nbsp; FIVE KINGDOM PRINCIPLES THAT WILL TRANSFORM YOU.</div>
      <div class="s-ghost">HYP</div>
      <div style="text-align:center; position:relative; z-index:1;">
        <div class="s-tag">Series Complete</div>
        <div class="s-title" style="font-size:clamp(32px,6vw,64px);">HOW'S YOUR<br>POSTURE?</div>
        <div class="s-sub">Five Kingdom Principles That Will Transform You</div>
      </div>
      <div class="s-figure">🧘</div>
    </div>

  </div>
</div>

</body>
</html>
