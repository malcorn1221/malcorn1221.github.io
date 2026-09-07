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
<title>AP Lit Spring 2027</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@400;500&family=IBM+Plex+Sans:ital,wght@0,400;0,500;0,600;1,400&family=Spectral:ital,wght@0,500;0,600;0,700;1,500&display=swap">
<style>
:root{
  --bg:#EDEFF3; --surface:#FFFFFF; --surface-2:#F4F6FA; --surface-3:#E5E9F0;
  --ink:#13171E; --ink-2:#4B5462; --ink-3:#7C8494;
  --rule:#D6DBE3; --rule-2:#E6EAF0;
  --accent:#8E2F3B; --due:#1F5E8F; --good:#2F6B4F;
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
    --accent:#D9808B; --due:#7DB3DC; --good:#7FBF9C;
    --u-launch:#8FA1B3; --u-fiction:#7FAACB; --u-poetry:#D7AE5C;
    --u-frank:#62B8B2; --u-nlmg:#A3B978; --u-hamlet:#D9808B; --u-review:#9B8AD6;
    --shadow:0 1px 2px rgba(0,0,0,.4), 0 8px 24px -14px rgba(0,0,0,.7);
  }
}
:root[data-theme="dark"]{
  --bg:#0F1217; --surface:#171B22; --surface-2:#1E232B; --surface-3:#262C36;
  --ink:#E7EAEF; --ink-2:#A6AEBC; --ink-3:#6F7887;
  --rule:#2A303A; --rule-2:#222831;
  --accent:#D9808B; --due:#7DB3DC; --good:#7FBF9C;
  --u-launch:#8FA1B3; --u-fiction:#7FAACB; --u-poetry:#D7AE5C;
  --u-frank:#62B8B2; --u-nlmg:#A3B978; --u-hamlet:#D9808B; --u-review:#9B8AD6;
  --shadow:0 1px 2px rgba(0,0,0,.4), 0 8px 24px -14px rgba(0,0,0,.7);
}

*{box-sizing:border-box}
body{background:var(--bg); color:var(--ink); font-family:var(--sans); font-size:15px; line-height:1.55; -webkit-font-smoothing:antialiased}
.wrap{max-width:960px; margin:0 auto; padding:0 24px 96px}
h1,h2,h3{font-family:var(--serif); font-weight:600; text-wrap:balance; margin:0}
a{color:var(--accent)}
:focus-visible{outline:2px solid var(--accent); outline-offset:2px; border-radius:3px}
@media (prefers-reduced-motion: reduce){*{animation:none!important; transition:none!important}}

/* ---------- masthead ---------- */
.mast{padding:44px 0 24px}
.eyebrow{font-family:var(--mono); font-size:11.5px; letter-spacing:.13em; text-transform:uppercase; color:var(--ink-3); margin:0 0 12px}
.mast h1{font-size:clamp(34px,5.4vw,50px); line-height:1.04; letter-spacing:-.018em}
.mast h1 em{font-style:italic; color:var(--accent); font-weight:500}
.standfirst{margin:14px 0 0; max-width:60ch; font-size:16px; color:var(--ink-2)}

/* ---------- next up ---------- */
.nextup{
  margin-top:26px; background:var(--surface); border:1px solid var(--rule);
  border-top:4px solid var(--due); border-radius:5px; box-shadow:var(--shadow);
  display:grid; grid-template-columns:1fr auto; gap:18px; padding:20px 22px; align-items:start;
}
.nu-label{font-family:var(--mono); font-size:10.5px; letter-spacing:.13em; text-transform:uppercase; color:var(--due); margin-bottom:7px}
.nu-date{font-family:var(--serif); font-size:22px; font-weight:600; line-height:1.2}
.nu-title{color:var(--ink-2); font-size:15px; margin-top:3px}
.nu-due{
  margin-top:13px; padding:11px 14px; border-radius:4px; background:var(--surface-2);
  border-left:3px solid var(--due); font-size:14.5px; color:var(--ink);
}
.nu-due b{font-family:var(--mono); font-size:10px; letter-spacing:.1em; text-transform:uppercase; color:var(--ink-3); display:block; margin-bottom:4px; font-weight:500}
.nu-count{text-align:right; font-family:var(--mono); white-space:nowrap}
.nu-count .big{font-size:34px; font-weight:500; color:var(--ink); line-height:1; font-variant-numeric:tabular-nums; display:block}
.nu-count .cap{font-size:10.5px; letter-spacing:.1em; text-transform:uppercase; color:var(--ink-3); margin-top:6px; display:block; line-height:1.5}
.jump{
  margin-top:12px; font-family:var(--mono); font-size:11px; letter-spacing:.06em; text-transform:uppercase;
  background:transparent; border:1px solid var(--rule); color:var(--ink-2); padding:7px 11px; border-radius:4px; cursor:pointer;
}
.jump:hover{border-color:var(--due); color:var(--due)}

/* ---------- sections ---------- */
.sec{margin-top:50px}
.sec-head{display:flex; align-items:baseline; justify-content:space-between; gap:20px; flex-wrap:wrap; margin-bottom:8px}
.sec h2{font-size:24px; letter-spacing:-.01em}
.sec-note{font-size:13.5px; color:var(--ink-3); max-width:52ch}

/* ---------- unit nav ---------- */
.units{display:grid; grid-template-columns:repeat(auto-fill,minmax(210px,1fr)); gap:8px; margin-top:16px}
.ubtn{
  display:block; text-align:left; background:var(--surface); border:1px solid var(--rule);
  border-radius:5px; padding:11px 13px; cursor:pointer; font-family:var(--sans); color:var(--ink);
  border-left:3px solid var(--uc);
}
.ubtn:hover{border-color:var(--uc); border-left-color:var(--uc)}
.ubtn[aria-pressed="true"]{background:var(--surface-2); box-shadow:inset 0 0 0 1px var(--uc)}
.ubtn .un{font-family:var(--serif); font-weight:600; font-size:15.5px; display:block; line-height:1.2}
.ubtn .us{font-size:11.5px; color:var(--ink-3); display:block; margin-top:3px; line-height:1.4}
.ubtn .ur{font-family:var(--mono); font-size:11px; color:var(--uc); display:block; margin-top:6px}

.toolbar{display:flex; gap:9px; flex-wrap:wrap; align-items:center; margin-top:16px}
.tbtn{
  font-family:var(--mono); font-size:11.5px; letter-spacing:.06em; text-transform:uppercase;
  background:var(--surface); border:1px solid var(--rule); color:var(--ink-2);
  padding:8px 13px; border-radius:4px; cursor:pointer;
}
.tbtn:hover{border-color:var(--ink-3); color:var(--ink)}
.tbtn[aria-pressed="true"]{background:var(--ink); color:var(--bg); border-color:var(--ink)}
.showing{font-family:var(--mono); font-size:12px; color:var(--ink-3); margin-left:auto; font-variant-numeric:tabular-nums}

/* ---------- progress ---------- */
.prog{margin-top:14px; background:var(--surface); border:1px solid var(--rule-2); border-radius:5px; padding:14px 16px}
.prog-top{display:flex; justify-content:space-between; align-items:baseline; gap:14px; flex-wrap:wrap}
.prog-t{font-size:13.5px; color:var(--ink-2)}
.prog-t strong{color:var(--ink); font-family:var(--mono); font-variant-numeric:tabular-nums}
.prog-bar{height:6px; border-radius:3px; background:var(--surface-3); margin-top:10px; overflow:hidden}
.prog-fill{height:100%; background:var(--good); width:0%; border-radius:3px; transition:width .25s ease}
.prog-note{font-size:12px; color:var(--ink-3); margin-top:8px}
.linkbtn{background:none; border:0; color:var(--ink-3); font-size:12px; text-decoration:underline; cursor:pointer; padding:0; font-family:var(--sans)}
.linkbtn:hover{color:var(--accent)}

/* ---------- schedule ---------- */
.week{margin-top:30px}
.week-bar{display:flex; align-items:baseline; gap:12px; padding-bottom:8px; border-bottom:1px solid var(--rule); margin-bottom:10px}
.week-n{font-family:var(--mono); font-size:11px; letter-spacing:.12em; text-transform:uppercase; color:var(--ink-3)}
.week-r{font-family:var(--serif); font-size:17px; font-weight:600}

