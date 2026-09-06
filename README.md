<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
  :root{color-scheme:light dark}
  html,body{margin:0}
  img{max-width:100%}
  [hidden]{display:none!important}
</style>
</head>
<body>
<title>AP Lit in 77 Days</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@400;500&family=IBM+Plex+Sans:ital,wght@0,400;0,500;0,600;1,400&family=Spectral:ital,wght@0,500;0,600;0,700;1,500&display=swap">
<style>
:root{
  --bg:#EDEFF3; --surface:#FFFFFF; --surface-2:#F4F6FA; --surface-3:#E5E9F0;
  --ink:#13171E; --ink-2:#4B5462; --ink-3:#7C8494;
  --rule:#D6DBE3; --rule-2:#E6EAF0;
  --accent:#8E2F3B;
  --u-launch:#5C6B7A; --u-fiction:#3F6B8F; --u-poetry:#8F6716;
  --u-frank:#1F6C68; --u-nlmg:#576B36; --u-hamlet:#8E2F3B; --u-review:#574691;
  --shadow:0 1px 2px rgba(19,23,30,.05), 0 6px 18px -12px rgba(19,23,30,.28);
  --serif:"Spectral",Georgia,"Times New Roman",serif;
  --sans:"IBM Plex Sans",-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
  --mono:"IBM Plex Mono",ui-monospace,SFMono-Regular,Menlo,monospace;
}
@media (prefers-color-scheme: dark){
  :root:not([data-theme="light"]){
    --bg:#0F1217; --surface:#171B22; --surface-2:#1E232B; --surface-3:#262C36;
    --ink:#E7EAEF; --ink-2:#A6AEBC; --ink-3:#6F7887;
    --rule:#2A303A; --rule-2:#222831;
    --accent:#D9808B;
    --u-launch:#8FA1B3; --u-fiction:#7FAACB; --u-poetry:#D7AE5C;
    --u-frank:#62B8B2; --u-nlmg:#A3B978; --u-hamlet:#D9808B; --u-review:#9B8AD6;
    --shadow:0 1px 2px rgba(0,0,0,.4), 0 8px 24px -14px rgba(0,0,0,.7);
  }
}
:root[data-theme="dark"]{
  --bg:#0F1217; --surface:#171B22; --surface-2:#1E232B; --surface-3:#262C36;
  --ink:#E7EAEF; --ink-2:#A6AEBC; --ink-3:#6F7887;
  --rule:#2A303A; --rule-2:#222831;
  --accent:#D9808B;
  --u-launch:#8FA1B3; --u-fiction:#7FAACB; --u-poetry:#D7AE5C;
  --u-frank:#62B8B2; --u-nlmg:#A3B978; --u-hamlet:#D9808B; --u-review:#9B8AD6;
  --shadow:0 1px 2px rgba(0,0,0,.4), 0 8px 24px -14px rgba(0,0,0,.7);
}

*{box-sizing:border-box}
body{
  background:var(--bg); color:var(--ink);
  font-family:var(--sans); font-size:15px; line-height:1.55;
  -webkit-font-smoothing:antialiased;
}
.wrap{max-width:1060px; margin:0 auto; padding:0 24px 96px}
h1,h2,h3{font-family:var(--serif); font-weight:600; text-wrap:balance; margin:0}
a{color:var(--accent)}
:focus-visible{outline:2px solid var(--accent); outline-offset:2px; border-radius:3px}
@media (prefers-reduced-motion: reduce){*{animation:none!important; transition:none!important}}

/* ---------- masthead ---------- */
.mast{padding:52px 0 30px; border-bottom:1px solid var(--rule)}
.eyebrow{
  font-family:var(--mono); font-size:11.5px; letter-spacing:.13em;
  text-transform:uppercase; color:var(--ink-3); margin:0 0 14px
}
.mast h1{font-size:clamp(38px,6.2vw,60px); line-height:1.02; letter-spacing:-.018em}
.mast h1 em{font-style:italic; color:var(--accent); font-weight:500}
.standfirst{
  margin:16px 0 0; max-width:62ch; font-size:16.5px; color:var(--ink-2);
}
.facts{
  display:flex; flex-wrap:wrap; gap:0; margin-top:30px;
  border-top:1px solid var(--rule-2);
}
.fact{
  flex:1 1 150px; padding:14px 18px 12px; border-right:1px solid var(--rule-2);
}
.fact:last-child{border-right:0}
.fact dt{
  font-family:var(--mono); font-size:10.5px; letter-spacing:.11em;
  text-transform:uppercase; color:var(--ink-3); margin:0 0 5px
}
.fact dd{
  margin:0; font-family:var(--mono); font-size:20px; font-weight:500;
  font-variant-numeric:tabular-nums; color:var(--ink); line-height:1.2
}
.fact dd small{font-size:12.5px; color:var(--ink-2); font-weight:400; display:block; margin-top:3px; font-family:var(--sans); letter-spacing:0}

/* ---------- section headings ---------- */
.sec{margin-top:56px}
.sec-head{display:flex; align-items:baseline; justify-content:space-between; gap:20px; flex-wrap:wrap; margin-bottom:6px}
.sec h2{font-size:25px; letter-spacing:-.01em}
.sec-note{font-size:13.5px; color:var(--ink-3); max-width:52ch}

/* ---------- budget bar ---------- */
.budget{display:flex; width:100%; height:44px; border-radius:4px; overflow:hidden; margin-top:20px; background:var(--surface-2)}
.budget-seg{
  border:0; padding:0; cursor:pointer; position:relative;
  font-family:var(--mono); font-size:12px; font-weight:600; color:var(--bg);
  display:flex; align-items:center; justify-content:center;
  transition:filter .15s ease, opacity .15s ease;
}
.budget-seg + .budget-seg{border-left:1px solid var(--bg)}
.budget-seg:hover{filter:brightness(1.12)}
.budget-seg[aria-pressed="false"].dimmed{opacity:.28}
.budget-seg span{letter-spacing:.04em}

/* ---------- unit legend / filters ---------- */
.legend{
  display:grid; grid-template-columns:repeat(auto-fill,minmax(232px,1fr));
  gap:8px; margin-top:14px;
}
.ubtn{
  display:grid; grid-template-columns:auto 1fr auto; align-items:center; gap:11px;
  text-align:left; background:var(--surface); border:1px solid var(--rule);
  border-radius:5px; padding:11px 13px; cursor:pointer; font-family:var(--sans);
  color:var(--ink); transition:border-color .15s ease, background .15s ease;
}
.ubtn:hover{border-color:var(--uc)}
.ubtn[aria-pressed="true"]{border-color:var(--uc); background:var(--surface-2); box-shadow:inset 3px 0 0 var(--uc)}
.ubtn .swatch{width:10px; height:10px; border-radius:2px; background:var(--uc)}
.ubtn .un{font-family:var(--serif); font-weight:600; font-size:15px; line-height:1.2; display:block}
.ubtn .us{font-size:11.5px; color:var(--ink-3); line-height:1.35; display:block; margin-top:2px}
.ubtn .uc{font-family:var(--mono); font-size:15px; font-variant-numeric:tabular-nums; color:var(--uc); font-weight:500}
.ubtn .uc small{display:block; font-size:9.5px; letter-spacing:.08em; text-transform:uppercase; color:var(--ink-3)}

.toolbar{display:flex; gap:10px; flex-wrap:wrap; align-items:center; margin-top:16px}
.tbtn{
  font-family:var(--mono); font-size:11.5px; letter-spacing:.06em; text-transform:uppercase;
  background:var(--surface); border:1px solid var(--rule); color:var(--ink-2);
  padding:8px 13px; border-radius:4px; cursor:pointer;
}
.tbtn:hover{border-color:var(--ink-3); color:var(--ink)}
.tbtn[aria-pressed="true"]{background:var(--ink); color:var(--bg); border-color:var(--ink)}
.showing{font-family:var(--mono); font-size:12px; color:var(--ink-3); font-variant-numeric:tabular-nums; margin-left:auto}

/* ---------- schedule ---------- */
.week{margin-top:34px}
.week-bar{
  display:flex; align-items:baseline; gap:12px; padding-bottom:8px;
  border-bottom:1px solid var(--rule); margin-bottom:10px;
}
.week-n{
  font-family:var(--mono); font-size:11px; letter-spacing:.12em; text-transform:uppercase;
  color:var(--ink-3);
}
.week-r{font-family:var(--serif); font-size:17px; font-weight:600; color:var(--ink)}
.week-c{margin-left:auto; font-family:var(--mono); font-size:11px; color:var(--ink-3)}

.day{
  display:grid; grid-template-columns:78px 1fr; gap:0;
  background:var(--surface); border:1px solid var(--rule-2); border-left:3px solid var(--uc);
  border-radius:4px; margin-bottom:7px; box-shadow:var(--shadow);
}
.day-mark{
  padding:14px 8px 14px 14px; border-right:1px solid var(--rule-2);
  display:flex; flex-direction:column; gap:2px;
}
.day-n{font-family:var(--mono); font-size:19px; font-weight:500; color:var(--uc); font-variant-numeric:tabular-nums; line-height:1}
.day-d{font-family:var(--mono); font-size:11px; color:var(--ink-3); line-height:1.35}
.day-body{padding:13px 16px 14px}
.day-t{font-family:var(--serif); font-size:18px; font-weight:600; line-height:1.25; letter-spacing:-.005em}
.day-x{margin:6px 0 0; color:var(--ink-2); font-size:14.5px; max-width:72ch}
.day-meta{display:flex; flex-wrap:wrap; gap:7px; margin-top:11px; align-items:center}

.chip{
  font-family:var(--mono); font-size:10.5px; letter-spacing:.05em;
  padding:4px 8px; border-radius:3px; white-space:nowrap;
}
.chip-read{background:var(--surface-2); color:var(--ink-2); border:1px solid var(--rule-2); white-space:normal}
.chip-read b{font-weight:500; color:var(--ink-3); letter-spacing:.09em; text-transform:uppercase; font-size:9.5px; margin-right:5px}
.chip-poem{
  background:transparent; color:var(--u-poetry); border:1px dashed color-mix(in srgb, var(--u-poetry) 45%, transparent);
  white-space:normal; font-family:var(--sans); font-size:12px; font-style:italic; letter-spacing:0;
}
.chip-poem b{font-family:var(--mono); font-style:normal; font-size:9.5px; letter-spacing:.09em; text-transform:uppercase; margin-right:6px; color:var(--ink-3); font-weight:500}
.chip-story{
  background:transparent; color:var(--u-fiction);
  border:1px solid color-mix(in srgb, var(--u-fiction) 42%, transparent);
  white-space:normal; font-family:var(--sans); font-size:12px; letter-spacing:0;
}
.chip-story.echo{border-style:dashed; opacity:.85}
.chip-story b{font-family:var(--mono); font-size:9.5px; letter-spacing:.09em; text-transform:uppercase; margin-right:6px; color:var(--ink-3); font-weight:500}
.chip-story i{font-style:italic}
.chip-story em{font-style:normal; color:var(--ink-3); font-size:11px}
.chip-frq{
  background:color-mix(in srgb, var(--uc) 13%, transparent); color:var(--uc);
  border:1px solid color-mix(in srgb, var(--uc) 38%, transparent); font-weight:500;
  white-space:normal;
}
.chip-mcq{background:var(--surface-2); color:var(--ink-2); border:1px solid var(--rule); white-space:normal}
.chip-task{background:transparent; color:var(--ink-2); border:1px dotted var(--rule); white-space:normal}

.brk{
  display:flex; align-items:center; gap:14px; margin:9px 0 2px; padding:9px 14px;
  border:1px dashed var(--rule); border-radius:4px; background:transparent;
}
.brk-l{font-family:var(--mono); font-size:11px; letter-spacing:.11em; text-transform:uppercase; color:var(--ink-3)}
.brk-d{font-family:var(--serif); font-size:15px; font-style:italic; color:var(--ink-2)}
.brk-t{margin-left:auto; font-family:var(--mono); font-size:10.5px; color:var(--ink-3)}

.examday{
  margin-top:22px; padding:22px 24px; border-radius:5px;
  background:var(--ink); color:var(--bg);
  display:flex; align-items:center; gap:22px; flex-wrap:wrap;
}
.examday .ed-n{font-family:var(--mono); font-size:11px; letter-spacing:.14em; text-transform:uppercase; opacity:.7}
.examday .ed-t{font-family:var(--serif); font-size:24px; font-weight:600; line-height:1.15}
.examday .ed-s{font-family:var(--mono); font-size:12.5px; opacity:.75; margin-left:auto; text-align:right; line-height:1.6}

/* ---------- reference tables ---------- */
.panel{
  background:var(--surface); border:1px solid var(--rule-2); border-radius:5px;
  padding:22px 24px; margin-top:16px; box-shadow:var(--shadow);
}
.tw{overflow-x:auto; margin:0 -4px}
table{border-collapse:collapse; width:100%; font-size:14px; min-width:520px}
th{
  text-align:left; font-family:var(--mono); font-size:10.5px; letter-spacing:.1em;
  text-transform:uppercase; color:var(--ink-3); font-weight:500;
  padding:0 14px 9px 0; border-bottom:1px solid var(--rule); white-space:nowrap;
}
td{padding:10px 14px 10px 0; border-bottom:1px solid var(--rule-2); vertical-align:top; color:var(--ink-2)}
tr:last-child td{border-bottom:0}
td.k{color:var(--ink); font-weight:500}
td.m{font-family:var(--mono); font-variant-numeric:tabular-nums; white-space:nowrap; font-size:13px}
td.u{font-family:var(--mono); font-size:12px; color:var(--uc); white-space:nowrap}
cite{font-style:italic; font-family:var(--serif)}

.note{
  border-left:3px solid var(--accent); background:var(--surface-2);
  padding:16px 20px; border-radius:0 4px 4px 0; margin-top:16px;
}
.note h3{font-size:16px; margin-bottom:6px}
.note p{margin:0 0 10px; color:var(--ink-2); font-size:14px; max-width:70ch}
.note p:last-child{margin-bottom:0}
.note ul{margin:0; padding-left:18px; color:var(--ink-2); font-size:14px}
.note li{margin-bottom:5px}
.note li:last-child{margin-bottom:0}

.foot{margin-top:60px; padding-top:20px; border-top:1px solid var(--rule); font-size:12.5px; color:var(--ink-3); display:flex; gap:18px; flex-wrap:wrap}
.foot a{color:var(--ink-3)}

@media (max-width:640px){
  .wrap{padding:0 16px 72px}
  .mast{padding:36px 0 24px}
  .fact{flex:1 1 45%; border-right:0}
  .day{grid-template-columns:1fr}
  .day-mark{flex-direction:row; align-items:baseline; gap:10px; border-right:0; border-bottom:1px solid var(--rule-2); padding:10px 14px}
  .budget{height:34px}
  .budget-seg span{font-size:10px}
}
</style>

<div class="wrap">

<header class="mast">
  <p class="eyebrow">Spring 2027 &middot; 90-minute daily block &middot; Rockingham County Schools</p>
  <h1>AP&nbsp;Lit in <em>77&nbsp;Days</em></h1>
  <p class="standfirst">One semester, three major works, and every minute of the textbook's first three chapters spent where it earns something on May 5. This is the whole plan, day by day — filter it, argue with it, cut from it when the snow days come.</p>
  <dl class="facts">
    <div class="fact"><dt>Semester</dt><dd>Jan 6<small>through May 28</small></dd></div>
    <div class="fact"><dt>Class days to exam</dt><dd>77<small>Jan 6 &ndash; May 4</small></dd></div>
    <div class="fact"><dt>Instructional time</dt><dd>115.5<small>hours, at 90 min/day</small></dd></div>
    <div class="fact"><dt>Graded timed writes</dt><dd>10<small>plus 2 diagnostics</small></dd></div>
    <div class="fact"><dt>Short stories</dt><dd>8<small>6 taught in January</small></dd></div>
    <div class="fact"><dt>AP Exam</dt><dd>May 5<small>Wednesday, 8 a.m.</small></dd></div>
  </dl>
</header>

<section class="sec" id="budget">
  <div class="sec-head">
    <h2>Where the days go</h2>
    <p class="sec-note">Seventy-seven days is the entire budget. Click a unit to filter the calendar below.</p>
  </div>
  <div class="budget" id="bar" role="group" aria-label="Filter schedule by unit"></div>
  <div class="legend" id="legend"></div>
  <div class="toolbar">
    <button class="tbtn" id="btn-all" aria-pressed="true">All 77 days</button>
    <button class="tbtn" id="btn-assess" aria-pressed="false">Assessment days only</button>
    <button class="tbtn" id="btn-poem" aria-pressed="false">Poetry anchors only</button>
    <button class="tbtn" id="btn-story" aria-pressed="false">Short story days only</button>
    <span class="showing" id="showing"></span>
  </div>
</section>

<section class="sec" id="schedule">
  <div class="sec-head">
    <h2>The calendar</h2>
    <p class="sec-note">Reading listed on a day is assigned <em>that night</em>, due the next class.</p>
  </div>
  <div id="weeks"></div>
  <div class="examday">
    <div>
      <div class="ed-n">Wednesday, May 5, 2027</div>
      <div class="ed-t">AP English Literature &amp; Composition Exam</div>
    </div>
    <div class="ed-s">55 multiple-choice &middot; 60 min &middot; 45%<br>3 free-response &middot; 120 min &middot; 55%</div>
  </div>
</section>

<section class="sec" id="textbook">
  <div class="sec-head">
    <h2>How the textbook carries the course</h2>
    <p class="sec-note">Chapters 1 and 2 are taught whole, up front. Chapter 3 is deliberately split so each section arrives attached to the work that needs it.</p>
  </div>
  <div class="panel"><div class="tw"><table>
    <thead><tr><th>Chapter &amp; section</th><th>What it teaches</th><th>Where it lands</th><th>Days</th></tr></thead>
    <tbody>
      <tr><td class="k">Ch. 1 §1 — Literary Elements</td><td>Character, setting, plot, narrative perspective in short fiction</td><td>Short Fiction unit, Jan 8&ndash;14</td><td class="m">5</td></tr>
      <tr><td class="k">Ch. 1 §2 — Close Reading &amp; Writing</td><td>Diction, syntax, figurative language, tone; the Q2 prose essay</td><td>Short Fiction unit, Jan 15&ndash;22</td><td class="m">5</td></tr>
      <tr><td class="k">Ch. 1 §3 — Sophistication</td><td>Complexity, tension, qualified argument</td><td>Jan 25 &mdash; then reused in every revision cycle</td><td class="m">1</td></tr>
      <tr><td class="k">Ch. 2 §1 — Reading &amp; Analyzing</td><td>Paraphrase, speaker, contrast, image, structure, sound</td><td>Poetry unit, Jan 26 &ndash; Feb 3</td><td class="m">7</td></tr>
      <tr><td class="k">Ch. 2 §2 — Writing Analysis</td><td>The Q1 poetry essay, organizer to thesis to evidence</td><td>Poetry unit, Feb 4&ndash;8</td><td class="m">3</td></tr>
      <tr><td class="k">Ch. 2 §3 — Sophistication</td><td>Situating a reading in broader context; qualification</td><td>Poetry unit, Feb 9&ndash;10</td><td class="m">2</td></tr>
      <tr><td class="k">Ch. 3 §1 — Literary Elements</td><td>Character, setting, layered narration, symbol and allegory <em>at novel length</em></td><td>Taught through <cite>Frankenstein</cite>, Feb 12 &ndash; Mar 2</td><td class="m">5</td></tr>
      <tr><td class="k">Ch. 3 §2 — Literary Arguments</td><td>Summary to interpretation, thesis, topic sentences, interpretive commentary</td><td>Taught through <cite>Never Let Me Go</cite>, Mar 12&ndash;23</td><td class="m">4</td></tr>
      <tr><td class="k">Ch. 3 §3 — Sophistication</td><td>Critical lenses; incorporating and answering alternative interpretations</td><td>Taught through <cite>Hamlet</cite>, Apr 14&ndash;20</td><td class="m">3</td></tr>
    </tbody>
  </table></div></div>
  <div class="note">
    <h3>Why Chapter 3 is split three ways</h3>
    <p>Read straight through, Chapter 3 is a survey with nothing to practice on. Split, each section becomes the reason a novel is on the syllabus: <cite>Frankenstein</cite>'s nested narrators make §1's material on layered perspective concrete; <cite>Never Let Me Go</cite> is the cleanest possible case for §2's move from summary to interpretation, because summarizing it is almost impossible without interpreting it; and <cite>Hamlet</cite> is the text with the longest critical argument attached to it, which is exactly what §3's work on competing interpretations needs.</p>
  </div>