.day{
  display:grid; grid-template-columns:92px 1fr;
  background:var(--surface); border:1px solid var(--rule-2); border-left:3px solid var(--uc);
  border-radius:4px; margin-bottom:7px; box-shadow:var(--shadow);
}
.day.is-today{border-color:var(--due); border-left-color:var(--due); box-shadow:0 0 0 2px color-mix(in srgb, var(--due) 30%, transparent), var(--shadow)}
.day.is-past{opacity:.62}
.day-mark{padding:14px 8px 14px 15px; border-right:1px solid var(--rule-2); display:flex; flex-direction:column; gap:3px}
.day-dow{font-family:var(--mono); font-size:11px; letter-spacing:.09em; text-transform:uppercase; color:var(--ink-3)}
.day-md{font-family:var(--serif); font-size:19px; font-weight:600; line-height:1.1}
.day-tag{font-family:var(--mono); font-size:9.5px; letter-spacing:.1em; text-transform:uppercase; color:var(--due); margin-top:3px}
.day-body{padding:13px 16px 14px; min-width:0}

.due{
  display:grid; grid-template-columns:auto 1fr; gap:10px; align-items:start;
  background:var(--surface-2); border-left:3px solid var(--due);
  border-radius:0 4px 4px 0; padding:10px 13px; margin-bottom:11px;
}
.due label{font-size:14px; color:var(--ink); cursor:pointer; line-height:1.45}
.due b{font-family:var(--mono); font-size:9.5px; letter-spacing:.1em; text-transform:uppercase; color:var(--due); display:block; margin-bottom:3px; font-weight:500}
.due input{width:17px; height:17px; margin:2px 0 0; accent-color:var(--good); cursor:pointer}
.due.done{opacity:.55}
.due.done label{text-decoration:line-through}

.day-t{font-family:var(--serif); font-size:18px; font-weight:600; line-height:1.25}
.day-x{margin:5px 0 0; color:var(--ink-2); font-size:14.5px; max-width:70ch}
.day-meta{display:flex; flex-wrap:wrap; gap:7px; margin-top:11px}
.chip{font-family:var(--mono); font-size:10.5px; letter-spacing:.05em; padding:4px 9px; border-radius:3px; white-space:normal}
.chip-poem{
  background:transparent; color:var(--u-poetry); border:1px dashed color-mix(in srgb, var(--u-poetry) 45%, transparent);
  font-family:var(--sans); font-size:12px; font-style:italic; letter-spacing:0;
}
.chip-poem b{font-family:var(--mono); font-style:normal; font-size:9.5px; letter-spacing:.09em; text-transform:uppercase; margin-right:6px; color:var(--ink-3); font-weight:500}
.chip-frq{background:color-mix(in srgb, var(--accent) 12%, transparent); color:var(--accent); border:1px solid color-mix(in srgb, var(--accent) 36%, transparent); font-weight:500}
.chip-mcq{background:var(--surface-2); color:var(--ink-2); border:1px solid var(--rule)}
.chip-task{background:transparent; color:var(--ink-2); border:1px dotted var(--rule)}

.brk{display:flex; align-items:center; gap:14px; margin:9px 0 2px; padding:9px 14px; border:1px dashed var(--rule); border-radius:4px}
.brk-l{font-family:var(--mono); font-size:11px; letter-spacing:.11em; text-transform:uppercase; color:var(--ink-3)}
.brk-d{font-family:var(--serif); font-size:15px; font-style:italic; color:var(--ink-2)}
.brk-t{margin-left:auto; font-family:var(--mono); font-size:10.5px; color:var(--ink-3)}

.examday{margin-top:22px; padding:22px 24px; border-radius:5px; background:var(--ink); color:var(--bg); display:flex; align-items:center; gap:22px; flex-wrap:wrap}
.examday .ed-n{font-family:var(--mono); font-size:11px; letter-spacing:.14em; text-transform:uppercase; opacity:.7}
.examday .ed-t{font-family:var(--serif); font-size:23px; font-weight:600; line-height:1.15}
.examday .ed-s{font-family:var(--mono); font-size:12.5px; opacity:.75; margin-left:auto; text-align:right; line-height:1.6}

/* ---------- panels ---------- */
.panel{background:var(--surface); border:1px solid var(--rule-2); border-radius:5px; padding:22px 24px; margin-top:14px; box-shadow:var(--shadow)}
.tw{overflow-x:auto}
table{border-collapse:collapse; width:100%; font-size:14px; min-width:480px}
th{text-align:left; font-family:var(--mono); font-size:10.5px; letter-spacing:.1em; text-transform:uppercase; color:var(--ink-3); font-weight:500; padding:0 14px 9px 0; border-bottom:1px solid var(--rule); white-space:nowrap}
td{padding:10px 14px 10px 0; border-bottom:1px solid var(--rule-2); vertical-align:top; color:var(--ink-2)}
tr:last-child td{border-bottom:0}
td.k{color:var(--ink); font-weight:500}
td.m{font-family:var(--mono); font-variant-numeric:tabular-nums; white-space:nowrap; font-size:13px}
cite{font-style:italic; font-family:var(--serif)}

.rows{display:grid; gap:12px; margin-top:14px}
.row{background:var(--surface); border:1px solid var(--rule-2); border-radius:5px; padding:18px 20px; box-shadow:var(--shadow); border-left:3px solid var(--uc)}
.row h3{font-size:17px; margin-bottom:3px}
.row .pts{font-family:var(--mono); font-size:11px; letter-spacing:.08em; text-transform:uppercase; color:var(--uc); margin-bottom:8px}
.row p{margin:0 0 8px; color:var(--ink-2); font-size:14.5px; max-width:72ch}
.row p:last-child{margin-bottom:0}
.row .no{color:var(--ink-3); font-size:13.5px; font-style:italic}

.note{border-left:3px solid var(--accent); background:var(--surface-2); padding:16px 20px; border-radius:0 4px 4px 0; margin-top:14px}
.note h3{font-size:16px; margin-bottom:6px}
.note p{margin:0 0 9px; color:var(--ink-2); font-size:14px; max-width:70ch}
.note p:last-child{margin-bottom:0}
.note ul{margin:0; padding-left:18px; color:var(--ink-2); font-size:14px}
.note li{margin-bottom:6px}
.note li:last-child{margin-bottom:0}

.foot{margin-top:56px; padding-top:18px; border-top:1px solid var(--rule); font-size:12.5px; color:var(--ink-3)}

@media (max-width:640px){
  .wrap{padding:0 15px 72px}
  .nextup{grid-template-columns:1fr}
  .nu-count{text-align:left}
  .day{grid-template-columns:1fr}
  .day-mark{flex-direction:row; align-items:baseline; gap:10px; border-right:0; border-bottom:1px solid var(--rule-2); padding:10px 15px}
}
</style>

<div class="wrap">

<header class="mast">
  <p class="eyebrow">AP English Literature &amp; Composition &middot; Mr. Alcorn &middot; Spring 2027</p>
  <h1>Every day, <em>every deadline</em></h1>
  <p class="standfirst">The whole semester is on this page. What&rsquo;s due, when it&rsquo;s due, what we&rsquo;re doing in class, and every graded thing between now and the exam on May 5. Nothing here is a surprise later.</p>
  <div class="nextup" id="nextup"></div>
</header>

<section class="sec" id="jump">
  <div class="sec-head">
    <h2>The semester</h2>
    <p class="sec-note">Tap a unit to see only those days.</p>
  </div>
  <div class="units" id="units"></div>
  <div class="toolbar">
    <button class="tbtn" id="btn-all" aria-pressed="true">Show everything</button>
    <button class="tbtn" id="btn-due" aria-pressed="false">Only days with reading due</button>
    <button class="tbtn" id="btn-grade" aria-pressed="false">Only graded work</button>
    <span class="showing" id="showing"></span>
  </div>
  <div class="prog" id="prog">
    <div class="prog-top">
      <span class="prog-t">Reading checked off: <strong id="prog-n">0 of 64</strong></span>
      <button class="linkbtn" id="prog-clear">Clear all my checkmarks</button>
    </div>
    <div class="prog-bar"><div class="prog-fill" id="prog-fill"></div></div>
    <p class="prog-note">These checkboxes are only for you. They are saved in this browser, on this device, and are never sent to your teacher or anyone else. Clearing your browser data will erase them.</p>
  </div>
</section>

<section class="sec" id="calendar">
  <div class="sec-head">
    <h2>Class by class</h2>
    <p class="sec-note">A reading listed on a date is <strong>due at the start of that class</strong>, not assigned that day.</p>
  </div>
  <div id="weeks"></div>
  <div class="examday">
    <div>
      <div class="ed-n">Wednesday, May 5, 2027 &middot; 8:00 a.m.</div>
      <div class="ed-t">AP English Literature &amp; Composition Exam</div>
    </div>
    <div class="ed-s">55 multiple choice &middot; 60 min<br>3 essays &middot; 120 min</div>
  </div>
</section>

<section class="sec" id="grading">
  <div class="sec-head">
    <h2>How your essays are scored</h2>
    <p class="sec-note">Every AP essay is worth six points, in three rows. Knowing what each row rewards is worth more than any other single thing on this page.</p>
  </div>
  <div class="rows">
    <div class="row" style="--uc:var(--u-fiction)">
      <h3>Row A &mdash; Thesis</h3>
      <div class="pts">1 point &middot; you get it or you don&rsquo;t</div>
      <p>One sentence making a claim about what the text means that a reasonable person could disagree with. That&rsquo;s the whole test. It does not have to be at the end of your first paragraph, and it does not have to be long.</p>
      <p class="no">Earns nothing: restating the prompt, announcing your topic, or listing the devices you plan to point at.</p>
    </div>
    <div class="row" style="--uc:var(--u-poetry)">
      <h3>Row B &mdash; Evidence and commentary</h3>
      <div class="pts">4 points &middot; where the score is actually won</div>
      <p>Specific evidence from the text, plus your explanation of how that evidence supports your line of reasoning. The explanation is the essay. Most students who lose points here quote something accurate and then move on without saying what it does.</p>
      <p>A useful rule: for every sentence of quotation, write at least two sentences that are yours.</p>
    </div>
    <div class="row" style="--uc:var(--u-hamlet)">
      <h3>Row C &mdash; Sophistication</h3>
      <div class="pts">1 point &middot; rare, and worth understanding early</div>
      <p>This is not a reward for big vocabulary or a dramatic conclusion. It is given for a small number of real moves: identifying a tension the text does not resolve, placing your reading inside a broader context, qualifying your own claim, or naming a competing interpretation and answering it.</p>
      <p>We work on exactly these moves on January 25, February 9, April 20, and April 30. They are learnable.</p>
    </div>
  </div>
</section>

<section class="sec" id="reading">
  <div class="sec-head">
    <h2>Reading, and how to do it</h2>
    <p class="sec-note">Three books, roughly forty pages a week during a novel unit.</p>
  </div>
  <div class="panel"><div class="tw"><table>
    <thead><tr><th>Book</th><th>We start</th><th>Finish it by</th><th>Pace</th></tr></thead>
    <tbody>
      <tr><td class="k"><cite>Frankenstein</cite><br><span style="color:var(--ink-3)">Mary Shelley</span></td><td class="m">Thu Feb 11</td><td class="m">Tue Mar 2</td><td>About 2 chapters a night, roughly 18 pages</td></tr>
      <tr><td class="k"><cite>Never Let Me Go</cite><br><span style="color:var(--ink-3)">Kazuo Ishiguro</span></td><td class="m">Mon Mar 8</td><td class="m">Mon Mar 22</td><td>About 2 chapters a night, roughly 28 pages</td></tr>
      <tr><td class="k"><cite>Hamlet</cite><br><span style="color:var(--ink-3)">William Shakespeare</span></td><td class="m">Mon Apr 5</td><td class="m">Tue Apr 20</td><td>Read aloud together in class; homework is rereading one scene</td></tr>
    </tbody>
  </table></div></div>
  <div class="note">
    <h3>What &ldquo;annotate&rdquo; means in this class</h3>
    <p>Not highlighting. Highlighting feels like work and teaches you nothing. What counts is writing in the margin, and there are only three things worth writing:</p>
    <ul>
      <li><strong>A question.</strong> Anything you didn&rsquo;t follow, or any moment a character does something that seems out of character.</li>
      <li><strong>A connection.</strong> This scene is doing what that earlier scene did. This narrator sounds like that one.</li>
      <li><strong>A word that seems chosen.</strong> When a writer picks a strange word over an ordinary one, circle it. Those are your quotations later.</li>
    </ul>
    <p>Six to ten marks a chapter is plenty. Thirty is procrastination.</p>
  </div>
  <div class="note">
    <h3>One rule for <cite>Never Let Me Go</cite></h3>
    <p>Do not look this novel up, and do not let anyone tell you about it &mdash; not a summary, not a review, not a video, not a friend who read it last year. The book is constructed so that you understand it at the same rate its narrator does, and that only works once. If you accidentally read something you shouldn&rsquo;t have, tell me privately; it&rsquo;s not a problem, but I&rsquo;d rather know.</p>
    <p>If you get behind, catch up on the reading before you try to catch up on notes. Everything we do in class assumes you read it.</p>
  </div>
</section>

<section class="sec" id="absent">
  <div class="sec-head">
    <h2>If you were absent</h2>
    <p class="sec-note">In order. Don&rsquo;t start with step three.</p>
  </div>
  <div class="note">
    <ul>
      <li><strong>Check this page first.</strong> Find the day you missed and the next class. The reading due date does not move because you were out.</li>
      <li><strong>Do the reading before anything else.</strong> Notes from a friend are useful only if you have read the text they&rsquo;re about.</li>
      <li><strong>Get the class notes from someone,</strong> then bring me one specific question about what you missed. &ldquo;What did we do?&rdquo; is not that question.</li>
      <li><strong>Timed essays and multiple-choice sections</strong> are made up within five school days, before or after school. Come find me the day you return to schedule it &mdash; I won&rsquo;t chase you.</li>
      <li><strong>Seminars and the performance workshop</strong> can&rsquo;t be recreated. If you miss one, you&rsquo;ll write a response instead; see me for the prompt.</li>
    </ul>
  </div>
</section>

<footer class="foot">
  AP English Literature &amp; Composition &middot; Spring 2027 &middot; Textbook: <cite>Literature &amp; Composition: Essential Voices, Essential Skills for the AP&reg; Course</cite>, 3rd edition. Dates follow the school calendar and may shift for weather; this page is updated when they do.
</footer>

</div>