</section>

<section class="sec" id="stories">
  <div class="sec-head">
    <h2>The short-story spine</h2>
    <p class="sec-note">Six stories carry the January skills unit, each doing one job. Two are held back to open a novel. Five come back later, which is the point.</p>
  </div>
  <div class="panel"><div class="tw"><table>
    <thead><tr><th>Story</th><th>Taught</th><th>The job it does</th><th>Returns</th></tr></thead>
    <tbody>
      <tr><td class="k">&ldquo;Where Are You Going, Where Have You Been?&rdquo;<br><span style="color:var(--ink-3)">Joyce Carol Oates, 1966</span></td><td class="m">Jan 8 &middot; Day 3</td><td>Character built entirely from surface. Connie&rsquo;s two selves and Arnold Friend&rsquo;s stuffed boots leave inference as the only route in.</td><td class="m">Jan 25 &mdash; the unresolved ending as a Row C exhibit</td></tr>
      <tr><td class="k">&ldquo;The Yellow Wallpaper&rdquo;<br><span style="color:var(--ink-3)">Charlotte Perkins Gilman, 1892</span></td><td class="m">Jan 11 &middot; Day 4</td><td>Setting as agent. The room stops being where the story happens and becomes what it is about. Also the semester&rsquo;s first pre-1900 prose.</td><td class="m">Jan 19 &mdash; image into symbol<br>Feb 26 &mdash; <cite>Frankenstein</cite>&rsquo;s women</td></tr>
      <tr><td class="k">&ldquo;A Good Man Is Hard to Find&rdquo;<br><span style="color:var(--ink-3)">Flannery O&rsquo;Connor, 1953</span></td><td class="m">Jan 12 &middot; Day 5</td><td>Plot as arrangement. The Misfit is planted in paragraph one; twenty pages are spent staging the collision.</td><td class="m">Jan 20 &mdash; thesis workshop<br>Feb 25 &mdash; the Misfit beside Victor</td></tr>
      <tr><td class="k">&ldquo;Playing Metal Gear Solid V: The Phantom Pain&rdquo;<br><span style="color:var(--ink-3)">Jamil Jan Kochai, 2020</span></td><td class="m">Jan 13 &middot; Day 6</td><td>Second person &mdash; the rarest narration on the AP exam and the hardest to find taught well.</td><td class="m">Apr 6 &mdash; the son, the lost father, the replay</td></tr>
      <tr><td class="k">&ldquo;Erasure&rdquo;<br><span style="color:var(--ink-3)">Sakinah Hofler, 2020</span></td><td class="m">Jan 13 &middot; Day 6</td><td>First-person plural. A collective office &ldquo;we&rdquo; watches its colleagues vanish and does nothing &mdash; witness and accomplice in one pronoun.</td><td class="m">Jan 25 &mdash; the Row C clinic&rsquo;s best example</td></tr>
      <tr><td class="k">&ldquo;Sonny&rsquo;s Blues&rdquo;<br><span style="color:var(--ink-3)">James Baldwin, 1957</span></td><td class="m">Jan 14 &middot; Day 7</td><td>The §1 culminating text, because it holds every element at once &mdash; and the narrator is a character who is wrong about things.</td><td class="m">Jan 15 &mdash; syntax<br>Jan 19 &mdash; allusion</td></tr>
      <tr><td class="k">&ldquo;The Ones Who Walk Away from Omelas&rdquo;<br><span style="color:var(--ink-3)">Ursula K. Le Guin, 1973</span></td><td class="m">Mar 8 &middot; Day 42</td><td>Held back to launch <cite>Never Let Me Go</cite>. Le Guin states the bargain plainly in five pages; Ishiguro spends 288 never stating it.</td><td class="m">Mar 22 &mdash; the paired seminar</td></tr>
      <tr><td class="k">&ldquo;Lulu&rdquo;<br><span style="color:var(--ink-3)">Te-Ping Chen, 2021</span></td><td class="m">Mar 15 &middot; Day 47</td><td>Held back for the Cottages. At Hailsham nobody leaves; Lulu speaks, and the brother who stays home narrates what it costs her.</td><td class="m">&mdash;</td></tr>
    </tbody>
  </table></div></div>
  <div class="note">
    <h3>Why five of them come back</h3>
    <p>A story taught once in January is a story students have read. A story that reappears in February beside <cite>Frankenstein</cite>, and again in April beside <cite>Hamlet</cite>, becomes something they can think with &mdash; and, on May 5, something they can reach for when a Question 3 prompt catches them off guard. The returns cost about ten minutes of class each; they are marked <strong>Story echo</strong> on the calendar and require rereading a few pages, not a whole text.</p>
    <p>Two notes on sourcing: Chen&rsquo;s &ldquo;Lulu&rdquo; is in <cite>Land of Big Numbers</cite> (2021), Hofler&rsquo;s &ldquo;Erasure&rdquo; is free at <em>Kenyon Review Online</em>, and Kochai&rsquo;s story is in <cite>The Haunting of Hajji Hotak</cite> and was first published in <em>The New Yorker</em>. Where your edition of the textbook already prints one of these, teach from the book so students have the apparatus.</p>
  </div>
</section>

<section class="sec" id="reading">
  <div class="sec-head">
    <h2>Reading load</h2>
    <p class="sec-note">Homework nights exclude timed-write days, seminar days, and the day a work is finished.</p>
  </div>
  <div class="panel"><div class="tw"><table>
    <thead><tr><th>Work</th><th>Class days</th><th>Reading nights</th><th>Per night</th><th>Read where</th></tr></thead>
    <tbody>
      <tr><td class="k"><cite>Frankenstein</cite> <span style="color:var(--ink-3)">(Shelley)</span></td><td class="m">16</td><td class="m">12</td><td class="m">≈2 chapters / 18 pp</td><td>At home; discussed in class</td></tr>
      <tr><td class="k"><cite>Never Let Me Go</cite> <span style="color:var(--ink-3)">(Ishiguro)</span></td><td class="m">14</td><td class="m">10</td><td class="m">≈2 chapters / 28 pp</td><td>At home; discussed in class</td></tr>
      <tr><td class="k"><cite>Hamlet</cite> <span style="color:var(--ink-3)">(Shakespeare)</span></td><td class="m">15</td><td class="m">6</td><td class="m">≈1 scene, reread</td><td>Read aloud in class; scenes reread at home</td></tr>
      <tr><td class="k">Short fiction &amp; poetry</td><td class="m">25</td><td class="m">18</td><td class="m">1 story or 2&ndash;3 poems</td><td>At home, always with the textbook section</td></tr>
    </tbody>
  </table></div></div>
</section>

<section class="sec" id="assessments">
  <div class="sec-head">
    <h2>Assessment ledger</h2>
    <p class="sec-note">Every timed and graded piece, in order. Ten graded timed writes and seven multiple-choice administrations before the exam.</p>
  </div>
  <div class="panel"><div class="tw"><table>
    <thead><tr><th>Date</th><th>Day</th><th>Unit</th><th>Assessment</th></tr></thead>
    <tbody id="ledger"></tbody>
  </table></div></div>
</section>

<section class="sec" id="assumptions">
  <div class="sec-head">
    <h2>Before you commit to this</h2>
    <p class="sec-note">Two things to check, and a plan for the days you will inevitably lose.</p>
  </div>
  <div class="note">
    <h3>Non-instructional days I assumed</h3>
    <p>The district's 2026&ndash;27 calendar confirms the semester runs to <strong>May 28</strong>, but the printed PDF did not give legible spring holiday dates. These four are assumptions — verify each against the official calendar, and the day count will shift accordingly.</p>
    <ul>
      <li><strong>Mon Jan 18</strong> — MLK Day</li>
      <li><strong>Mon Feb 15</strong> — Presidents Day / teacher workday</li>
      <li><strong>Fri Mar 26</strong> — Good Friday <span style="color:var(--ink-3)">(Easter falls Mar 28, 2027)</span></li>
      <li><strong>Mon Mar 29 &ndash; Fri Apr 2</strong> — Spring Break</li>
    </ul>
  </div>
  <div class="note">
    <h3>What to cut first, in order</h3>
    <p>Assume you lose five days to weather, assemblies, and testing. Cut in this sequence and the exam preparation survives intact:</p>
    <ul>
      <li><strong>First:</strong> one <cite>Frankenstein</cite> discussion day (combine Ch. 19&ndash;20 with Ch. 21&ndash;22) and one <cite>Hamlet</cite> day (fold Act IV, i&ndash;iv into the Act IV, v&ndash;vii class).</li>
      <li><strong>Second:</strong> the untimed Ch. 3 §2 culminating essay on Mar 23 — the timed Q3 the next day covers the same skill under real conditions.</li>
      <li><strong>Third:</strong> the Mar 22 paired seminar, moved to a graded written response instead.</li>
      <li><strong>Never cut:</strong> the seven review days, the three timed Q3s, or the two full-length multiple-choice sections. Those are the plan.</li>
    </ul>
  </div>
  <div class="note">
    <h3>After the exam — 17 days left</h3>
    <p>May 6 through May 28 is roughly seventeen class days with no exam pressure and seniors already gone in spirit. The plan that works: a self-selected novel from the AP Question 3 list, read independently with a weekly conference, ending in a staged or recorded scene and a five-minute defense of one interpretive choice. It uses everything the semester built and requires almost no new preparation from you.</p>
  </div>
</section>