<script>
const DATA = {"days": [{"n": 1, "iso": "2027-01-06", "dow": "Wed", "md": "Jan 6", "wk": "2027-01-04", "u": "launch", "t": "What this course is actually asking you to do", "d": "We map the exam on day one so none of it is mysterious in May: 55 multiple-choice questions in an hour, then three essays in two hours. You’ll take a short diagnostic so we both know where you’re starting from.", "due": null, "p": null, "a": [{"k": "mcq", "l": "Diagnostic · 11 multiple-choice questions · 15 min · not graded"}]}, {"n": 2, "iso": "2027-01-07", "dow": "Thu", "md": "Jan 7", "wk": "2027-01-04", "u": "launch", "t": "Your baseline essay", "d": "You’ll write for 40 minutes with no instruction beforehand. This one is deliberately not for a grade — it exists so that in May you can look back and measure how far you moved.", "due": "Signed syllabus. Skim the AP Literature scoring rubric.", "p": null, "a": [{"k": "frq", "l": "Baseline essay · 40 min · feedback only, no grade"}]}, {"n": 3, "iso": "2027-01-08", "dow": "Fri", "md": "Jan 8", "wk": "2027-01-04", "u": "fiction", "t": "Character: what people reveal without meaning to", "d": "Oates gives you almost nothing but surface, so inference is the only way in. You’ll practice moving from what a character does, to why, to what the gap between those two tells you.", "due": "Read Joyce Carol Oates, “Where Are You Going, Where Have You Been?”", "p": null, "a": []}, {"n": 4, "iso": "2027-01-11", "dow": "Mon", "md": "Jan 11", "wk": "2027-01-11", "u": "fiction", "t": "Setting: when a place starts doing something", "d": "Setting is not scenery. You’ll find the exact point in Gilman’s story where the room stops being where things happen and starts being what the story is about.", "due": "Textbook Ch. 1 §1 “Setting.” Read Charlotte Perkins Gilman, “The Yellow Wallpaper.”", "p": null, "a": []}, {"n": 5, "iso": "2027-01-12", "dow": "Tue", "md": "Jan 12", "wk": "2027-01-11", "u": "fiction", "t": "Plot: why the order matters", "d": "The same events arranged differently mean different things. You’ll take O’Connor’s story apart and argue about where a writer chooses to begin and what that choice costs.", "due": "Textbook Ch. 1 §1 “Plot.” Read Flannery O’Connor, “A Good Man Is Hard to Find.”", "p": null, "a": []}, {"n": 6, "iso": "2027-01-13", "dow": "Wed", "md": "Jan 13", "wk": "2027-01-11", "u": "fiction", "t": "Point of view: who is telling you this?", "d": "Two contemporary stories break the usual rules — Kochai writes in “you,” Hofler writes in “we.” Narration is the largest single category on the AP exam, so this is the day to get it right.", "due": "Textbook Ch. 1 §1 “Narrative Perspective and Point of View.” Read Kochai, “Playing Metal Gear Solid V: The Phantom Pain” and Hofler, “Erasure.”", "p": null, "a": [{"k": "mcq", "l": "Multiple choice · 11 questions on a prose passage · 13 min · timed"}]}, {"n": 7, "iso": "2027-01-14", "dow": "Thu", "md": "Jan 14", "wk": "2027-01-11", "u": "fiction", "t": "Putting all four together", "d": "“Sonny’s Blues” holds character, setting, plot, and narration at once. You’ll build claim–evidence–commentary chains as a class, then on your own.", "due": "Read James Baldwin, “Sonny’s Blues” up to the brothers’ reunion.", "p": null, "a": [{"k": "task", "l": "Graded · one interpretive claim with two pieces of evidence"}]}, {"n": 8, "iso": "2027-01-15", "dow": "Fri", "md": "Jan 15", "wk": "2027-01-11", "u": "fiction", "t": "Word choice and sentence shape", "d": "Close reading at the smallest scale: why this word instead of a near-synonym, and why this order. You’ll rewrite one of Baldwin’s sentences into plain order and say precisely what got lost.", "due": "Finish “Sonny’s Blues.” Bring your claim and two pieces of evidence.", "p": null, "a": []}, {"n": 9, "iso": "2027-01-19", "dow": "Tue", "md": "Jan 19", "wk": "2027-01-18", "u": "fiction", "t": "Figurative language, tone, and mood", "d": "Naming a device earns you nothing. You’ll practice the part that does count — explaining what the device is doing — and drill the tone/mood distinction until it’s automatic.", "due": "Textbook Ch. 1 §2 close-reading section. Reread Baldwin’s last three pages.", "p": null, "a": []}, {"n": 10, "iso": "2027-01-20", "dow": "Wed", "md": "Jan 20", "wk": "2027-01-18", "u": "fiction", "t": "Writing the prose essay, part 1: the thesis", "d": "How to take a prompt apart and build a thesis someone could actually argue with. You’ll write three competing theses from one passage and defend a ranking of them.", "due": "Textbook Ch. 1 §2, “Crafting an AP Prose Fiction Analysis Essay.”", "p": null, "a": []}, {"n": 11, "iso": "2027-01-21", "dow": "Thu", "md": "Jan 21", "wk": "2027-01-18", "u": "fiction", "t": "Writing the prose essay, part 2: evidence and commentary", "d": "You’ll score real released student essays against the rubric and argue about the scores. Learning to grade an essay is the fastest way to learn to write one.", "due": "Bring your three theses from yesterday.", "p": null, "a": []}, {"n": 12, "iso": "2027-01-22", "dow": "Fri", "md": "Jan 22", "wk": "2027-01-18", "u": "fiction", "t": "First timed essay", "d": "Forty minutes, exam conditions, a passage you have not seen before. You’ll score yourself against the rubric before you leave the room.", "due": null, "p": null, "a": [{"k": "frq", "l": "Timed essay · prose passage · 40 min · graded"}]}, {"n": 13, "iso": "2027-01-25", "dow": "Mon", "md": "Jan 25", "wk": "2027-01-25", "u": "fiction", "t": "The sophistication point, explained", "d": "The hardest rubric row, in plain language: it rewards noticing a tension the text refuses to settle. You’ll revise the weakest paragraph of Friday’s essay to do exactly that.", "due": "Textbook Ch. 1 §3.", "p": null, "a": [{"k": "task", "l": "Graded · revised paragraph + a note on what you changed and why"}]}, {"n": 14, "iso": "2027-01-26", "dow": "Tue", "md": "Jan 26", "wk": "2027-01-25", "u": "poetry", "t": "Say what it literally says first", "d": "The single biggest thing that raises poetry scores: paraphrase every line before interpreting anything. You’ll rewrite tangled syntax into ordinary sentences.", "due": "Textbook Ch. 2 §1, “Reading for Literal Meaning.”", "p": null, "a": []}, {"n": 15, "iso": "2027-01-27", "dow": "Wed", "md": "Jan 27", "wk": "2027-01-25", "u": "poetry", "t": "Who is speaking — and what are they arguing with?", "d": "The speaker is not the poet. Then the machinery of contrast: juxtaposition, antithesis, paradox — how a fourteen-line poem holds two opposed things at once.", "due": "Textbook Ch. 2 §1, “Considering the Speaker,” + assigned poems.", "p": null, "a": []}, {"n": 16, "iso": "2027-01-28", "dow": "Thu", "md": "Jan 28", "wk": "2027-01-25", "u": "poetry", "t": "Tone, mood, and irony", "d": "You’ll hunt for the line where a poem’s attitude turns, and practice catching irony in poems short enough that it’s easy to miss entirely.", "due": "Textbook Ch. 2 §1, “Tone and Mood with Irony.”", "p": null, "a": []}, {"n": 17, "iso": "2027-01-29", "dow": "Fri", "md": "Jan 29", "wk": "2027-01-25", "u": "poetry", "t": "Image, symbol, and the figure that runs a whole poem", "d": "Reading one metaphor across an entire poem instead of device by device. The question we keep asking: what evidence lets you call an image a symbol?", "due": "Textbook Ch. 2 §1, “Reading for Detail and Figurative Language.”", "p": null, "a": []}, {"n": 18, "iso": "2027-02-01", "dow": "Mon", "md": "Feb 1", "wk": "2027-02-01", "u": "poetry", "t": "Structure, and the turn", "d": "Sonnets, villanelles, free verse — and the volta. Finding where a poem changes its mind is the most reliable way to find your thesis.", "due": "Textbook Ch. 2 §1, “Structure, Poetic Syntax, Meter, and Form.”", "p": null, "a": []}, {"n": 19, "iso": "2027-02-02", "dow": "Tue", "md": "Feb 2", "wk": "2027-02-01", "u": "poetry", "t": "Sound, meter, and when to bring it up", "d": "Enough scansion to hear when a poem breaks its own pattern. The rule for the rest of the year: only mention sound if you can tie it to meaning.", "due": "Textbook Ch. 2 §1, “Sound and Rhyme.”", "p": null, "a": []}, {"n": 20, "iso": "2027-02-03", "dow": "Wed", "md": "Feb 3", "wk": "2027-02-01", "u": "poetry", "t": "A poem you have never seen, start to finish", "d": "Everything from the last six classes, applied on your own to an unfamiliar poem in one period, then compared against a partner’s reading.", "due": null, "p": null, "a": [{"k": "mcq", "l": "Multiple choice · 11 questions on a poem · 13 min"}, {"k": "task", "l": "Graded · independent interpretation of the poem"}]}, {"n": 21, "iso": "2027-02-04", "dow": "Thu", "md": "Feb 4", "wk": "2027-02-01", "u": "poetry", "t": "Writing the poetry essay, part 1", "d": "Organizer to thesis. Your thesis has to name something the poem does — a shift, a tension, a reversal — not list the devices it contains.", "due": "Textbook Ch. 2 §2, “Crafting an AP Poetry Analysis Essay.”", "p": null, "a": []}, {"n": 22, "iso": "2027-02-05", "dow": "Fri", "md": "Feb 5", "wk": "2027-02-01", "u": "poetry", "t": "Writing the poetry essay, part 2", "d": "How to quote poetry correctly — line breaks, slashes, line numbers — and a peer review that flags only two things: claims with no support, and quotations with no explanation.", "due": "A full draft of the poetry essay.", "p": null, "a": []}, {"n": 23, "iso": "2027-02-08", "dow": "Mon", "md": "Feb 8", "wk": "2027-02-08", "u": "poetry", "t": "Timed poetry essay", "d": "Forty minutes, exam conditions. Afterward you’ll spend five minutes writing down the one move that would have raised your score.", "due": null, "p": null, "a": [{"k": "frq", "l": "Timed essay · poem · 40 min · graded"}]}, {"n": 24, "iso": "2027-02-09", "dow": "Tue", "md": "Feb 9", "wk": "2027-02-08", "u": "poetry", "t": "Sophistication in poetry", "d": "Placing your reading inside a bigger conversation without inventing outside research, and qualifying a claim so that it comes out stronger rather than softer.", "due": "Textbook Ch. 2 §3.", "p": null, "a": []}, {"n": 25, "iso": "2027-02-10", "dow": "Wed", "md": "Feb 10", "wk": "2027-02-08", "u": "poetry", "t": "Poetry checkpoint", "d": "Revision due, plus the first mixed multiple-choice checkpoint. Results come back broken out by question type so you can see which kind is costing you points.", "due": "Revised poetry essay.", "p": null, "a": [{"k": "mcq", "l": "Checkpoint · 22 questions across a poem and a prose passage · 26 min"}]}, {"n": 26, "iso": "2027-02-11", "dow": "Thu", "md": "Feb 11", "wk": "2027-02-08", "u": "frank", "t": "Frankenstein: where this book comes from", "d": "Before page one — Romanticism, the Prometheus myth, the science of 1818, and the strange summer that produced the novel. We set one question to carry the whole unit: who is telling you this, and how much should you trust them?", "due": "Bring your copy of the novel.", "p": null, "a": []}, {"n": 27, "iso": "2027-02-12", "dow": "Fri", "md": "Feb 12", "wk": "2027-02-08", "u": "frank", "t": "Letters 1–4 · A story inside a story inside a story", "d": "Shelley builds the novel out of nested narrators. You’ll diagram who is telling what to whom, and what each layer lets the book keep from you.", "due": "Frankenstein, Letters 1–4.", "p": null, "a": []}, {"n": 28, "iso": "2027-02-16", "dow": "Tue", "md": "Feb 16", "wk": "2027-02-15", "u": "frank", "t": "Chapters 1–4 · Ambition as characterization", "d": "Victor tells you what kind of person he is well before he does anything. You’ll track the vocabulary of appetite and secrecy from Ingolstadt onward.", "due": "Frankenstein, Chapters 1–4.", "p": null, "a": []}, {"n": 29, "iso": "2027-02-17", "dow": "Wed", "md": "Feb 17", "wk": "2027-02-15", "u": "frank", "t": "Chapters 5–6 · Close reading a famous chapter", "d": "Poem first, then everything you learned in January applied to a single chapter of a novel — diction, syntax, the whole apparatus.", "due": "Frankenstein, Chapters 5–6.", "p": "Percy Shelley, 'Mutability' — quoted inside Chapter 10", "a": []}, {"n": 30, "iso": "2027-02-18", "dow": "Thu", "md": "Feb 18", "wk": "2027-02-15", "u": "frank", "t": "Chapters 7–8 · Landscape as argument", "d": "Mont Blanc, the ice, the laboratory. You’ll argue what the novel’s enormous landscapes are doing to the size of the people standing inside them.", "due": "Frankenstein, Chapters 7–8.", "p": null, "a": []}, {"n": 31, "iso": "2027-02-19", "dow": "Fri", "md": "Feb 19", "wk": "2027-02-15", "u": "frank", "t": "Chapters 9–10 · Whose account is this?", "d": "Narration shifts, and so does where your sympathy sits. You’ll track that movement in yourself and identify the moves on the page that cause it.", "due": "Frankenstein, Chapters 9–10.", "p": null, "a": []}, {"n": 32, "iso": "2027-02-22", "dow": "Mon", "md": "Feb 22", "wk": "2027-02-22", "u": "frank", "t": "Chapters 11–12 · Foils and doubles", "d": "Characters defined against each other. Foil used as a tool rather than a vocabulary word: what does a pairing let a novel say that neither figure could say alone?", "due": "Frankenstein, Chapters 11–12.", "p": null, "a": []}, {"n": 33, "iso": "2027-02-23", "dow": "Tue", "md": "Feb 23", "wk": "2027-02-22", "u": "frank", "t": "Chapters 13–14 · A book inside the book", "d": "Shelley builds Milton’s Paradise Lost into her novel. We’ll read an excerpt of it alongside — borrowing another text is itself a form of characterization.", "due": "Frankenstein, Chapters 13–14.", "p": "Milton, Paradise Lost, Book IX (excerpt)", "a": []}, {"n": 34, "iso": "2027-02-24", "dow": "Wed", "md": "Feb 24", "wk": "2027-02-22", "u": "frank", "t": "Chapters 15–16 · Symbol and allegory", "d": "Poem first, then the discipline of arguing a symbol from repetition and context instead of simply asserting one.", "due": "Frankenstein, Chapters 15–16.", "p": "Percy Shelley, 'Ozymandias' — ruin and the maker's boast", "a": []}, {"n": 35, "iso": "2027-02-25", "dow": "Thu", "md": "Feb 25", "wk": "2027-02-22", "u": "frank", "t": "Chapters 17–18 · Reasoning under pressure", "d": "How a text can present a decision without telling you what to think about it — and what that silence asks of you as a reader. We’ll reread O’Connor’s story alongside.", "due": "Frankenstein, Chapters 17–18.", "p": null, "a": []}, {"n": 36, "iso": "2027-02-26", "dow": "Fri", "md": "Feb 26", "wk": "2027-02-22", "u": "frank", "t": "Chapters 19–20 · Who speaks, and who is spoken for", "d": "The women of this novel and the structure of silence around them. Reread “The Yellow Wallpaper” beside it — the two texts are asking a related question.", "due": "Frankenstein, Chapters 19–20.", "p": null, "a": []}, {"n": 37, "iso": "2027-03-01", "dow": "Mon", "md": "Mar 1", "wk": "2027-03-01", "u": "frank", "t": "Chapters 21–22 · Returning to the frame", "d": "The outermost narrator comes back. You’ll consider what the closing of a frame does to everything held inside it.", "due": "Frankenstein, Chapters 21–22.", "p": null, "a": []}, {"n": 38, "iso": "2027-03-02", "dow": "Tue", "md": "Mar 2", "wk": "2027-03-01", "u": "frank", "t": "Finishing the novel · Building a whole-book interpretation", "d": "You’ll build a thesis about the novel’s central unresolved tension and support it with evidence from all three narrators. Crossing narrators is what makes this hard.", "due": "Frankenstein, Chapters 23–24 and the ending. Finish the novel.", "p": null, "a": [{"k": "task", "l": "Graded · whole-novel interpretation with evidence from all three narrators"}]}, {"n": 39, "iso": "2027-03-03", "dow": "Wed", "md": "Mar 3", "wk": "2027-03-01", "u": "frank", "t": "Preparing Frankenstein for the exam", "d": "Poem first, then the practical part: a scene inventory, a quotation bank you can write from memory, and a one-page sheet. You leave with a document built to answer prompts nobody has written yet.", "due": "Evidence prepared from each of the three narrators.", "p": "Coleridge, 'The Rime of the Ancient Mariner' (excerpt) — Walton's touchstone", "a": []}, {"n": 40, "iso": "2027-03-04", "dow": "Thu", "md": "Mar 4", "wk": "2027-03-01", "u": "frank", "t": "Timed literary argument essay", "d": "Forty minutes on a released prompt, written from memory with no book in the room — exactly like Question 3 on the exam.", "due": "Your finished Frankenstein one-page sheet.", "p": null, "a": [{"k": "frq", "l": "Timed essay · literary argument · 40 min · graded"}]}, {"n": 41, "iso": "2027-03-05", "dow": "Fri", "md": "Mar 5", "wk": "2027-03-01", "u": "frank", "t": "Seminar and checkpoint", "d": "A seminar on the question the novel refuses to settle, then a timed checkpoint that includes a pre-1900 prose passage.", "due": null, "p": null, "a": [{"k": "mcq", "l": "Checkpoint · 22 questions · pre-1900 prose + poetry"}, {"k": "task", "l": "Seminar participation · rubric-scored"}]}, {"n": 42, "iso": "2027-03-08", "dow": "Mon", "md": "Mar 8", "wk": "2027-03-08", "u": "nlmg", "t": "Starting Never Let Me Go", "d": "We open with Le Guin’s five-page story, then begin the novel. One rule for this unit, and it genuinely matters: no summaries, no spoilers, no looking it up. This book is built to be read in order, and it only works once.", "due": "Read Ursula K. Le Guin, “The Ones Who Walk Away from Omelas” (5 pp). Bring the novel.", "p": null, "a": []}, {"n": 43, "iso": "2027-03-09", "dow": "Tue", "md": "Mar 9", "wk": "2027-03-08", "u": "nlmg", "t": "Chapters 1–2 · A narrator remembering", "d": "Kathy tells this looking back, which changes what you are actually being given. Start a running list: what she notices, and what she passes over without comment.", "due": "Never Let Me Go, Chapters 1–2.", "p": null, "a": []}, {"n": 44, "iso": "2027-03-10", "dow": "Wed", "md": "Mar 10", "wk": "2027-03-08", "u": "nlmg", "t": "Chapters 3–4 · Reading for what isn’t said", "d": "Poem first, then close attention to this novel’s vocabulary. You’ll keep a glossary of words the book uses in ways you would not expect.", "due": "Never Let Me Go, Chapters 3–4.", "p": "Philip Larkin, 'Ambulances'", "a": []}, {"n": 45, "iso": "2027-03-11", "dow": "Thu", "md": "Mar 11", "wk": "2027-03-08", "u": "nlmg", "t": "Chapters 5–6 · Art, and what it is asked to prove", "d": "The novel keeps returning to the students’ artwork and to why it matters so much to the adults. You’ll argue what is actually at stake in that.", "due": "Never Let Me Go, Chapters 5–6.", "p": null, "a": []}, {"n": 46, "iso": "2027-03-12", "dow": "Fri", "md": "Mar 12", "wk": "2027-03-08", "u": "nlmg", "t": "Chapters 7–9 · From summary to interpretation", "d": "End of Part One, and textbook Ch. 3 §2 opens. You’ll take five summary-level theses and convert each one into an interpretive claim.", "due": "Never Let Me Go, Chapters 7–9 (end of Part One).", "p": null, "a": []}, {"n": 47, "iso": "2027-03-15", "dow": "Mon", "md": "Mar 15", "wk": "2027-03-15", "u": "nlmg", "t": "Chapters 10–11 · A story to read against this one", "d": "Te-Ping Chen’s “Lulu” beside the novel: two narrators watching someone else make choices they themselves do not make.", "due": "Never Let Me Go, Chapters 10–11. Read Te-Ping Chen, “Lulu” (assigned over the weekend).", "p": null, "a": []}, {"n": 48, "iso": "2027-03-16", "dow": "Tue", "md": "Mar 16", "wk": "2027-03-15", "u": "nlmg", "t": "Chapters 12–13 · Setting and social structure", "d": "Where these characters are, who placed them there, and what they do with the freedom they have. Setting doing work again, at novel scale.", "due": "Never Let Me Go, Chapters 12–13.", "p": null, "a": []}, {"n": 49, "iso": "2027-03-17", "dow": "Wed", "md": "Mar 17", "wk": "2027-03-15", "u": "nlmg", "t": "Chapters 14–15 · Symbol and motif", "d": "Poem first, then the novel’s recurring objects and images — a book that keeps its symbols deliberately quiet, which makes them harder to argue and better to argue about.", "due": "Never Let Me Go, Chapters 14–15.", "p": "Keats, 'Ode on a Grecian Urn' — arrested life, art as evidence", "a": []}, {"n": 50, "iso": "2027-03-18", "dow": "Thu", "md": "Mar 18", "wk": "2027-03-15", "u": "nlmg", "t": "Chapters 16–17 · Thesis and topic sentences", "d": "End of Part Two. Textbook Ch. 3 §2 on topic sentences that move an argument forward instead of announcing a new subject.", "due": "Never Let Me Go, Chapters 16–17 (end of Part Two).", "p": null, "a": []}, {"n": 51, "iso": "2027-03-19", "dow": "Fri", "md": "Mar 19", "wk": "2027-03-15", "u": "nlmg", "t": "Chapters 18–20 · Evidence and commentary", "d": "The difference between quoting and using. You’ll rebuild one weak body paragraph across three timed passes, adding only commentary each time.", "due": "Never Let Me Go, Chapters 18–20.", "p": null, "a": []}, {"n": 52, "iso": "2027-03-22", "dow": "Mon", "md": "Mar 22", "wk": "2027-03-22", "u": "nlmg", "t": "Finishing the novel · Paired seminar", "d": "Poem first, then a seminar setting this novel beside Frankenstein. Come with two pieces of evidence from each book — you will be called on.", "due": "Never Let Me Go, Chapters 21–23. Finish the novel.", "p": "Auden, 'Musée des Beaux Arts' — suffering that goes unattended", "a": [{"k": "task", "l": "Seminar participation · rubric-scored"}]}, {"n": 53, "iso": "2027-03-23", "dow": "Tue", "md": "Mar 23", "wk": "2027-03-22", "u": "nlmg", "t": "Full-process literary argument essay", "d": "Plan, draft, peer review — untimed on purpose, so the process gets taught before you have to compress it into forty minutes.", "due": "Two pieces of evidence from each novel.", "p": null, "a": [{"k": "task", "l": "Graded on process · plan, draft, revision"}]}, {"n": 54, "iso": "2027-03-24", "dow": "Wed", "md": "Mar 24", "wk": "2027-03-22", "u": "nlmg", "t": "Timed literary argument essay", "d": "Forty minutes from memory, no book in the room. You choose which novel to write on — and choosing well is itself a skill.", "due": "Your finished draft from yesterday.", "p": null, "a": [{"k": "frq", "l": "Timed essay · literary argument · 40 min · graded"}]}, {"n": 55, "iso": "2027-03-25", "dow": "Thu", "md": "Mar 25", "wk": "2027-03-22", "u": "nlmg", "t": "First full-length multiple-choice section", "d": "Fifty-five questions in sixty minutes — the real length, with real pacing pressure. We analyze results by question type immediately, then update your text sheets before break.", "due": null, "p": null, "a": [{"k": "mcq", "l": "Full section · 55 questions · 60 min · graded"}]}, {"n": 56, "iso": "2027-04-05", "dow": "Mon", "md": "Apr 5", "wk": "2027-04-05", "u": "hamlet", "t": "Hamlet: revenge tragedy, and how to read Shakespeare", "d": "Genre conventions first, then the toolkit — verse against prose, and what a soliloquy is actually for. We read Act I, scenes i–ii aloud in class today. Most of this play we read together; homework is rereading.", "due": "Bring your copy of the play.", "p": null, "a": []}, {"n": 57, "iso": "2027-04-06", "dow": "Tue", "md": "Apr 6", "wk": "2027-04-05", "u": "hamlet", "t": "Act I, scenes iii–v", "d": "On our feet. What exactly is Hamlet being asked to do, and on what terms? We’ll reread Kochai’s story beside it — a son handed an impossible task.", "due": "Nothing new. Reread Act I, scenes i–ii if you can.", "p": null, "a": []}, {"n": 58, "iso": "2027-04-07", "dow": "Wed", "md": "Apr 7", "wk": "2027-04-05", "u": "hamlet", "t": "Act II, scene i · A soliloquy read as a poem", "d": "Today’s poem is a Hamlet soliloquy given the full poetry treatment — paraphrase, speaker, structure, sound. Proof that January’s poetry unit was never a separate subject.", "due": "Reread Act I, scene v. Mark the conditions Hamlet sets for himself.", "p": "Shakespeare, 'O that this too too solid flesh' (I.ii.129–159)", "a": []}, {"n": 59, "iso": "2027-04-08", "dow": "Thu", "md": "Apr 8", "wk": "2027-04-05", "u": "hamlet", "t": "Act II, scene ii · Watching and being watched", "d": "Almost everyone in this play is observing someone else. The Players arrive, and acting becomes the play’s central idea about honesty.", "due": "Read Act II, scene i.", "p": null, "a": []}, {"n": 60, "iso": "2027-04-09", "dow": "Fri", "md": "Apr 9", "wk": "2027-04-05", "u": "hamlet", "t": "Act III, scene i · Two filmed versions", "d": "A close read of the most quoted speech in English, then two filmed performances compared shot by shot. Staging is interpretation — you’ll argue which reading the text supports.", "due": "Reread the Hecuba speech in Act II, scene ii.", "p": null, "a": []}, {"n": 61, "iso": "2027-04-12", "dow": "Mon", "md": "Apr 12", "wk": "2027-04-12", "u": "hamlet", "t": "Act III, scene ii · A play inside the play", "d": "A frame inside a frame — the same structural question you worked through in Frankenstein, now in drama, where you watch an audience watching.", "due": "Read Act III, scene i.", "p": null, "a": []}, {"n": 62, "iso": "2027-04-13", "dow": "Tue", "md": "Apr 13", "wk": "2027-04-12", "u": "hamlet", "t": "Act III, scenes iii–iv · Motive and dramatic irony", "d": "Two scenes where you know more than the people on stage do. You’ll track what that knowledge does to your sympathy, minute by minute.", "due": "Reread Act III, scene ii.", "p": null, "a": []}, {"n": 63, "iso": "2027-04-14", "dow": "Wed", "md": "Apr 14", "wk": "2027-04-12", "u": "hamlet", "t": "Act IV, scenes i–iv · Critical lenses, part 1", "d": "Poem first, then textbook Ch. 3 §3: reading through a psychological lens, and the difference between using a lens and forcing one onto a text that doesn’t reward it.", "due": "Read Act III, scenes iii–iv.", "p": "Shakespeare, Sonnet 30 — memory, grief, and account-keeping", "a": []}, {"n": 64, "iso": "2027-04-15", "dow": "Thu", "md": "Apr 15", "wk": "2027-04-12", "u": "hamlet", "t": "Act IV, scenes v–vii · Critical lenses, part 2", "d": "Gendered and cultural readings of the play, against both its own period and ours. You’ll argue which interpretation the play supports and where it resists you.", "due": "Read Act IV, scenes i–iv.", "p": null, "a": []}, {"n": 65, "iso": "2027-04-16", "dow": "Fri", "md": "Apr 16", "wk": "2027-04-12", "u": "hamlet", "t": "Act V, scene i · Comedy inside a tragedy", "d": "The graveyard scene, and why Shakespeare puts jokes here of all places. You’ll name the tonal shift and defend what it accomplishes.", "due": "Read Act IV, scenes v–vii.", "p": null, "a": []}, {"n": 66, "iso": "2027-04-19", "dow": "Mon", "md": "Apr 19", "wk": "2027-04-19", "u": "hamlet", "t": "Act V, scene ii · Finishing the play", "d": "How the ending lands, and what it deliberately leaves unsettled for the audience to argue about on the way out.", "due": "Reread Act V, scene i and mark the tonal shift.", "p": null, "a": []}, {"n": 67, "iso": "2027-04-20", "dow": "Tue", "md": "Apr 20", "wk": "2027-04-19", "u": "hamlet", "t": "Answering a reading you disagree with", "d": "Textbook Ch. 3 §3: how to name a competing interpretation and answer it. This is the most reliable route to the sophistication point, and the hardest one to fake.", "due": "Finish the play.", "p": null, "a": []}, {"n": 68, "iso": "2027-04-21", "dow": "Wed", "md": "Apr 21", "wk": "2027-04-19", "u": "hamlet", "t": "Performance workshop", "d": "In groups you’ll stage twenty lines and defend one interpretive choice in writing. Blocking, pace, and what you cut are all arguments about meaning.", "due": "Draft one paragraph arguing against your own reading of the play.", "p": null, "a": [{"k": "task", "l": "Graded · performance + written rationale"}]}, {"n": 69, "iso": "2027-04-22", "dow": "Thu", "md": "Apr 22", "wk": "2027-04-19", "u": "hamlet", "t": "Timed literary argument essay", "d": "Forty minutes on Hamlet, from memory. Third and last one before the exam — by now the process should be automatic and the thinking is where your time goes.", "due": null, "p": null, "a": [{"k": "frq", "l": "Timed essay · literary argument · 40 min · graded"}]}, {"n": 70, "iso": "2027-04-23", "dow": "Fri", "md": "Apr 23", "wk": "2027-04-19", "u": "hamlet", "t": "Three-text seminar · Exam sheets due", "d": "What each of the three works is best at answering. You’ll finalize a one-page sheet per text — five scenes, eight quotations, six themes. This is the document you will think with on May 5.", "due": null, "p": null, "a": [{"k": "task", "l": "Due · one-page sheet for each of the three works"}]}, {"n": 71, "iso": "2027-04-26", "dow": "Mon", "md": "Apr 26", "wk": "2027-04-26", "u": "review", "t": "Full multiple-choice section", "d": "Fifty-five questions in sixty minutes, then analysis by question type. The score is not the point — finding your two weakest categories is.", "due": null, "p": null, "a": [{"k": "mcq", "l": "Full section · 55 questions · 60 min · graded"}]}, {"n": 72, "iso": "2027-04-27", "dow": "Tue", "md": "Apr 27", "wk": "2027-04-26", "u": "review", "t": "Multiple-choice clinic", "d": "Targeted work on whatever yesterday exposed. Question types, elimination, and pacing — roughly thirteen minutes per passage, plus a plan for when one set goes badly.", "due": null, "p": null, "a": []}, {"n": 73, "iso": "2027-04-28", "dow": "Wed", "md": "Apr 28", "wk": "2027-04-26", "u": "review", "t": "Timed poetry essay, peer-scored", "d": "Forty minutes, then you score a classmate’s essay with the official rubric, then compare your score against a released College Board sample.", "due": null, "p": null, "a": [{"k": "frq", "l": "Timed essay · poem · 40 min · peer-scored"}]}, {"n": 74, "iso": "2027-04-29", "dow": "Thu", "md": "Apr 29", "wk": "2027-04-26", "u": "review", "t": "Timed prose essay, peer-scored", "d": "Same protocol as yesterday. Two days of scoring other people’s essays will calibrate you faster than a whole semester of receiving grades on your own.", "due": null, "p": null, "a": [{"k": "frq", "l": "Timed essay · prose passage · 40 min · peer-scored"}]}, {"n": 75, "iso": "2027-04-30", "dow": "Fri", "md": "Apr 30", "wk": "2027-04-26", "u": "review", "t": "The sophistication clinic", "d": "Eight moves that actually earn the sophistication point, each shown with a real example from this class’s essays this semester. You’ll revise one paragraph from each of your three argument essays.", "due": "All three of your literary argument essays.", "p": null, "a": []}, {"n": 76, "iso": "2027-05-03", "dow": "Mon", "md": "May 3", "wk": "2027-05-03", "u": "review", "t": "Full essay section at exam pace", "d": "The whole block run as a simulation — two complete essays plus one full plan, at real speed. The debrief is entirely about time, not content.", "due": null, "p": null, "a": [{"k": "frq", "l": "Timed · two essays + one plan at exam pace"}]}, {"n": 77, "iso": "2027-05-04", "dow": "Tue", "md": "May 4", "wk": "2027-05-03", "u": "review", "t": "The day before", "d": "Logistics, a timing plan written on paper, the five-minute planning rule, and what to do when a passage makes no sense on the first read. Everything gets returned. No new material.", "due": "Nothing. Sleep.", "p": null, "a": []}], "units": [{"k": "launch", "name": "Getting started", "sub": "How the course and the exam work", "days": 2, "range": "Jan 6 – Jan 7"}, {"k": "fiction", "name": "Short fiction", "sub": "Six stories, and how to read closely", "days": 11, "range": "Jan 8 – Jan 25"}, {"k": "poetry", "name": "Poetry", "sub": "Reading and writing about poems", "days": 12, "range": "Jan 26 – Feb 10"}, {"k": "frank", "name": "Frankenstein", "sub": "Mary Shelley · read at home, discussed in class", "days": 16, "range": "Feb 11 – Mar 5"}, {"k": "nlmg", "name": "Never Let Me Go", "sub": "Kazuo Ishiguro · read at home, discussed in class", "days": 14, "range": "Mar 8 – Mar 25"}, {"k": "hamlet", "name": "Hamlet", "sub": "Shakespeare · read aloud together in class", "days": 15, "range": "Apr 5 – Apr 23"}, {"k": "review", "name": "Exam review", "sub": "Full-length practice before May 5", "days": 7, "range": "Apr 26 – May 4"}], "weeks": [{"wk": "2027-01-04", "num": 1, "range": "Jan 6 – Jan 8", "count": 3}, {"wk": "2027-01-11", "num": 2, "range": "Jan 11 – Jan 15", "count": 5}, {"wk": "2027-01-18", "num": 3, "range": "Jan 19 – Jan 22", "count": 4}, {"wk": "2027-01-25", "num": 4, "range": "Jan 25 – Jan 29", "count": 5}, {"wk": "2027-02-01", "num": 5, "range": "Feb 1 – Feb 5", "count": 5}, {"wk": "2027-02-08", "num": 6, "range": "Feb 8 – Feb 12", "count": 5}, {"wk": "2027-02-15", "num": 7, "range": "Feb 16 – Feb 19", "count": 4}, {"wk": "2027-02-22", "num": 8, "range": "Feb 22 – Feb 26", "count": 5}, {"wk": "2027-03-01", "num": 9, "range": "Mar 1 – Mar 5", "count": 5}, {"wk": "2027-03-08", "num": 10, "range": "Mar 8 – Mar 12", "count": 5}, {"wk": "2027-03-15", "num": 11, "range": "Mar 15 – Mar 19", "count": 5}, {"wk": "2027-03-22", "num": 12, "range": "Mar 22 – Mar 25", "count": 4}, {"wk": "2027-04-05", "num": 13, "range": "Apr 5 – Apr 9", "count": 5}, {"wk": "2027-04-12", "num": 14, "range": "Apr 12 – Apr 16", "count": 5}, {"wk": "2027-04-19", "num": 15, "range": "Apr 19 – Apr 23", "count": 5}, {"wk": "2027-04-26", "num": 16, "range": "Apr 26 – Apr 30", "count": 5}, {"wk": "2027-05-03", "num": 17, "range": "May 3 – May 4", "count": 2}], "breaks": [{"wk": "2027-01-18", "label": "MLK Day", "range": "Jan 18", "after": "2027-01-17"}, {"wk": "2027-02-15", "label": "Presidents Day / teacher workday", "range": "Feb 15", "after": "2027-02-14"}, {"wk": "2027-03-22", "label": "Good Friday", "range": "Mar 26", "after": "2027-03-25"}, {"wk": "2027-03-29", "label": "Spring Break", "range": "Mar 29 – Apr 2", "after": "2027-03-28"}], "exam": "2027-05-05", "first": "2027-01-06", "last": "2027-05-04"};
const U = {}; DATA.units.forEach(u => U[u.k] = u);
const state = { unit: null, due: false, grade: false };

/* ---------- text helpers ---------- */
const KIND = { frq:'chip-frq', mcq:'chip-mcq', task:'chip-task' };
const esc = s => String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;');
function ital(s){
  return s.replace(/Frankenstein/g, '<cite>Frankenstein</cite>')
          .replace(/Never Let Me Go/g, '<cite>Never Let Me Go</cite>')
          .replace(/Paradise Lost/g, '<cite>Paradise Lost</cite>')
          .replace(/\bHamlet\b(?!\u2019s)/g, '<cite>Hamlet</cite>');
}

/* ---------- today ---------- */
function localISO(d){
  return d.getFullYear() + '-' + String(d.getMonth()+1).padStart(2,'0') + '-' + String(d.getDate()).padStart(2,'0');
}
const TODAY = localISO(new Date());
const EXAM = DATA.exam;
function daysBetween(a, b){
  return Math.round((new Date(b + 'T00:00:00') - new Date(a + 'T00:00:00')) / 86400000);
}

/* ---------- saved checkmarks (this browser only) ---------- */
const KEY = 'aplit-spring-2027-reading';
let done = {};
try { done = JSON.parse(localStorage.getItem(KEY) || '{}') || {}; } catch (e) { done = {}; }
function save(){ try { localStorage.setItem(KEY, JSON.stringify(done)); } catch (e) {} }