<footer class="foot">
  <span>Pacing guide drafted for Matthew Alcorn &middot; AP English Literature &amp; Composition &middot; Spring 2027</span>
  <span>Textbook: <cite>Literature &amp; Composition: Essential Voices, Essential Skills for the AP Course</cite>, 3rd ed. (Bedford/St. Martin's)</span>
</footer>

</div>

<script>
const DATA = {"days": [{"n": 1, "iso": "2027-01-06", "dow": "Wed", "md": "Jan 6", "wk": "2027-01-04", "u": "launch", "t": "What the exam actually asks", "d": "Reverse-engineer the test before touching a text: 55 multiple-choice items in 60 minutes (45% of the score) and three free-response essays in 120 minutes (55%). Walk the three scoring rows — thesis, evidence and commentary, sophistication — and post them permanently.", "r": "Syllabus + course contract. Skim the AP Literature rubric.", "p": null, "a": [{"k": "mcq", "l": "Diagnostic MCQ · 11 items · 15 min · ungraded"}], "s": []}, {"n": 2, "iso": "2027-01-07", "dow": "Thu", "md": "Jan 7", "wk": "2027-01-04", "u": "launch", "t": "Baseline timed write", "d": "A cold 40-minute prose analysis with no instruction beforehand. Then students score two anonymous sample responses against Row A only. The goal is for every student to see, on day two, the exact gap between what they wrote and what a defensible thesis looks like.", "r": "Read Joyce Carol Oates, “Where Are You Going, Where Have You Been?”", "p": null, "a": [{"k": "frq", "l": "Diagnostic Q2 · 40 min · feedback only"}], "s": []}, {"n": 3, "iso": "2027-01-08", "dow": "Fri", "md": "Jan 8", "wk": "2027-01-04", "u": "fiction", "t": "Character: traits, motives, contradiction", "d": "Ch. 1 §1. Characters are known by what they do, say, and withhold. Oates supplies almost nothing but surface — Connie’s two selves, Arnold Friend’s borrowed slang and his stuffed boots — so inference is the only way in. Drill the move from trait to motive to what the contradiction reveals.", "r": "Ch. 1 §1 ‘Setting’ + Charlotte Perkins Gilman, “The Yellow Wallpaper.”", "p": null, "a": [], "s": [{"t": "Where Are You Going, Where Have You Been?", "a": "Joyce Carol Oates", "y": "1966", "e": "new"}]}, {"n": 4, "iso": "2027-01-11", "dow": "Mon", "md": "Jan 11", "wk": "2027-01-11", "u": "fiction", "t": "Setting as an agent, not a backdrop", "d": "Ch. 1 §1. The clearest case in American fiction of setting acting rather than describing — the room, the bars, the paper. Students mark the exact moment the nursery stops being where the story happens and becomes what the story is about.", "r": "Ch. 1 §1 ‘Plot’ + Flannery O’Connor, “A Good Man Is Hard to Find.”", "p": null, "a": [], "s": [{"t": "The Yellow Wallpaper", "a": "Charlotte Perkins Gilman", "y": "1892", "e": "new"}]}, {"n": 5, "iso": "2027-01-12", "dow": "Tue", "md": "Jan 12", "wk": "2027-01-11", "u": "fiction", "t": "Plot: arrangement over events", "d": "Ch. 1 §1. What order does to meaning. O’Connor plants the Misfit in the first paragraph and then spends twenty pages arranging a collision; students track the foreshadowing and argue whether the ending is inevitable or imposed. Plot and structure: 16–20% of the exam.", "r": "Ch. 1 §1 ‘Narrative Perspective and Point of View’ + Kochai, “Playing Metal Gear Solid V” and Hofler, “Erasure.”", "p": null, "a": [], "s": [{"t": "A Good Man Is Hard to Find", "a": "Flannery O'Connor", "y": "1953", "e": "new"}]}, {"n": 6, "iso": "2027-01-13", "dow": "Wed", "md": "Jan 13", "wk": "2027-01-11", "u": "fiction", "t": "Narrative perspective and point of view", "d": "Ch. 1 §1. Two contemporary stories make the textbook’s discussion of person concrete in a single class. Kochai writes in the second person, putting the reader inside a boy replaying a war his father survived; Hofler writes in the first-person plural, a collective office ‘we’ that watches its colleagues vanish and does nothing. Then back to third person, distance, and free indirect discourse. This category is 21–26% of the exam — the largest on the test.", "r": "Begin James Baldwin, “Sonny’s Blues” — read through the brothers’ reunion.", "p": null, "a": [{"k": "mcq", "l": "MCQ set · 11 prose items · 13 min · timed"}], "s": [{"t": "Playing Metal Gear Solid V: The Phantom Pain", "a": "Jamil Jan Kochai", "y": "2020", "e": "new"}, {"t": "Erasure", "a": "Sakinah Hofler", "y": "2020", "e": "new"}]}, {"n": 7, "iso": "2027-01-14", "dow": "Thu", "md": "Jan 14", "wk": "2027-01-11", "u": "fiction", "t": "Culminating: interpreting short fiction", "d": "Ch. 1 §1 culminating activity. “Sonny’s Blues” holds every element at once: a narrator who is also a character and an unreliable one, a Harlem that functions as a condition rather than a place, and a plot that only arrives at its meaning in the last two pages. Claim–evidence–commentary chains built on the board, then independently.", "r": "Finish “Sonny’s Blues.” Bring one interpretive claim with two pieces of evidence.", "p": null, "a": [{"k": "task", "l": "Ch. 1 §1 culminating task · graded for claim quality"}], "s": [{"t": "Sonny's Blues", "a": "James Baldwin", "y": "1957", "e": "new"}]}, {"n": 8, "iso": "2027-01-15", "dow": "Fri", "md": "Jan 15", "wk": "2027-01-11", "u": "fiction", "t": "Diction and syntax under the microscope", "d": "Ch. 1 §2. Close reading at word and sentence level, worked on Baldwin’s final scene — the passage beginning ‘All I know about music’ is one of the great syntactic performances in American prose. Students rewrite its sentences into ordinary order and say precisely what is lost.", "r": "Ch. 1 §2 close-reading section; reread Baldwin’s last three pages.", "p": null, "a": [], "s": [{"t": "Sonny's Blues", "a": "James Baldwin", "y": "1957", "e": "echo"}]}, {"n": 9, "iso": "2027-01-19", "dow": "Tue", "md": "Jan 19", "wk": "2027-01-18", "u": "fiction", "t": "Figurative language, imagery, tone, mood", "d": "Ch. 1 §2. Naming a device earns nothing; the commentary earns everything. Two returns: Gilman’s wallpaper, an image that becomes a symbol under pressure, and Baldwin’s cup of trembling, an allusion doing work no other image could do. Tone and mood drilled until the distinction is automatic.", "r": "Ch. 1 §2 ‘Crafting an AP Prose Fiction Analysis Essay.’", "p": null, "a": [], "s": [{"t": "The Yellow Wallpaper", "a": "Charlotte Perkins Gilman", "y": "1892", "e": "echo"}]}, {"n": 10, "iso": "2027-01-20", "dow": "Wed", "md": "Jan 20", "wk": "2027-01-18", "u": "fiction", "t": "From reading to writing: the Q2 essay", "d": "Ch. 1 §2. Prompt deconstruction, then defensible thesis, then line of reasoning. Students write three competing theses about the grandmother’s final gesture in O’Connor and rank them, defending the ranking. A thesis no one could argue against is not a thesis.", "r": "Ch. 1 §2 'Crafting an AP Prose Fiction Analysis Essay'.", "p": null, "a": [], "s": []}, {"n": 11, "iso": "2027-01-21", "dow": "Thu", "md": "Jan 21", "wk": "2027-01-18", "u": "fiction", "t": "Evidence, commentary, rubric calibration", "d": "Ch. 1 §2 revision work. Students score released College Board sample responses and norm to Row B. Disagreements get argued out loud — the norming conversation teaches more than the scores do.", "r": "Revise one sample essay paragraph from Ch. 1 §2.", "p": null, "a": [], "s": []}, {"n": 12, "iso": "2027-01-22", "dow": "Fri", "md": "Jan 22", "wk": "2027-01-18", "u": "fiction", "t": "Timed prose analysis essay", "d": "First graded free response of the semester, written under exam conditions. Students self-score against the rubric before leaving the room, while the choices they made are still fresh.", "r": "None — recover.", "p": null, "a": [{"k": "frq", "l": "Timed Q2 #1 · 40 min · graded"}], "s": []}, {"n": 13, "iso": "2027-01-25", "dow": "Mon", "md": "Jan 25", "wk": "2027-01-25", "u": "fiction", "t": "Sophistication: complexity, tension, qualification", "d": "Ch. 1 §3. What Row C actually rewards: a tension the text refuses to resolve. Two exhibits are already on the table — Hofler’s ‘we,’ which is witness and accomplice at once, and Oates’s ending, which declines to say what happens. Students revise the weakest paragraph of their timed essay to carry a qualified claim.", "r": "Ch. 1 §3 + revision due next class.", "p": null, "a": [{"k": "task", "l": "Ch. 1 §3 culminating revision + annotated rationale"}], "s": [{"t": "Erasure", "a": "Sakinah Hofler", "y": "2020", "e": "echo"}]}, {"n": 14, "iso": "2027-01-26", "dow": "Tue", "md": "Jan 26", "wk": "2027-01-25", "u": "poetry", "t": "Literal first: paraphrase before interpretation", "d": "Ch. 2 §1. The single biggest lever on poetry scores. Line-by-line paraphrase before any interpretive claim; inverted syntax rewritten into prose order. Students who skip this step write about a poem they have not read.", "r": "Ch. 2 §1 'Reading for Literal Meaning'.", "p": null, "a": [], "s": []}, {"n": 15, "iso": "2027-01-27", "dow": "Wed", "md": "Jan 27", "wk": "2027-01-25", "u": "poetry", "t": "The speaker, and what they speak against", "d": "Ch. 2 §1. Speaker is not poet. Then the machinery of contrast: juxtaposition, antithesis, paradox — the structures that let a short poem hold two things at once.", "r": "Ch. 2 §1 'Considering the Speaker' + assigned poems.", "p": null, "a": [], "s": []}, {"n": 16, "iso": "2027-01-28", "dow": "Thu", "md": "Jan 28", "wk": "2027-01-25", "u": "poetry", "t": "Diction, tone, mood, irony", "d": "Ch. 2 §1. Tone-shift hunting as a physical exercise — mark the line where the poem's attitude turns. Verbal, situational, and dramatic irony inside lyric poems, where irony is easiest to miss.", "r": "Ch. 2 §1 'Tone and Mood with Irony'.", "p": null, "a": [], "s": []}, {"n": 17, "iso": "2027-01-29", "dow": "Fri", "md": "Jan 29", "wk": "2027-01-25", "u": "poetry", "t": "Image, symbol, and the extended figure", "d": "Ch. 2 §1. Reading a controlling metaphor across an entire poem rather than device by device. The threshold question: when does an image become a symbol, and what evidence licenses that claim?", "r": "Ch. 2 §1 'Reading for Detail and Figurative Language'.", "p": null, "a": [], "s": []}, {"n": 18, "iso": "2027-02-01", "dow": "Mon", "md": "Feb 1", "wk": "2027-02-01", "u": "poetry", "t": "Structure: form, stanza, syntax, the volta", "d": "Ch. 2 §1. Sonnet, villanelle, free verse. Locating the turn — the volta is the most reliable thesis generator in poetry, because it marks the poem admitting to a change.", "r": "Ch. 2 §1 'Structure, Poetic Syntax, Meter, and Form'.", "p": null, "a": [], "s": []}, {"n": 19, "iso": "2027-02-02", "dow": "Tue", "md": "Feb 2", "wk": "2027-02-01", "u": "poetry", "t": "Sound, meter, rhyme — and when to mention it", "d": "Ch. 2 §1. Enough scansion to hear disruption, and a hard rule: sound only enters an essay when it is tied to meaning. Students find the metrical break in three poems and argue what it does.", "r": "Ch. 2 §1 'Sound and Rhyme'.", "p": null, "a": [], "s": []}, {"n": 20, "iso": "2027-02-03", "dow": "Wed", "md": "Feb 3", "wk": "2027-02-01", "u": "poetry", "t": "Culminating: interpret a complex poem cold", "d": "Ch. 2 §1 culminating activity. Full apparatus applied independently to an unseen poem in a single class period, then compared against a partner's reading.", "r": "None.", "p": null, "a": [{"k": "mcq", "l": "MCQ set · 11 poetry items · 13 min"}, {"k": "task", "l": "Ch. 2 §1 culminating task"}], "s": []}, {"n": 21, "iso": "2027-02-04", "dow": "Thu", "md": "Feb 4", "wk": "2027-02-01", "u": "poetry", "t": "From reading to writing: the Q1 essay", "d": "Ch. 2 §2. Graphic organizer to thesis. The thesis must name a movement in the poem — a shift, a tension, a reversal — not a list of devices. Device-list theses are diagnosed and rewritten on the spot.", "r": "Ch. 2 §2 'Crafting an AP Poetry Analysis Essay'.", "p": null, "a": [], "s": []}, {"n": 22, "iso": "2027-02-05", "dow": "Fri", "md": "Feb 5", "wk": "2027-02-01", "u": "poetry", "t": "Evidence, commentary, and peer feedback", "d": "Ch. 2 §2. Mechanics of quoting poetry — line breaks, slash marks, line numbers — then a structured peer-review protocol on full drafts. Peers mark only two things: unsupported claims and unexplained quotations.", "r": "Revise draft for tomorrow's conditions.", "p": null, "a": [], "s": []}, {"n": 23, "iso": "2027-02-08", "dow": "Mon", "md": "Feb 8", "wk": "2027-02-08", "u": "poetry", "t": "Timed poetry analysis essay", "d": "Exam conditions. Self-score, then a five-minute written reflection naming the one move that would have raised the score.", "r": "None — recover.", "p": null, "a": [{"k": "frq", "l": "Timed Q1 #1 · 40 min · graded"}], "s": []}, {"n": 24, "iso": "2027-02-09", "dow": "Tue", "md": "Feb 9", "wk": "2027-02-08", "u": "poetry", "t": "Sophistication in poetry", "d": "Ch. 2 §3. Situating a reading inside a broader literary or historical conversation without importing outside research. Qualification as a move, not a hedge.", "r": "Ch. 2 §3.", "p": null, "a": [], "s": []}, {"n": 25, "iso": "2027-02-10", "dow": "Wed", "md": "Feb 10", "wk": "2027-02-08", "u": "poetry", "t": "Culminating revision + unit checkpoint", "d": "Ch. 2 §3 culminating activity, and the first mixed-mode multiple-choice checkpoint. Scores get broken out by skill category so students can see which of the seven is costing them points.", "r": "None.", "p": null, "a": [{"k": "mcq", "l": "Checkpoint · 2 passages (1 poetry, 1 prose) · 22 items · 26 min"}, {"k": "task", "l": "Poetry revision due"}], "s": []}, {"n": 26, "iso": "2027-02-11", "dow": "Thu", "md": "Feb 11", "wk": "2027-02-08", "u": "frank", "t": "Launch: Prometheus, the Gothic, and 1816", "d": "Contexts that pay off analytically rather than trivia: Romanticism, Godwin and Wollstonecraft, galvanism, and the Prometheus myth. Read the 1831 introduction. Post the frame question that governs the unit — who is telling you this, and why should you doubt them?", "r": "Letters 1–4 (Walton to Margaret Saville).", "p": null, "a": [], "s": []}, {"n": 27, "iso": "2027-02-12", "dow": "Fri", "md": "Feb 12", "wk": "2027-02-08", "u": "frank", "t": "Ch. 3 §1: narration in longer works", "d": "Textbook Ch. 3 §1 on layered perspectives and unreliable narrators, taught directly onto Shelley's structure. Students diagram the three nested narrators and mark who controls what the reader is allowed to know.", "r": "Chapters 1–4.", "p": null, "a": [], "s": []}, {"n": 28, "iso": "2027-02-16", "dow": "Tue", "md": "Feb 16", "wk": "2027-02-15", "u": "frank", "t": "Victor's education and the will to know", "d": "Ambition rendered as characterization. Track the language of appetite and secrecy from Ingolstadt forward; Victor tells you what he is before he does anything.", "r": "Chapters 5–6.", "p": null, "a": [], "s": []}, {"n": 29, "iso": "2027-02-17", "dow": "Wed", "md": "Feb 17", "wk": "2027-02-15", "u": "frank", "t": "The creation scene: close-reading workshop", "d": "Ch. 1 §2 skills reapplied at novel scale — a full close read of the diction and syntax of Chapter 5, the passage most likely to appear on any exam. Opens with the semester's first Poetry Anchor.", "r": "Chapters 7–8.", "p": "Percy Shelley, 'Mutability' — quoted inside Chapter 10", "a": [], "s": []}, {"n": 30, "iso": "2027-02-18", "dow": "Thu", "md": "Feb 18", "wk": "2027-02-15", "u": "frank", "t": "Ch. 3 §1: setting as moral landscape", "d": "Textbook Ch. 3 §1 on historical and cultural setting. Mont Blanc, the Arctic frame, and the laboratory. Setting here is making an argument about scale and human smallness — students locate where the sublime turns from beautiful to indicting.", "r": "Chapters 9–10.", "p": null, "a": [], "s": []}, {"n": 31, "iso": "2027-02-19", "dow": "Fri", "md": "Feb 19", "wk": "2027-02-15", "u": "frank", "t": "The creature speaks", "d": "The novel's central formal gamble: handing narration to the antagonist. Students track their own sympathy shifting in real time and identify the rhetorical moves that cause it.", "r": "Chapters 11–12.", "p": null, "a": [], "s": []}, {"n": 32, "iso": "2027-02-22", "dow": "Mon", "md": "Feb 22", "wk": "2027-02-22", "u": "frank", "t": "Ch. 3 §1: character, foils, and doubles", "d": "Victor and the creature, Victor and Clerval, Walton and Victor. Foil used as an analytic instrument rather than a vocabulary word: what does the pairing let the novel say that neither figure could say alone?", "r": "Chapters 13–14.", "p": null, "a": [], "s": []}, {"n": 33, "iso": "2027-02-23", "dow": "Tue", "md": "Feb 23", "wk": "2027-02-22", "u": "frank", "t": "Paradise Lost inside Frankenstein", "d": "The creature's three books, and the choice between Adam and Satan as self-description. Excerpt from Paradise Lost Book IX read alongside Chapter 15 — intertextuality as characterization.", "r": "Chapters 15–16.", "p": "Milton, Paradise Lost, Book IX (excerpt)", "a": [], "s": []}, {"n": 34, "iso": "2027-02-24", "dow": "Wed", "md": "Feb 24", "wk": "2027-02-22", "u": "frank", "t": "Ch. 3 §1: symbol and allegory", "d": "Textbook Ch. 3 §1 closing element. Fire and light, ice, the double. The discipline of arguing a symbol from repetition and context rather than asserting it.", "r": "Chapters 17–18.", "p": "Percy Shelley, 'Ozymandias' — ruin and the maker's boast", "a": [], "s": []}, {"n": 35, "iso": "2027-02-25", "dow": "Thu", "md": "Feb 25", "wk": "2027-02-22", "u": "frank", "t": "The second creation refused", "d": "Moral reasoning under narrative pressure. Set Victor’s calculation beside the Misfit’s: both men talk themselves, one careful step at a time, into an atrocity. Where does each text withhold judgment, and what does that withholding do to the reader? A strong Row C paragraph often lives in exactly this kind of gap.", "r": "Chapters 19–20.", "p": null, "a": [], "s": [{"t": "A Good Man Is Hard to Find", "a": "Flannery O'Connor", "y": "1953", "e": "echo"}]}, {"n": 36, "iso": "2027-02-26", "dow": "Fri", "md": "Feb 26", "wk": "2027-02-22", "u": "frank", "t": "Justice, Justine, and the novel's women", "d": "Elizabeth, Justine, Safie, and Margaret Saville — who gets to speak, who only gets narrated, and what the novel’s structure of silence implies. Reread “The Yellow Wallpaper” against them: a woman diagnosed, confined, and written about by the man who loves her. Sets up the gendered lens taken up formally in the Hamlet unit.", "r": "Chapters 21–22.", "p": null, "a": [], "s": [{"t": "The Yellow Wallpaper", "a": "Charlotte Perkins Gilman", "y": "1892", "e": "echo"}]}, {"n": 37, "iso": "2027-03-01", "dow": "Mon", "md": "Mar 1", "wk": "2027-03-01", "u": "frank", "t": "The pursuit north; the frame closes", "d": "Return to Walton. How the closing of a frame retroactively revises everything inside it — the last two pages change the status of the whole novel's testimony.", "r": "Chapters 23–24 and 'Walton, in continuation' (finish the novel).", "p": null, "a": [], "s": []}, {"n": 38, "iso": "2027-03-02", "dow": "Tue", "md": "Mar 2", "wk": "2027-03-01", "u": "frank", "t": "Ch. 3 §1 culminating: interpreting longer fiction", "d": "Whole-novel interpretation. Students build a thesis about the novel's central unresolved tension and defend it with evidence drawn from all three narrators — the requirement to cross narrators is what makes it hard.", "r": "Prepare evidence from each narrator.", "p": null, "a": [{"k": "task", "l": "Ch. 3 §1 culminating task · graded"}], "s": []}, {"n": 39, "iso": "2027-03-03", "dow": "Wed", "md": "Mar 3", "wk": "2027-03-01", "u": "frank", "t": "Building the Q3 text bank", "d": "The mechanics that make Question 3 survivable: a scene inventory, a quotation bank kept from memory, and a thematic index card. Every student leaves with a one-page Frankenstein sheet built to answer prompts that have not been written yet.", "r": "Finish Frankenstein index page.", "p": "Coleridge, 'The Rime of the Ancient Mariner' (excerpt) — Walton's touchstone", "a": [], "s": []}, {"n": 40, "iso": "2027-03-04", "dow": "Thu", "md": "Mar 4", "wk": "2027-03-01", "u": "frank", "t": "Timed literary argument essay", "d": "First Question 3 under exam conditions, on a released prompt, using Frankenstein. Written from memory with no text in the room — as on the exam.", "r": "None — recover.", "p": null, "a": [{"k": "frq", "l": "Timed Q3 #1 · 40 min · graded"}], "s": []}, {"n": 41, "iso": "2027-03-05", "dow": "Fri", "md": "Mar 5", "wk": "2027-03-01", "u": "frank", "t": "Seminar + multiple-choice checkpoint", "d": "Socratic seminar on the question the novel refuses to settle: is Victor's crime the creation or the abandonment? Followed by a timed checkpoint including a pre-1900 prose passage.", "r": "Over the weekend: Ursula K. Le Guin, “The Ones Who Walk Away from Omelas” (5 pp).", "p": null, "a": [{"k": "mcq", "l": "Checkpoint · 2 passages (pre-1900 prose + poetry) · 22 items"}, {"k": "task", "l": "Seminar participation · rubric-scored"}], "s": []}, {"n": 42, "iso": "2027-03-08", "dow": "Mon", "md": "Mar 8", "wk": "2027-03-08", "u": "nlmg", "t": "Launch: Hailsham and the withheld premise", "d": "Deliberately paired with Frankenstein, and opened with Le Guin. “Omelas” states the bargain plainly in five pages and asks the reader to decide; Ishiguro will spend 288 pages never stating it at all. Establish the reading rule for the unit — attend to what Kathy does not say. Strict no-spoiler contract.", "r": "Chapters 1–2 (Part One).", "p": null, "a": [], "s": [{"t": "The Ones Who Walk Away from Omelas", "a": "Ursula K. Le Guin", "y": "1973", "e": "new"}]}, {"n": 43, "iso": "2027-03-09", "dow": "Tue", "md": "Mar 9", "wk": "2027-03-08", "u": "nlmg", "t": "Kathy H.: memory as narration", "d": "Retrospective first person, and the hardest version of the reliability question — a narrator who is entirely sincere and still cannot tell you the truth, because of how she was raised.", "r": "Chapters 3–4.", "p": null, "a": [], "s": []}, {"n": 44, "iso": "2027-03-10", "dow": "Wed", "md": "Mar 10", "wk": "2027-03-08", "u": "nlmg", "t": "Euphemism as worldbuilding", "d": "Carers, donors, completing. Diction study using Ch. 1 §2 tools: how a vocabulary can make an atrocity administratively ordinary. Students build a glossary of the novel's substitutions.", "r": "Chapters 5–6.", "p": "Philip Larkin, 'Ambulances'", "a": [], "s": []}, {"n": 45, "iso": "2027-03-11", "dow": "Thu", "md": "Mar 11", "wk": "2027-03-08", "u": "nlmg", "t": "Art, the Gallery, and the soul question", "d": "Madame, the Gallery, and Tommy's animals. What exactly is art being asked to prove here, and to whom? The novel's most direct statement of its own stakes.", "r": "Chapters 7–9 (finish Part One).", "p": null, "a": [], "s": []}, {"n": 46, "iso": "2027-03-12", "dow": "Fri", "md": "Mar 12", "wk": "2027-03-08", "u": "nlmg", "t": "Ch. 3 §2: from summary to interpretation", "d": "Textbook Ch. 3 §2 opens. The Question 3 thesis makes a claim about meaning, not about plot. Students take five summary-level theses and convert each into an interpretive one.", "r": "Chapters 10–11 (Part Two) + Te-Ping Chen, “Lulu” over the weekend.", "p": null, "a": [], "s": []}, {"n": 47, "iso": "2027-03-15", "dow": "Mon", "md": "Mar 15", "wk": "2027-03-15", "u": "nlmg", "t": "The Cottages: freedom without a future", "d": "Setting and social structure. The students imitate behavior they have only seen on television, and nobody leaves. Chen’s “Lulu” is the counterexample read against them — a twin who does speak, what it costs her, and the brother who stays home and narrates it.", "r": "Chapters 12–13.", "p": null, "a": [], "s": [{"t": "Lulu", "a": "Te-Ping Chen", "y": "2021", "e": "new"}]}, {"n": 48, "iso": "2027-03-16", "dow": "Tue", "md": "Mar 16", "wk": "2027-03-15", "u": "nlmg", "t": "Norfolk and the lost corner", "d": "Symbol and motif revisited from Ch. 3 §1, now in a novel that keeps its symbols deliberately thin. The possible, the found, the misremembered.", "r": "Chapters 14–15.", "p": null, "a": [], "s": []}, {"n": 49, "iso": "2027-03-17", "dow": "Wed", "md": "Mar 17", "wk": "2027-03-15", "u": "nlmg", "t": "Ch. 3 §2: thesis and topic sentences", "d": "Textbook Ch. 3 §2 workshop. Topic sentences that advance a line of reasoning instead of announcing a new topic. Built on a Never Let Me Go prompt written for the class.", "r": "Chapters 16–17 (finish Part Two).", "p": "Keats, 'Ode on a Grecian Urn' — arrested life, art as evidence", "a": [], "s": []}, {"n": 50, "iso": "2027-03-18", "dow": "Thu", "md": "Mar 18", "wk": "2027-03-15", "u": "nlmg", "t": "Part Three: deferrals and the visit", "d": "The revelation scene. Miss Emily's speech read as rhetoric — who is she persuading, and what does she need the reader to concede?", "r": "Chapters 18–20.", "p": null, "a": [], "s": []}, {"n": 51, "iso": "2027-03-19", "dow": "Fri", "md": "Mar 19", "wk": "2027-03-15", "u": "nlmg", "t": "Ch. 3 §2: evidence and interpretive commentary", "d": "Textbook Ch. 3 §2. The difference between quoting and using. Students rebuild one weak body paragraph in three timed passes, adding only commentary each time.", "r": "Chapters 21–23 (finish the novel).", "p": null, "a": [], "s": []}, {"n": 52, "iso": "2027-03-22", "dow": "Mon", "md": "Mar 22", "wk": "2027-03-22", "u": "nlmg", "t": "Structure, the flat ending, and a paired seminar", "d": "Why the final field scene refuses catharsis, and what that refusal argues. Then the paired seminar with Frankenstein: what makes a person, and who gets to decide?", "r": "Prepare two pieces of evidence from each novel.", "p": "Auden, 'Musée des Beaux Arts' — suffering that goes unattended", "a": [{"k": "task", "l": "Paired seminar · rubric-scored"}], "s": []}, {"n": 53, "iso": "2027-03-23", "dow": "Tue", "md": "Mar 23", "wk": "2027-03-22", "u": "nlmg", "t": "Ch. 3 §2 culminating: literary argument essay", "d": "Full-process Question 3 — plan, draft, peer review using the Ch. 3 §2 protocol. Untimed, so that the process itself can be taught before it has to be compressed.", "r": "Finish draft.", "p": null, "a": [{"k": "task", "l": "Ch. 3 §2 culminating essay · process-graded"}], "s": []}, {"n": 54, "iso": "2027-03-24", "dow": "Wed", "md": "Mar 24", "wk": "2027-03-22", "u": "nlmg", "t": "Timed literary argument essay", "d": "Second timed Question 3. Student chooses Frankenstein or Never Let Me Go — the choice itself is a skill, and choosing badly is a diagnosable habit.", "r": "None — recover.", "p": null, "a": [{"k": "frq", "l": "Timed Q3 #2 · 40 min · graded"}], "s": []}, {"n": 55, "iso": "2027-03-25", "dow": "Thu", "md": "Mar 25", "wk": "2027-03-22", "u": "nlmg", "t": "First full-length multiple-choice section", "d": "Fifty-five items in sixty minutes — the real thing, including pacing pressure. Immediate item analysis by skill category, then update the Q3 text bank before break.", "r": "No required reading over break. Optional: watch a filmed Hamlet.", "p": null, "a": [{"k": "mcq", "l": "Full MCQ section · 55 items · 60 min · graded"}], "s": []}, {"n": 56, "iso": "2027-04-05", "dow": "Mon", "md": "Apr 5", "wk": "2027-04-05", "u": "hamlet", "t": "Launch: revenge tragedy and the problem of delay", "d": "Genre conventions, then Shakespeare's toolkit: blank verse against prose, and the soliloquy as a technology for showing interiority. Ch. 3 §1 elements revisited for drama, where the reader has no narrator to trust or doubt.", "r": "Act I, scenes i–ii read aloud in class.", "p": null, "a": [], "s": []}, {"n": 57, "iso": "2027-04-06", "dow": "Tue", "md": "Apr 6", "wk": "2027-04-05", "u": "hamlet", "t": "Act I, iii–v: the Ghost's charge", "d": "Performance-based reading, standing up. What the Ghost’s command actually obligates. Reread Kochai beside it: a son handed an impossible charge by a lost father, replaying the same level over and over trying to change the outcome. Hamlet gets one life and no save point.", "r": "Reread I.v; mark Hamlet's conditions.", "p": null, "a": [], "s": [{"t": "Playing Metal Gear Solid V: The Phantom Pain", "a": "Jamil Jan Kochai", "y": "2020", "e": "echo"}]}, {"n": 58, "iso": "2027-04-07", "dow": "Wed", "md": "Apr 7", "wk": "2027-04-05", "u": "hamlet", "t": "The soliloquy as characterization", "d": "'O that this too too solid flesh' treated as a poem and given the full Ch. 2 §1 apparatus — paraphrase, speaker, contrast, structure, sound. The clearest demonstration all semester that poetry skills are not a separate unit.", "r": "Act II, scene i.", "p": "Shakespeare, 'O that this too too solid flesh' (I.ii.129–159)", "a": [], "s": []}, {"n": 59, "iso": "2027-04-08", "dow": "Thu", "md": "Apr 8", "wk": "2027-04-05", "u": "hamlet", "t": "Act II, ii: surveillance and performance", "d": "Everyone in Elsinore is watching someone. The Players arrive and the play turns meta-theatrical — acting becomes the play's governing metaphor for sincerity and its absence.", "r": "Reread the Hecuba speech.", "p": null, "a": [], "s": []}, {"n": 60, "iso": "2027-04-09", "dow": "Fri", "md": "Apr 9", "wk": "2027-04-05", "u": "hamlet", "t": "'To be or not to be' and the nunnery scene", "d": "Close read of III.i, then two filmed deliveries compared shot for shot. Staging is interpretation: students argue which reading the text better supports and what each production had to suppress.", "r": "Act III, scene i.", "p": null, "a": [], "s": []}, {"n": 61, "iso": "2027-04-12", "dow": "Mon", "md": "Apr 12", "wk": "2027-04-12", "u": "hamlet", "t": "Act III, ii: The Mousetrap", "d": "The play-within-the-play as structural device, taught against Ch. 3 §1 on structure. A frame inside a frame — the same formal question the class already worked through in Frankenstein.", "r": "Reread III.ii.", "p": null, "a": [], "s": []}, {"n": 62, "iso": "2027-04-13", "dow": "Tue", "md": "Apr 13", "wk": "2027-04-12", "u": "hamlet", "t": "The prayer scene and the closet scene", "d": "Motive and dramatic irony at their sharpest, and the killing of Polonius. Sets up the interpretive dispute the next two classes formalize: whose reading of Gertrude is the text actually licensing?", "r": "Act III, scenes iii–iv.", "p": null, "a": [], "s": []}, {"n": 63, "iso": "2027-04-14", "dow": "Wed", "md": "Apr 14", "wk": "2027-04-12", "u": "hamlet", "t": "Ch. 3 §3: critical lenses I — psychological", "d": "Textbook Ch. 3 §3. A psychological lens applied to the delay, and the crucial distinction between using a lens and imposing one. A lens is only earned when the text rewards it.", "r": "Act IV, scenes i–iv.", "p": "Shakespeare, Sonnet 30 — memory, grief, and account-keeping", "a": [], "s": []}, {"n": 64, "iso": "2027-04-15", "dow": "Thu", "md": "Apr 15", "wk": "2027-04-12", "u": "hamlet", "t": "Ch. 3 §3: critical lenses II — gendered and cultural", "d": "Textbook Ch. 3 §3 continued. Ophelia's madness and Gertrude's silence, read against both the Elizabethan frame and a modern one. Students argue which reading the play supports and where it resists.", "r": "Act IV, scenes v–vii.", "p": null, "a": [], "s": []}, {"n": 65, "iso": "2027-04-16", "dow": "Fri", "md": "Apr 16", "wk": "2027-04-12", "u": "hamlet", "t": "Act V, i: the graveyard", "d": "Memento mori, and comedy placed inside tragedy on purpose. Yorick's skull as the play's pivot from revenge toward acceptance — a structural turn students can name and defend.", "r": "Reread V.i; mark the tonal shift.", "p": null, "a": [], "s": []}, {"n": 66, "iso": "2027-04-19", "dow": "Mon", "md": "Apr 19", "wk": "2027-04-19", "u": "hamlet", "t": "Act V, ii: 'the readiness is all'", "d": "The duel, the bodies, and Fortinbras walking in. What the ending asks the audience to conclude, and what it pointedly declines to settle.", "r": "Finish the play.", "p": null, "a": [], "s": []}, {"n": 67, "iso": "2027-04-20", "dow": "Tue", "md": "Apr 20", "wk": "2027-04-19", "u": "hamlet", "t": "Ch. 3 §3: answering a competing reading", "d": "Textbook Ch. 3 §3 closing. Building a Row C argument that names an opposing interpretation and answers it — the most reliable route to the sophistication point, and the hardest to fake.", "r": "Draft one counter-reading paragraph.", "p": null, "a": [], "s": []}, {"n": 68, "iso": "2027-04-21", "dow": "Wed", "md": "Apr 21", "wk": "2027-04-19", "u": "hamlet", "t": "Performance workshop", "d": "Small groups stage a twenty-line cut and defend one interpretive choice in writing. Performance is argument: blocking, pace, and cuts are all claims about meaning that have to be supported by the text.", "r": "None.", "p": null, "a": [{"k": "task", "l": "Performance + written interpretive rationale · graded"}], "s": []}, {"n": 69, "iso": "2027-04-22", "dow": "Thu", "md": "Apr 22", "wk": "2027-04-19", "u": "hamlet", "t": "Timed literary argument essay", "d": "Third timed Question 3, on Hamlet, using a released prompt. By now the process should be automatic and the thinking should be where the time goes.", "r": "None — recover.", "p": null, "a": [{"k": "frq", "l": "Timed Q3 #3 · 40 min · graded"}], "s": []}, {"n": 70, "iso": "2027-04-23", "dow": "Fri", "md": "Apr 23", "wk": "2027-04-19", "u": "hamlet", "t": "Three-text seminar; text bank finalized", "d": "What each of the three works is best at answering. Students finalize a one-page index per text: five scenes, eight quotations, six thematic entry points. This is the document they will think with on May 5.", "r": "None.", "p": null, "a": [{"k": "task", "l": "Q3 text bank due · all three works"}], "s": []}, {"n": 71, "iso": "2027-04-26", "dow": "Mon", "md": "Apr 26", "wk": "2027-04-26", "u": "review", "t": "Full multiple-choice section + item analysis", "d": "Fifty-five items in sixty minutes, then analysis broken out by the seven skill categories. The point is not the score — it is identifying the two categories that are actually costing points.", "r": "None.", "p": null, "a": [{"k": "mcq", "l": "Full MCQ section · 55 items · 60 min · graded"}], "s": []}, {"n": 72, "iso": "2027-04-27", "dow": "Tue", "md": "Apr 27", "wk": "2027-04-26", "u": "review", "t": "Multiple-choice strategy clinic", "d": "Targeted work on the two weakest categories from yesterday. Question-stem taxonomy, elimination discipline, and pacing — roughly thirteen minutes per passage set, with a plan for the set that goes wrong.", "r": "None.", "p": null, "a": [], "s": []}, {"n": 73, "iso": "2027-04-28", "dow": "Wed", "md": "Apr 28", "wk": "2027-04-26", "u": "review", "t": "Poetry essay under time, peer-scored", "d": "Timed Question 1, then peer scoring with the official rubric, then re-scoring against a released College Board sample. Scoring other people's essays is the fastest way to see your own.", "r": "None.", "p": null, "a": [{"k": "frq", "l": "Timed Q1 #2 · 40 min · peer-scored"}], "s": []}, {"n": 74, "iso": "2027-04-29", "dow": "Thu", "md": "Apr 29", "wk": "2027-04-26", "u": "review", "t": "Prose essay under time, peer-scored", "d": "Timed Question 2 on the same protocol. Two consecutive days of scoring calibrates students to the rubric far better than a semester of receiving grades.", "r": "None.", "p": null, "a": [{"k": "frq", "l": "Timed Q2 #2 · 40 min · peer-scored"}], "s": []}, {"n": 75, "iso": "2027-04-30", "dow": "Fri", "md": "Apr 30", "wk": "2027-04-26", "u": "review", "t": "Row C clinic: earning the sophistication point", "d": "Eight authentic sophistication moves, each illustrated with a real example pulled from this class's own essays this semester. Students then revise one paragraph from each of their three Question 3 essays.", "r": "None.", "p": null, "a": [], "s": []}, {"n": 76, "iso": "2027-05-03", "dow": "Mon", "md": "May 3", "wk": "2027-05-03", "u": "review", "t": "Full free-response block at exam pace", "d": "The 90-minute block used as a compressed exam simulation: two complete essays plus one full Question 3 plan, at real pace. Debrief is entirely about time management, not content.", "r": "None.", "p": null, "a": [{"k": "frq", "l": "Timed FRQ block · Q1 + Q2 + Q3 plan"}], "s": []}, {"n": 77, "iso": "2027-05-04", "dow": "Tue", "md": "May 4", "wk": "2027-05-03", "u": "review", "t": "Exam-day walkthrough", "d": "Logistics, a timing plan written on paper, the five-minute planning rule, and what to do when the passage is genuinely opaque. Everything is returned. No new content — the learning is done.", "r": "Sleep.", "p": null, "a": [], "s": []}], "units": [{"k": "launch", "name": "Course Launch", "sub": "Diagnostics & the shape of the exam", "c": "#5C6B7A", "days": 2, "range": "Jan 6 – Jan 7"}, {"k": "fiction", "name": "Short Fiction", "sub": "Textbook Ch. 1 — prose analysis (Q2)", "c": "#3F6B8F", "days": 11, "range": "Jan 8 – Jan 25"}, {"k": "poetry", "name": "Poetry", "sub": "Textbook Ch. 2 — poetry analysis (Q1)", "c": "#A8792B", "days": 12, "range": "Jan 26 – Feb 10"}, {"k": "frank", "name": "Frankenstein", "sub": "Textbook Ch. 3 §1 — elements of longer fiction", "c": "#2E7C7A", "days": 16, "range": "Feb 11 – Mar 5"}, {"k": "nlmg", "name": "Never Let Me Go", "sub": "Textbook Ch. 3 §2 — the literary argument (Q3)", "c": "#6C7F52", "days": 14, "range": "Mar 8 – Mar 25"}, {"k": "hamlet", "name": "Hamlet", "sub": "Textbook Ch. 3 §3 — critical lenses & sophistication", "c": "#93303C", "days": 15, "range": "Apr 5 – Apr 23"}, {"k": "review", "name": "Exam Review", "sub": "Full-length practice and the Row C clinic", "c": "#5B4A8C", "days": 7, "range": "Apr 26 – May 4"}], "weeks": [{"wk": "2027-01-04", "num": 1, "range": "Jan 6 – Jan 8", "count": 3}, {"wk": "2027-01-11", "num": 2, "range": "Jan 11 – Jan 15", "count": 5}, {"wk": "2027-01-18", "num": 3, "range": "Jan 19 – Jan 22", "count": 4}, {"wk": "2027-01-25", "num": 4, "range": "Jan 25 – Jan 29", "count": 5}, {"wk": "2027-02-01", "num": 5, "range": "Feb 1 – Feb 5", "count": 5}, {"wk": "2027-02-08", "num": 6, "range": "Feb 8 – Feb 12", "count": 5}, {"wk": "2027-02-15", "num": 7, "range": "Feb 16 – Feb 19", "count": 4}, {"wk": "2027-02-22", "num": 8, "range": "Feb 22 – Feb 26", "count": 5}, {"wk": "2027-03-01", "num": 9, "range": "Mar 1 – Mar 5", "count": 5}, {"wk": "2027-03-08", "num": 10, "range": "Mar 8 – Mar 12", "count": 5}, {"wk": "2027-03-15", "num": 11, "range": "Mar 15 – Mar 19", "count": 5}, {"wk": "2027-03-22", "num": 12, "range": "Mar 22 – Mar 25", "count": 4}, {"wk": "2027-04-05", "num": 13, "range": "Apr 5 – Apr 9", "count": 5}, {"wk": "2027-04-12", "num": 14, "range": "Apr 12 – Apr 16", "count": 5}, {"wk": "2027-04-19", "num": 15, "range": "Apr 19 – Apr 23", "count": 5}, {"wk": "2027-04-26", "num": 16, "range": "Apr 26 – Apr 30", "count": 5}, {"wk": "2027-05-03", "num": 17, "range": "May 3 – May 4", "count": 2}], "breaks": [{"wk": "2027-01-18", "label": "MLK Day", "range": "Jan 18", "after": "2027-01-17"}, {"wk": "2027-02-15", "label": "Presidents Day / teacher workday", "range": "Feb 15", "after": "2027-02-14"}, {"wk": "2027-03-22", "label": "Good Friday", "range": "Mar 26", "after": "2027-03-25"}, {"wk": "2027-03-29", "label": "Spring Break", "range": "Mar 29 – Apr 2", "after": "2027-03-28"}]};
const U = {}; DATA.units.forEach(u => U[u.k] = u);
const state = { unit: null, assess: false, poem: false, story: false };

/* ---- budget bar ---- */
const bar = document.getElementById('bar');
DATA.units.forEach(u => {
  const b = document.createElement('button');
  b.className = 'budget-seg';
  b.style.width = (u.days / 77 * 100) + '%';
  b.style.background = 'var(--u-' + u.k + ')';
  b.setAttribute('aria-pressed', 'false');
  b.setAttribute('title', u.name + ' — ' + u.days + ' days (' + u.range + ')');
  b.innerHTML = '<span>' + (u.days >= 7 ? u.days : '') + '</span>';
  b.addEventListener('click', () => toggleUnit(u.k));
  b.dataset.unit = u.k;
  bar.appendChild(b);
});

/* ---- legend / filters ---- */
const legend = document.getElementById('legend');
DATA.units.forEach(u => {
  const b = document.createElement('button');
  b.className = 'ubtn';
  b.style.setProperty('--uc', 'var(--u-' + u.k + ')');
  b.setAttribute('aria-pressed', 'false');
  b.dataset.unit = u.k;
  b.innerHTML =
    '<span class="swatch"></span>' +
    '<span><span class="un">' + u.name + '</span><span class="us">' + u.sub + '</span></span>' +
    '<span class="uc">' + u.days + '<small>' + u.range + '</small></span>';
  b.addEventListener('click', () => toggleUnit(u.k));
  legend.appendChild(b);
});

function toggleUnit(k){ state.unit = (state.unit === k) ? null : k; render(); }

document.getElementById('btn-all').addEventListener('click', () => {
  state.unit = null; state.assess = false; state.poem = false; state.story = false; render();
});
document.getElementById('btn-assess').addEventListener('click', () => {
  state.assess = !state.assess; if (state.assess) { state.poem = false; state.story = false; } render();
});
document.getElementById('btn-poem').addEventListener('click', () => {
  state.poem = !state.poem; if (state.poem) { state.assess = false; state.story = false; } render();
});
document.getElementById('btn-story').addEventListener('click', () => {
  state.story = !state.story; if (state.story) { state.assess = false; state.poem = false; } render();
});

/* ---- schedule ---- */
const KIND = { frq:'chip-frq', mcq:'chip-mcq', task:'chip-task' };
const esc = s => String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;');
const ital = s => esc(s)
  .replace(/Frankenstein/g, '<cite>Frankenstein</cite>')
  .replace(/Never Let Me Go/g, '<cite>Never Let Me Go</cite>')
  .replace(/Paradise Lost/g, '<cite>Paradise Lost</cite>')
  .replace(/\bHamlet\b(?!'s)/g, '<cite>Hamlet</cite>');

function dayCard(d){
  const el = document.createElement('article');
  el.className = 'day';
  el.style.setProperty('--uc', 'var(--u-' + d.u + ')');
  let meta = '';
  if (d.r && d.r !== 'None.' && d.r !== 'None — recover.' && d.r !== 'Sleep.')
    meta += '<span class="chip chip-read"><b>Tonight</b>' + ital(d.r) + '</span>';
  if (d.p)
    meta += '<span class="chip chip-poem"><b>Poetry anchor</b>' + ital(d.p) + '</span>';
  d.s.forEach(st => {
    meta += '<span class="chip chip-story' + (st.e === 'echo' ? ' echo' : '') + '">' +
      '<b>' + (st.e === 'echo' ? 'Story echo' : 'Story') + '</b>' +
      '<i>\u201c' + esc(st.t) + '\u201d</i> \u2014 ' + esc(st.a) + ' <em>' + st.y + '</em></span>';
  });
  d.a.forEach(a => { meta += '<span class="chip ' + KIND[a.k] + '">' + esc(a.l) + '</span>'; });
  el.innerHTML =
    '<div class="day-mark"><div class="day-n">' + d.n + '</div>' +
    '<div class="day-d">' + d.dow + '<br>' + d.md + '</div></div>' +
    '<div class="day-body"><h3 class="day-t">' + ital(d.t) + '</h3>' +
    '<p class="day-x">' + ital(d.d) + '</p>' +
    (meta ? '<div class="day-meta">' + meta + '</div>' : '') +
    '</div>';
  return el;
}

const weeksEl = document.getElementById('weeks');
function render(){
  const days = DATA.days.filter(d =>
    (!state.unit || d.u === state.unit) &&
    (!state.assess || d.a.length) &&
    (!state.poem || d.p) &&
    (!state.story || d.s.length)
  );
  const keep = new Set(days.map(d => d.wk));
  weeksEl.innerHTML = '';
  DATA.weeks.forEach(w => {
    const ds = days.filter(d => d.wk === w.wk);
    if (!ds.length) return;
    const sec = document.createElement('section');
    sec.className = 'week';
    sec.innerHTML =
      '<div class="week-bar"><span class="week-n">Week ' + w.num + '</span>' +
      '<span class="week-r">' + w.range + '</span>' +
      '<span class="week-c">' + ds.length + ' of ' + w.count + ' days shown</span></div>';
    ds.forEach(d => sec.appendChild(dayCard(d)));
    DATA.breaks.filter(b => b.wk === w.wk).forEach(b => {
      const bd = document.createElement('div');
      bd.className = 'brk';
      bd.innerHTML = '<span class="brk-l">No school</span><span class="brk-d">' + b.label +
        '</span><span class="brk-t">' + b.range + '</span>';
      sec.appendChild(bd);
    });
    weeksEl.appendChild(sec);
  });
  // spring break sits between two weeks with no class days of its own
  document.getElementById('showing').textContent =
    days.length + ' of 77 days' + (state.unit ? ' · ' + U[state.unit].name : '');
  document.querySelectorAll('.ubtn').forEach(b =>
    b.setAttribute('aria-pressed', String(b.dataset.unit === state.unit)));
  document.querySelectorAll('.budget-seg').forEach(b => {
    b.setAttribute('aria-pressed', String(b.dataset.unit === state.unit));
    b.classList.toggle('dimmed', !!state.unit);
  });
  document.getElementById('btn-all').setAttribute('aria-pressed',
    String(!state.unit && !state.assess && !state.poem && !state.story));
  document.getElementById('btn-assess').setAttribute('aria-pressed', String(state.assess));
  document.getElementById('btn-poem').setAttribute('aria-pressed', String(state.poem));
  document.getElementById('btn-story').setAttribute('aria-pressed', String(state.story));
}

/* ---- ledger ---- */
const ledger = document.getElementById('ledger');
DATA.days.forEach(d => d.a.forEach(a => {
  const tr = document.createElement('tr');
  tr.style.setProperty('--uc', 'var(--u-' + d.u + ')');
  tr.innerHTML = '<td class="m">' + d.dow + ' ' + d.md + '</td>' +
    '<td class="m">' + d.n + '</td>' +
    '<td class="u">' + U[d.u].name + '</td>' +
    '<td class="k" style="font-weight:400">' + esc(a.l) + '</td>';
  ledger.appendChild(tr);
}));

render();
</script>

</body>
</html>