const dueDays = DATA.days.filter(d => d.due && d.due !== 'Nothing. Sleep.');
function updateProgress(){
  const n = dueDays.filter(d => done[d.n]).length;
  document.getElementById('prog-n').textContent = n + ' of ' + dueDays.length;
  document.getElementById('prog-fill').style.width = (dueDays.length ? n / dueDays.length * 100 : 0) + '%';
}

/* ---------- next up ---------- */
const upcoming = DATA.days.find(d => d.iso >= TODAY);
(function renderNextUp(){
  const el = document.getElementById('nextup');
  const toExam = daysBetween(TODAY, EXAM);
  let label, day;
  if (!upcoming) {
    el.innerHTML = '<div><div class="nu-label">That’s the semester</div>' +
      '<div class="nu-date">The exam is behind you</div>' +
      '<div class="nu-title">Whatever the score, you read three hard books and wrote ten essays under time. That part is real.</div></div>';
    return;
  }
  day = upcoming;
  if (day.iso === TODAY) label = 'Today in class';
  else if (TODAY < DATA.first) label = 'First day of the semester';
  else label = 'Next class';

  const dt = new Date(day.iso + 'T00:00:00');
  const full = dt.toLocaleDateString('en-US', { weekday:'long', month:'long', day:'numeric' });
  let due = '';
  if (day.due && day.due !== 'Nothing. Sleep.')
    due = '<div class="nu-due"><b>Due at the start of class</b>' + ital(esc(day.due)) + '</div>';
  else
    due = '<div class="nu-due"><b>Due at the start of class</b>Nothing new — come ready to work.</div>';

  const count = toExam > 0
    ? '<span class="big">' + toExam + '</span><span class="cap">days until<br>the AP exam</span>'
    : '<span class="big">—</span><span class="cap">exam day</span>';

  el.innerHTML =
    '<div><div class="nu-label">' + label + '</div>' +
    '<div class="nu-date">' + full + '</div>' +
    '<div class="nu-title">' + ital(esc(day.t)) + '</div>' + due +
    '<button class="jump" id="btn-jump">Jump to this day</button></div>' +
    '<div class="nu-count">' + count + '</div>';
  document.getElementById('btn-jump').addEventListener('click', () => {
    state.unit = null; state.due = false; state.grade = false; render();
    const target = document.getElementById('day-' + day.n);
    if (target) target.scrollIntoView({ behavior:'smooth', block:'center' });
  });
})();

/* ---------- unit nav ---------- */
const unitsEl = document.getElementById('units');
DATA.units.forEach(u => {
  const b = document.createElement('button');
  b.className = 'ubtn';
  b.style.setProperty('--uc', 'var(--u-' + u.k + ')');
  b.setAttribute('aria-pressed', 'false');
  b.dataset.unit = u.k;
  b.innerHTML = '<span class="un">' + u.name + '</span><span class="us">' + u.sub +
    '</span><span class="ur">' + u.range + ' · ' + u.days + ' classes</span>';
  b.addEventListener('click', () => { state.unit = (state.unit === u.k) ? null : u.k; render(); });
  unitsEl.appendChild(b);
});

document.getElementById('btn-all').addEventListener('click', () => {
  state.unit = null; state.due = false; state.grade = false; render();
});
document.getElementById('btn-due').addEventListener('click', () => {
  state.due = !state.due; if (state.due) state.grade = false; render();
});
document.getElementById('btn-grade').addEventListener('click', () => {
  state.grade = !state.grade; if (state.grade) state.due = false; render();
});
document.getElementById('prog-clear').addEventListener('click', () => {
  done = {}; save(); render(); updateProgress();
});

/* ---------- rendering ---------- */
function dayCard(d){
  const el = document.createElement('article');
  el.className = 'day' + (d.iso === TODAY ? ' is-today' : '') + (d.iso < TODAY ? ' is-past' : '');
  el.id = 'day-' + d.n;
  el.style.setProperty('--uc', 'var(--u-' + d.u + ')');

  let dueHTML = '';
  if (d.due && d.due !== 'Nothing. Sleep.') {
    const isDone = !!done[d.n];
    dueHTML = '<div class="due' + (isDone ? ' done' : '') + '">' +
      '<input type="checkbox" id="chk-' + d.n + '"' + (isDone ? ' checked' : '') +
      ' aria-label="Mark this reading done"><label for="chk-' + d.n + '">' +
      '<b>Due today</b>' + ital(esc(d.due)) + '</label></div>';
  }

  let meta = '';
  if (d.p) meta += '<span class="chip chip-poem"><b>Poem in class</b>' + esc(d.p) + '</span>';
  d.a.forEach(a => { meta += '<span class="chip ' + KIND[a.k] + '">' + esc(a.l) + '</span>'; });

  el.innerHTML =
    '<div class="day-mark"><div class="day-dow">' + d.dow + '</div>' +
    '<div class="day-md">' + d.md + '</div>' +
    (d.iso === TODAY ? '<div class="day-tag">Today</div>' : '') + '</div>' +
    '<div class="day-body">' + dueHTML +
    '<h3 class="day-t">' + ital(esc(d.t)) + '</h3>' +
    '<p class="day-x">' + ital(esc(d.d)) + '</p>' +
    (meta ? '<div class="day-meta">' + meta + '</div>' : '') + '</div>';

  const box = el.querySelector('input');
  if (box) box.addEventListener('change', () => {
    if (box.checked) done[d.n] = true; else delete done[d.n];
    save();
    el.querySelector('.due').classList.toggle('done', box.checked);
    updateProgress();
  });
  return el;
}

const weeksEl = document.getElementById('weeks');
function render(){
  const days = DATA.days.filter(d =>
    (!state.unit || d.u === state.unit) &&
    (!state.due || (d.due && d.due !== 'Nothing. Sleep.')) &&
    (!state.grade || d.a.length)
  );
  weeksEl.innerHTML = '';
  DATA.weeks.forEach(w => {
    const ds = days.filter(d => d.wk === w.wk);
    if (!ds.length) return;
    const sec = document.createElement('section');
    sec.className = 'week';
    sec.innerHTML = '<div class="week-bar"><span class="week-n">Week ' + w.num +
      '</span><span class="week-r">' + w.range + '</span></div>';
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
  document.getElementById('showing').textContent =
    days.length + ' of ' + DATA.days.length + ' classes' + (state.unit ? ' · ' + U[state.unit].name : '');
  document.querySelectorAll('.ubtn').forEach(b =>
    b.setAttribute('aria-pressed', String(b.dataset.unit === state.unit)));
  document.getElementById('btn-all').setAttribute('aria-pressed', String(!state.unit && !state.due && !state.grade));
  document.getElementById('btn-due').setAttribute('aria-pressed', String(state.due));
  document.getElementById('btn-grade').setAttribute('aria-pressed', String(state.grade));
}

render();
updateProgress();
</script>

</body>
</html>
