<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover">
<title>SLLC Online Course — Imagine1Day</title>
<meta name="description" content="School-Based Literacy and Language Club implementation course for Ethiopian primary schools (Grades 1–8).">
<meta name="theme-color" content="#0d6b50" media="(prefers-color-scheme: light)">
<meta name="theme-color" content="#0e1612" media="(prefers-color-scheme: dark)">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Atkinson+Hyperlegible:wght@400;700&family=Bricolage+Grotesque:opsz,wght@12..96,600;12..96,800&display=swap">
<script>
try {
  var t = localStorage.getItem('sllc-theme');
  if (t === 'light' || t === 'dark') document.documentElement.dataset.theme = t;
} catch (e) {}
</script>
<style>
:root{color-scheme:light;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px);
  --bg:#f5f7f4; --surface:#ffffff; --surface2:#eaf0ec; --ink:#14201b; --muted:#53635b; --line:#d3ddd6;
  --accent:#0d6b50; --accent-ink:#ffffff; --sun:#f0b323; --sun-ink:#3a2a00; --good:#13795b; --bad:#b3261e; --good-bg:#e1f3ec; --bad-bg:#fbe6e4;
  --head:"Bricolage Grotesque","Atkinson Hyperlegible",system-ui,sans-serif; --body:"Atkinson Hyperlegible",system-ui,-apple-system,"Segoe UI",sans-serif;
}
@media (prefers-color-scheme: dark){:root:not([data-theme="light"]){
  --bg:#0e1612; --surface:#16211b; --surface2:#1e2c25; --ink:#e8f0eb; --muted:#9db0a5; --line:#2c3d34;
  --accent:#3fbf93; --accent-ink:#06231a; --sun:#f0b323; --sun-ink:#3a2a00; --good:#4fd1a1; --bad:#ff8a80; --good-bg:#12372b; --bad-bg:#40201d; color-scheme:dark}}
:root[data-theme="dark"]{
  --bg:#0e1612; --surface:#16211b; --surface2:#1e2c25; --ink:#e8f0eb; --muted:#9db0a5; --line:#2c3d34;
  --accent:#3fbf93; --accent-ink:#06231a; --sun:#f0b323; --sun-ink:#3a2a00; --good:#4fd1a1; --bad:#ff8a80; --good-bg:#12372b; --bad-bg:#40201d; color-scheme:dark}
html{scroll-padding-top:calc(env(safe-area-inset-top,0px) + 64px)}
*,*::before,*::after{box-sizing:border-box}
img{max-width:100%}
[hidden]:not([hidden=until-found i]){display:none!important}
body{background:var(--bg);color:var(--ink);font:16px/1.6 var(--body);margin:0;padding-block:0 48px;padding-left:max(16px,env(safe-area-inset-left,0px));padding-right:max(16px,env(safe-area-inset-right,0px))}
body::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);background:var(--surface);z-index:30}
h1,h2,h3{font-family:var(--head);line-height:1.15;text-wrap:balance;margin:0}
h1{font-size:clamp(2rem,5vw,3.2rem);font-weight:800;letter-spacing:-.02em}
h2{font-size:1.6rem;font-weight:800;letter-spacing:-.01em}
h3{font-size:1.15rem;font-weight:600}
p{margin:0}
a{color:var(--accent)}
[tabindex="-1"]:focus{outline:none}
.skip{position:absolute;left:-999px;top:env(safe-area-inset-top,0px);z-index:100;background:var(--accent);color:var(--accent-ink);padding:10px 16px;text-decoration:none;font-weight:700;border-radius:0 0 10px 0}
.skip:focus{left:0}
.wrap{max-width:1100px;margin:0 auto}
header.top{position:sticky;top:env(safe-area-inset-top,0px);z-index:20;background:var(--surface);border-bottom:1px solid var(--line);margin-inline:calc(-1*max(16px,env(safe-area-inset-left,0px)));padding-inline:max(16px,env(safe-area-inset-left,0px))}
.bar{max-width:1100px;margin:0 auto;display:flex;align-items:center;gap:16px;flex-wrap:wrap;padding:10px 0}
.brand{font-family:var(--head);font-weight:800;font-size:1.1rem;margin-right:auto;display:flex;align-items:center;gap:10px;text-decoration:none;color:var(--ink)}
.mark{width:30px;height:30px;border-radius:8px;background:var(--accent);color:var(--accent-ink);display:grid;place-items:center;font-size:.95rem}
nav{display:flex;gap:4px;flex-wrap:wrap}
nav a{padding:8px 12px;border-radius:8px;text-decoration:none;color:var(--muted);font-weight:700;font-size:.95rem}
nav a[aria-current="page"]{background:var(--surface2);color:var(--ink)}
nav a:hover{color:var(--ink)}
:focus-visible{outline:3px solid var(--sun);outline-offset:2px}
button,.btn{font:inherit;font-weight:700;border-radius:10px;border:1px solid var(--line);background:var(--surface);color:var(--ink);padding:10px 16px;cursor:pointer;text-decoration:none;display:inline-flex;align-items:center;gap:8px;min-height:44px}
button:hover,.btn:hover{border-color:var(--accent)}
.primary{background:var(--accent);color:var(--accent-ink);border-color:var(--accent)}
.primary:hover{filter:brightness(1.08)}
.sun{background:var(--sun);color:var(--sun-ink);border-color:var(--sun)}
button[disabled]{opacity:.5;cursor:not-allowed}
.theme-btn{min-height:40px;min-width:40px;padding:0 8px;font-size:1.15rem;line-height:1;border-radius:10px}
input[type=text],input[type=email],input[type=password],input[type=url]{font:inherit;width:100%;padding:11px 12px;border-radius:10px;border:1px solid var(--line);background:var(--bg);color:var(--ink);min-height:44px}
label{display:block;font-weight:700;margin-bottom:4px;font-size:.95rem}
.field{display:grid;gap:2px;margin-bottom:14px}
.hint{color:var(--muted);font-size:.9rem}
.card{background:var(--surface);border:1px solid var(--line);border-radius:14px;padding:22px}
.row{display:flex;gap:12px;flex-wrap:wrap;align-items:center}
.grid2{display:grid;grid-template-columns:1fr 1fr;gap:20px}
.stack{display:grid;gap:16px}
.pill{display:inline-block;font-size:.8rem;font-weight:700;padding:2px 10px;border-radius:99px;background:var(--surface2);color:var(--muted);letter-spacing:.02em}
.pill.ok{background:var(--good-bg);color:var(--good)}
.pill.warn{background:var(--sun);color:var(--sun-ink)}
.msg{padding:12px 14px;border-radius:10px;font-weight:700}
.msg.bad{background:var(--bad-bg);color:var(--bad)} .msg.good{background:var(--good-bg);color:var(--good)} .msg.info{background:var(--surface2);color:var(--ink);font-weight:400}
.hero{padding:44px 0 28px;display:grid;gap:16px;max-width:760px}
.hero p.lead{font-size:1.15rem;color:var(--muted)}
.copybox{background:var(--bg);border:1px dashed var(--line);border-radius:10px;padding:12px;font-family:ui-monospace,Menlo,Consolas,monospace;font-size:.85rem;white-space:pre-wrap;word-break:break-word;user-select:all}
.course{display:grid;grid-template-columns:290px minmax(0,1fr);gap:24px;padding-top:24px;align-items:start}
.rail{position:sticky;top:calc(env(safe-area-inset-top,0px) + 70px);display:grid;gap:4px;max-height:calc(100vh - 100px);overflow:auto}
.rail button{justify-content:flex-start;text-align:left;border:1px solid transparent;background:none;font-weight:400;padding:9px 10px;border-radius:10px;width:100%;line-height:1.3}
.rail button[aria-current="true"]{background:var(--surface2);border-color:var(--line);font-weight:700}
.rail button[disabled]{opacity:0.5;cursor:not-allowed;}
.rail .n{flex:0 0 26px;height:26px;border-radius:50%;display:grid;place-items:center;font-size:.8rem;font-weight:700;background:var(--surface2);color:var(--muted)}
.lesson{display:grid;gap:22px;min-width:0}
.lesson ul{margin:0;padding-left:1.2rem;display:grid;gap:6px}
.tablewrap{overflow-x:auto;border:1px solid var(--line);border-radius:10px}
table{border-collapse:collapse;width:100%;min-width:520px;font-size:.95rem}
th,td{text-align:left;padding:10px 12px;border-bottom:1px solid var(--line);vertical-align:top}
th{background:var(--surface2);font-family:var(--head)}
tr:last-child td{border-bottom:0}
.q{border:1px solid var(--line);border-radius:12px;padding:16px;display:grid;gap:10px;background:var(--surface);min-width:0}
.q legend{font-weight:700;padding:0 4px}
fieldset{border:0;margin:0;padding:0;min-width:0}
.opt{display:flex;gap:10px;align-items:flex-start;padding:10px 12px;border:1px solid var(--line);border-radius:10px;cursor:pointer;font-weight:400;margin:0}
.opt input{margin-top:5px;accent-color:var(--accent)}
.opt.right{border-color:var(--good);background:var(--good-bg)}
.opt.wrong{border-color:var(--bad);background:var(--bad-bg)}
.why{font-size:.92rem;color:var(--muted)}
.cert{background:#fffdf5;color:#1d2b24;border:1px solid var(--line);border-radius:6px;overflow:hidden}
.res{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:12px;padding:0;margin:0;list-style:none}
.res a{display:grid;gap:4px;height:100%;padding:14px;border:1px solid var(--line);border-radius:12px;background:var(--surface);text-decoration:none;color:var(--ink)}
.res a:hover{border-color:var(--accent)}
.res b{font-family:var(--head);font-weight:600;line-height:1.25}
.res span.d{color:var(--muted);font-size:.9rem}
footer{max-width:1100px;margin:40px auto 0;padding-top:20px;border-top:1px solid var(--line);color:var(--muted);font-size:.88rem;display:flex;justify-content:space-between;flex-wrap:wrap;gap:12px}
@media (max-width:860px){
  .course{grid-template-columns:1fr}.rail{display:none}
  .grid2{grid-template-columns:1fr}
}
textarea,select{font:inherit;width:100%;padding:11px 12px;border-radius:10px;border:1px solid var(--line);background:var(--bg);color:var(--ink)}
textarea{min-height:120px;resize:vertical}
@media (prefers-reduced-motion:reduce){*{transition:none!important;animation:none!important}}
</style>
</head>
<body>
<a class="skip" href="#app">Skip to main content</a>
<header class="top"><div class="bar">
  <a class="brand" href="#home"><span class="mark" aria-hidden="true">Aa</span>SLLC Online Course</a>
  <nav id="nav" aria-label="Main"></nav>
  <button type="button" id="theme-toggle" class="theme-btn" aria-label="Toggle colour theme" title="Toggle colour theme">☾</button>
</div></header>
<main class="wrap" id="app" tabindex="-1"></main>
<footer class="wrap" id="foot">
  <span>© 2026 Imagine1Day International Organization — School-Based Literacy & Language Club</span>
  <a href="#admin">Instructor / Admin Portal</a>
</footer>

<script>
/* ============================================================
   SETTINGS — Course Owner Configuration
   ============================================================ */
const CFG = {
  org: "Imagine1Day International Organization",
  course: "School-Based Literacy and Language Club (SLLC)",
  sub: "Reading & Writing Club implementation course for Ethiopian primary schools (Grades 1–8)",
  ownerEmail: "mohammedscho2023@gmail.com",
  passModule: 3,
  examSize: 30, passPct: 70,
  practiceMin: 5,
  salt: "imagine1day-sllc-2026-x7Qm",

  requireApproval: true,
  approved: [],
  instructorHash: "3b7af1bb3e422b7d1c9fd21c9d5e10d8a21d1bdc30f9f4fc92d2902a6a773c3c"
};

/* ============================================================
   SHA-256 CRYPTOGRAPHIC HELPER
   ============================================================ */
function sha256(s){
  const K=[0x428a2f98,0x71374491,0xb5c0fbcf,0xe9b5dba5,0x3956c25b,0x59f111f1,0x923f82a4,0xab1c5ed5,0xd807aa98,0x12835b01,0x243185be,0x550c7dc3,0x72be5d74,0x80deb1fe,0x9bdc06a7,0xc19bf174,0xe49b69c1,0xefbe4786,0x0fc19dc6,0x240ca1cc,0x2de92c6f,0x4a7484aa,0x5cb0a9dc,0x76f988da,0x983e5152,0xa831c66d,0xb00327c8,0xbf597fc7,0xc6e00bf3,0xd5a79147,0x06ca6351,0x14292967,0x27b70a85,0x2e1b2138,0x4d2c6dfc,0x53380d13,0x650a7354,0x766a0abb,0x81c2c92e,0x92722c85,0xa2bfe8a1,0xa81a664b,0xc24b8b70,0xc76c51a3,0xd192e819,0xd6990624,0xf40e3585,0x106aa070,0x19a4c116,0x1e376c08,0x2748774c,0x34b0bcb5,0x391c0cb3,0x4ed8aa4a,0x5b9cca4f,0x682e6ff3,0x748f82ee,0x78a5636f,0x84c87814,0x8cc70208,0x90befffa,0xa4506ceb,0xbef9a3f7,0xc67178f2];
  const b = Array.from(new TextEncoder().encode(s));
  const l = b.length * 8;
  b.push(0x80);
  while (b.length % 64 !== 56) b.push(0);
  for (let i = 7; i >= 0; i--) b.push(i > 3 ? 0 : (l >>> (i * 8)) & 255);
  let h = [0x6a09e667,0xbb67ae85,0x3c6ef372,0xa54ff53a,0x510e527f,0x9b05688c,0x1f83d9ab,0x5be0cd19];
  const R = (x, n) => (x >>> n) | (x << (32 - n));
  for (let o = 0; o < b.length; o += 64) {
    const w = new Array(64);
    for (let i = 0; i < 16; i++) w[i] = (b[o + 4*i] << 24) | (b[o + 4*i + 1] << 16) | (b[o + 4*i + 2] << 8) | b[o + 4*i + 3];
    for (let i = 16; i < 64; i++) {
      const s0 = R(w[i-15],7) ^ R(w[i-15],18) ^ (w[i-15] >>> 3);
      const s1 = R(w[i-2],17) ^ R(w[i-2],19) ^ (w[i-2] >>> 10);
      w[i] = (w[i-16] + s0 + w[i-7] + s1) | 0;
    }
    let [a,c,d,e,f,g,hh,j] = h;
    for (let i = 0; i < 64; i++) {
      const S1 = R(f,6) ^ R(f,11) ^ R(f,25), ch = (f & g) ^ (~f & hh), t1 = (j + S1 + ch + K[i] + w[i]) | 0;
      const S0 = R(a,2) ^ R(a,13) ^ R(a,22), mj = (a & c) ^ (a & d) ^ (c & d), t2 = (S0 + mj) | 0;
      j = hh; hh = g; g = f; f = (e + t1) | 0; e = d; d = c; c = a; a = (t1 + t2) | 0;
    }
    h = [h[0]+a,h[1]+c,h[2]+d,h[3]+e,h[4]+f,h[5]+g,h[6]+hh,h[7]+j].map(x => x | 0);
  }
  return h.map(x => (x >>> 0).toString(16).padStart(8,'0')).join('');
}

function getLearnerHash(email) {
  return sha256(email.trim().toLowerCase() + ":" + CFG.salt);
}

function isUserApproved(user) {
  if (!CFG.requireApproval) return true;
  if (!user || !user.email) return false;
  const h = getLearnerHash(user.email);
  return CFG.approved.includes(h) || user.approvalToken === h;
}

function isModuleUnlocked(id) {
  if (id === 1) return true;
  // Module N is unlocked only if Module N-1 quiz score >= CFG.passModule
  return (state.progress[id - 1] || 0) >= CFG.passModule;
}

/* ============================================================
   COURSE CONTENT
   ============================================================ */
const MODULES = [
{ id:1, title:"Understanding School-Based Literacy Improvement", mins:35,
  intro:"School-based literacy improvement is a planned, continuous effort led by the school itself (directors, teachers, volunteers, parents and students) so that all children learn to read and write well, especially in the early grades and in their mother tongue.",
  sections:[
   {h:"The core idea", l:["The school identifies its own literacy challenges, for example many Grade 2 students cannot read simple words.","It sets clear goals, for example 80% of Grade 2 students reading at least 40 words correct per minute by June.","It plans and carries out actions: TaRL, better teaching, extra practice time, reading clubs, reading corners, volunteer support and parent engagement.","It checks progress regularly and adjusts the plan using evidence such as simple assessments, observation and student work."]},
   {h:"Seven key components", l:["Strong classroom instruction in reading and writing","Extra practice time through clubs and activities","Access to supplementary reading materials","Support for struggling learners","Inclusion, gender equity and language considerations","Parent and community engagement","Monitoring, review and continuous improvement"]},
   {h:"Five types of school-based literacy activity", table:{head:["Type","Examples"],rows:[["Classroom reading and writing lessons","Letter/Fidel sounds, blending, guided reading, TaRL classrooms"],["Co-curricular literacy clubs","Reading and Writing Club, 1–2 times a week, about 90 minutes"],["Reading corners and spaces","Classroom shelves, reading room, community book banks"],["Volunteer, peer and family support","Reading buddies, parents listening to children read"],["School-wide events","Fluency competitions, storytelling contests, literacy weeks"]]}},
   {h:"The five key reading skills", table:{head:["Skill","What it means","Example"],rows:[["Phonemic awareness","Hearing and manipulating individual sounds in spoken words (oral, no letters)","Segmenting fish into /f/ /i/ /sh/"],["Phonics","Linking letters (graphemes) to sounds (phonemes)","Letters sh make one sound in ship"],["Fluency","Reading accurately, smoothly and with expression","Choral, paired and repeated reading"],["Vocabulary","Words a learner knows and uses","Teaching harvest with a sentence and discussion"],["Comprehension","Understanding, interpreting and thinking about text","Why did Sara carry an umbrella?"]]}},
   {h:"Eight principles of effective literacy development", l:["Start with the mother tongue","Teach the five key reading skills explicitly","Integrate reading, writing, speaking and listening","Provide lots of practice with appropriate texts: decodable, levelled, culturally relevant, narrative and informational","Differentiate support for struggling learners","Ensure inclusion and gender equity","Create a print-rich, supportive environment","Monitor progress and use data to improve"]}
  ],
  quiz:[
   {q:"What makes literacy improvement “school-based”?",o:["Decisions come only from the regional education bureau","Decisions are made at school level, led by teachers and school leaders with support from supervisors, PTSA and communities","Only textbooks supplied by the woreda are used","Only volunteers from outside the school lead it"],a:1,why:"The approach is school-based because decisions are made at school level and rooted in the school's daily reality."},
   {q:"Which skill is an oral language skill that does not involve printed letters?",o:["Phonics","Fluency","Phonemic awareness","Writing"],a:2,why:"Phonemic awareness is hearing, identifying and manipulating sounds in spoken words."},
   {q:"Why should instruction begin in the mother tongue?",o:["Children learn to read and write best in a language they understand, and this supports later learning of other languages","It is cheaper for schools","English should never be taught","It removes the need for assessment"],a:0,why:"Strong mother-tongue literacy supports later learning of additional languages such as English."},
   {q:"Texts for practice should be…",o:["Only very long and difficult","Decodable, levelled, interesting and culturally relevant","Only informational","Only chosen by volunteers without checking level"],a:1,why:"Texts should match sounds taught, match reading ability, interest children and include both narrative and informational types."}
  ]},
{ id:2, title:"The School-Based Literacy and Language Club (SLLC)", mins:30,
  intro:"The SLLC is a student-centred extracurricular platform within a school that improves literacy, language, communication and reading skills through organised and enjoyable activities beyond regular lessons.",
  sections:[
   {h:"Purpose", l:["Improve reading, writing, speaking and listening","Build a culture of reading and lifelong learning","Strengthen the language of instruction and other languages taught","Develop communication, collaboration, leadership and critical thinking","Support struggling readers and writers with inclusive participation","Offer storytelling, debates, public speaking, reading circles, drama, poetry and creative writing"]},
   {h:"Why one integrated club?", l:["Literacy skills are interconnected: reading, writing, speaking and listening reinforce each other.","Efficient use of limited resources, facilitators and meeting time.","Inclusive participation: varied activities appeal to different strengths.","Stronger learning, communication, reading culture, academic achievement and leadership skills.","Less duplication and administrative workload, and a sustainable framework."]},
   {h:"General objective", p:"To enhance students' literacy and language competencies through participatory, enjoyable and inclusive activities that promote reading, writing, speaking, listening and critical thinking."},
   {h:"Eleven guiding principles", l:["Learner-centred participation","Inclusiveness and equity","Voluntary and enjoyable learning","Holistic literacy development","Respect for diversity","Collaboration and teamwork","Creativity and innovation","Leadership and responsibility","Continuous learning and improvement","Community and stakeholder engagement","Child protection and a safe learning environment"]}
  ],
  quiz:[
   {q:"What is the main advantage of one integrated literacy club over separate clubs?",o:["It needs no facilitators","It combines reading, writing, speaking and listening under one coordinated platform, saving resources and reducing duplication","It only serves the best readers","It replaces classroom lessons"],a:1,why:"Integration recognises that literacy skills are interconnected and maximises limited resources."},
   {q:"Which principle says participation should be based on students' interest?",o:["Voluntary and enjoyable learning","Continuous improvement","Holistic development","Community engagement"],a:0,why:"Participation should come from interest and enthusiasm, with interactive, enjoyable activities."},
   {q:"Who are the primary actors in planning, implementing and evaluating club activities?",o:["Only teachers","Only the school director","Students","Only parents"],a:2,why:"Learner-centred participation makes students the primary actors."},
   {q:"The SLLC should give equal opportunities regardless of…",o:["Only gender","Gender, language background, disability, socioeconomic status or academic performance","Only academic performance","Nothing; places are limited to top learners"],a:1,why:"Inclusiveness and equity cover all these dimensions, with special attention to marginalised and struggling learners."}
  ]},
{ id:3, title:"Club Leadership and Management", mins:35,
  intro:"A clear committee structure, defined roles, annual and weekly plans and regular review meetings keep the club accountable and running smoothly.",
  sections:[
   {h:"Committee roles", table:{head:["Position","Key responsibilities"],rows:[["Chairperson / President","Overall leadership, chairs meetings, represents the club, ensures plans are implemented"],["Vice Chairperson","Supports the Chairperson, acts when the Chairperson is absent, monitors progress"],["Secretary","Agendas, minutes, records, correspondence and membership register"],["Treasurer","Financial records, budgets and reports, transparency"],["Program / Activity Coordinator","Activity schedules, event plans, monitors and reports outcomes"],["Membership Coordinator","Recruits and orients members, keeps records, promotes retention"],["Communications Officer","Shares information, publicises activities and achievements"]]}},
   {h:"Best practices for committees", l:["Define terms of office and election procedures","Hold regular committee meetings and document decisions and actions","Ensure transparency in financial and operational matters","Promote gender balance, inclusion and active member participation"]},
   {h:"Annual planning steps", l:["Review the previous year's performance","Identify priorities, opportunities and challenges","Set annual goals and objectives","Develop activities and timelines","Assign responsibilities","Prepare a budget and resource plan","Obtain committee approval","Communicate the plan to members"]},
   {h:"Weekly timetable and review meetings", l:["Weekly timetable: identify the week's activities, allocate dates, times and venues, assign people, confirm resources, share with members.","Review meetings come in four types: weekly, monthly, quarterly and annual review and planning.","Standard agenda: welcome, previous minutes and actions, progress updates, challenges, financial update, decisions and actions, planning ahead, closing.","Outputs: minutes, updated action plan, progress reports, recommendations and agreed next steps."]}
  ],
  quiz:[
   {q:"Who records and distributes meeting minutes and keeps the membership register?",o:["Treasurer","Secretary","Communications Officer","Vice Chairperson"],a:1,why:"The Secretary prepares agendas, records minutes and maintains records and the membership register."},
   {q:"Which is the FIRST step in annual planning?",o:["Prepare the budget","Review the previous year's performance","Assign responsibilities","Obtain committee approval"],a:1,why:"Planning begins by reviewing last year's performance."},
   {q:"Which is NOT one of the four types of review meeting?",o:["Weekly","Monthly","Quarterly","Daily"],a:3,why:"The manual lists weekly, monthly, quarterly and annual review meetings."},
   {q:"Who manages budgets and financial reports?",o:["Treasurer","Membership Coordinator","Program Coordinator","Chairperson only"],a:0,why:"The Treasurer maintains financial records and prepares budgets and reports."}
  ]},
{ id:4, title:"Student Participation and Inclusion", mins:35,
  intro:"All learners should have equal opportunities to benefit. Clubs identify and support vulnerable students, promote gender equity, include children with disabilities and create safe, accessible spaces.",
  sections:[
   {h:"Students who may need additional support", l:["Students with disabilities or learning difficulties","Girls facing social or cultural barriers","Children from economically disadvantaged households","Orphans and vulnerable children","Students with frequent absenteeism","Students with emotional or psychosocial challenges or language and communication difficulties"]},
   {h:"Identifying and supporting", l:["Identify through classroom observation, attendance monitoring, talks with students and parents, teacher referrals, peer feedback and community assessments.","Support through mentoring, tutoring, referral to specialised services, learning materials, psychosocial activities and regular follow-up.","Maintain confidentiality and dignity, avoid labelling or stigma, and involve parents and caregivers."]},
   {h:"Gender equity", l:["Encourage girls and boys to participate equally and balance club committees.","Use inclusive language, remove participation barriers and give leadership opportunities to all.","Indicators: balanced membership, equal participation, fair leadership distribution, reduced absenteeism and dropout."]},
   {h:"Disability inclusion and safe environments", l:["Adapt activities, use accessible communication, arrange seating and spaces, encourage peer support and give extra time when needed.","Focus on abilities rather than limitations and consult students and caregivers.","Safe environment: respectful relationships, clear rules, protection from bullying and discrimination.","Accessible environment: safe physical access, adequate lighting and seating, clear instructions and flexible participation."]},
   {h:"Safety and accessibility checklist", table:{head:["Area","Checklist item"],rows:[["Physical environment","Learning space is clean and safe"],["Accessibility","Students can enter and move around comfortably"],["Participation","All students have opportunities to contribute"],["Communication","Information is clear and understandable"],["Protection","Procedures exist for reporting concerns"],["Inclusion","Activities are adapted for different needs"]]}}
  ],
  quiz:[
   {q:"Which is a best practice when supporting vulnerable students?",o:["Announce their needs to the whole group","Maintain confidentiality and dignity and avoid labelling","Exclude them from leadership","Move them to separate clubs"],a:1,why:"Confidentiality, dignity and avoiding stigma are core practices."},
   {q:"Which is an indicator of gender equity?",o:["Only boys hold leadership roles","Balanced club membership by gender and fair distribution of leadership","Girls attend on separate days","No attendance records are kept"],a:1,why:"Balanced membership, equal participation and fair leadership are indicators."},
   {q:"Inclusion of children with disabilities means…",o:["They watch from the side","They participate fully, actively and meaningfully, with barriers removed","They only join once a year","Parents lead their sessions"],a:1,why:"Inclusion is full, active and meaningful participation."},
   {q:"Which method helps identify students needing support?",o:["Attendance monitoring and teacher referrals","Guessing from appearance","Ranking by family income publicly","Waiting for complaints"],a:0,why:"Observation, attendance monitoring, referrals and talks with parents are the best ways to identify students needing additional support."}
  ]}
];

/* ============================================================
   APP STATE & ROUTING
   ============================================================ */
let state = {
  user: JSON.parse(localStorage.getItem('sllc-user') || 'null'),
  progress: JSON.parse(localStorage.getItem('sllc-progress') || '{}'),
  practice: JSON.parse(localStorage.getItem('sllc-practice') || '{}'),
  examPassed: localStorage.getItem('sllc-exam-passed') === 'true',
  adminUnlocked: sessionStorage.getItem('sllc-admin') === 'true'
};

function saveState() {
  localStorage.setItem('sllc-progress', JSON.stringify(state.progress));
  localStorage.setItem('sllc-practice', JSON.stringify(state.practice));
  localStorage.setItem('sllc-exam-passed', state.examPassed ? 'true' : 'false');
  if (state.user) localStorage.setItem('sllc-user', JSON.stringify(state.user));
}

function checkMagicApproval() {
  const hash = location.hash;
  if (hash.startsWith('#approve?')) {
    const params = new URLSearchParams(hash.split('?')[1]);
    const email = params.get('email') || '';
    const token = params.get('token') || '';
    const name = params.get('name') || '';
    const school = params.get('school') || '';
    const expected = getLearnerHash(email);

    if (email && token === expected) {
      state.user = {
        name: name || (state.user && state.user.name) || email.split('@')[0],
        email: email.trim().toLowerCase(),
        school: school || (state.user && state.user.school) || 'Approved School',
        approvalToken: token
      };
      saveState();
      location.hash = '#home';
      setTimeout(() => alert(`Account approved for ${state.user.email}! You now have full access to the SLLC Course.`), 100);
    } else {
      location.hash = '#home';
      setTimeout(() => alert('Invalid or expired approval link. Please contact the course administrator.'), 100);
    }
  }
}

function renderNav() {
  const nav = document.getElementById('nav');
  const hash = location.hash || '#home';
  const links = [
    {h:'#home', label:'Home'},
    {h:'#modules', label:'Modules'},
    {h:'#practice', label:'Practice'},
    {h:'#exam', label:'Final Exam'},
    {h:'#certificate', label:'Certificate'},
    {h:'#resources', label:'Resources'}
  ];
  nav.innerHTML = links.map(l => `<a href="${l.h}" ${hash === l.h ? 'aria-current="page"' : ''}>${l.label}</a>`).join('');
}

function router() {
  checkMagicApproval();
  renderNav();
  const hash = location.hash || '#home';
  const app = document.getElementById('app');
  app.innerHTML = '';

  if (hash === '#home') renderHome(app);
  else if (hash === '#modules') renderModulesList(app);
  else if (hash.startsWith('#module/')) renderModule(app, parseInt(hash.split('/')[1]));
  else if (hash === '#practice') renderPractice(app);
  else if (hash === '#exam') renderExam(app);
  else if (hash === '#certificate') renderCertificate(app);
  else if (hash === '#resources') renderResources(app);
  else if (hash === '#admin') renderAdmin(app);
  else renderHome(app);
  window.scrollTo(0, 0);
}

window.addEventListener('hashchange', router);
window.addEventListener('DOMContentLoaded', () => {
  document.getElementById('theme-toggle').onclick = () => {
    const cur = document.documentElement.dataset.theme === 'dark' ? 'light' : 'dark';
    document.documentElement.dataset.theme = cur;
    localStorage.setItem('sllc-theme', cur);
    document.getElementById('theme-toggle').textContent = cur === 'dark' ? '☀' : '☾';
  };
  const cur = localStorage.getItem('sllc-theme') || (window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light');
  document.getElementById('theme-toggle').textContent = cur === 'dark' ? '☀' : '☾';
  router();
});

/* ============================================================
   ACCESS GUARD COMPONENT
   ============================================================ */
function guardAccess(el) {
  if (!state.user) {
    el.innerHTML = `
      <div class="card stack" style="margin-top:24px; text-align:center; padding:40px;">
        <h2>Registration Required</h2>
        <p class="hint">Please register with your email address on the Home page to access course modules and certification.</p>
        <div class="row" style="justify-content:center; margin-top:12px;">
          <a class="btn primary" href="#home">Go to Registration</a>
        </div>
      </div>`;
    return false;
  }
  if (!isUserApproved(state.user)) {
    const mailHref = buildRegistrationMailto(state.user);
    el.innerHTML = `
      <div class="card stack" style="margin-top:24px; padding:32px;">
        <span class="pill warn" style="justify-self:start">Pending Admin Approval</span>
        <h2>Your Registration is Awaiting Approval</h2>
        <p>Thank you, <b>${escapeHtml(state.user.name)}</b> (${escapeHtml(state.user.email)}). To unlock the modules, please email your registration request to the course coordinator and click the approval link sent back to you.</p>
        <div class="row" style="margin-top:8px;">
          <a class="btn primary" href="${mailHref}">✉ Send Registration Request via Email</a>
          <button class="btn" onclick="enterApprovalCode()">I Have an Approval Code</button>
        </div>
      </div>`;
    return false;
  }
  return true;
}

function buildRegistrationMailto(u) {
  const hash = getLearnerHash(u.email);
  const subject = encodeURIComponent(`SLLC Course Registration Request — ${u.name}`);
  const body = encodeURIComponent(
`Hello Imagine1Day SLLC Coordinator,

I would like to register for the School-Based Literacy and Language Club (SLLC) Online Course.

Full Name: ${u.name}
Email Address: ${u.email}
School / Woreda: ${u.school}
Verification Hash: ${hash}

Please review and send my approval link.

Thank you.`
  );
  return `mailto:${CFG.ownerEmail}?subject=${subject}&body=${body}`;
}

function enterApprovalCode() {
  const code = prompt('Paste the approval code or token sent to your email:');
  if (!code) return;
  const expected = getLearnerHash(state.user.email);
  if (code.trim() === expected) {
    state.user.approvalToken = expected;
    saveState();
    alert('Account approved! Welcome to the SLLC Course.');
    router();
  } else {
    alert('Invalid approval code for ' + state.user.email + '. Please check the code sent by the administrator.');
  }
}

/* ============================================================
   VIEWS
   ============================================================ */
function renderHome(el) {
  const approved = isUserApproved(state.user);
  el.innerHTML = `
    <div class="hero">
      <span class="pill">${CFG.org}</span>
      <h1>${CFG.course}</h1>
      <p class="lead">${CFG.sub}</p>
      <div class="row">
        <a class="btn primary" href="#modules">Start Course Modules</a>
        <a class="btn" href="#practice">Practical Tasks</a>
      </div>
    </div>
    <div class="grid2" style="margin-top:24px">
      <div class="card stack">
        <h3>Enrollment & Sequential Progression</h3>
        <ul style="padding-left:1.2rem; display:grid; gap:8px;">
          <li><b>1. Register by Email:</b> Submit your Name, Email, and School/Woreda.</li>
          <li><b>2. Email Approval:</b> Send your pre-filled registration email to the coordinator and open your approval link.</li>
          <li><b>3. Sequential Modules:</b> Complete and pass each module quiz (3+ correct answers) to unlock the next module in order.</li>
          <li><b>4. Final Exam & Certificate:</b> Pass the final exam to download your official certificate.</li>
        </ul>
      </div>
      <div class="card stack">
        <h3>Learner Registration & Status</h3>
        ${state.user ? `
          <div class="row" style="justify-content:space-between">
            <span class="pill ${approved ? 'ok' : 'warn'}">${approved ? '✓ Approved Learner' : '⏳ Pending Approval'}</span>
            <button class="btn" style="min-height:36px; padding:4px 12px;" onclick="logoutUser()">Change Account</button>
          </div>
          <p><b>Name:</b> ${escapeHtml(state.user.name)}</p>
          <p><b>Email:</b> ${escapeHtml(state.user.email)}</p>
          <p><b>School / Woreda:</b> ${escapeHtml(state.user.school)}</p>
          ${!approved ? `
            <div class="msg info">
              Step 2: Click below to send your registration email to <b>${CFG.ownerEmail}</b> so the administrator can send back your approval link.
            </div>
            <div class="row">
              <a class="btn primary" href="${buildRegistrationMailto(state.user)}">✉ Email Registration to Admin</a>
              <button class="btn" onclick="enterApprovalCode()">Enter Approval Code</button>
            </div>
          ` : `
            <div class="msg good">Your account is active and verified. You can access all unlocked modules and your certificate.</div>
          `}
        ` : `
          <p class="hint">Register your details below to request course access via email.</p>
          <div class="field">
            <label for="reg-name">Full Name</label>
            <input type="text" id="reg-name" placeholder="e.g., Abebe Kebede">
          </div>
          <div class="field">
            <label for="reg-email">Email Address</label>
            <input type="email" id="reg-email" placeholder="e.g., abebe@example.com">
          </div>
          <div class="field">
            <label for="reg-school">School Name & Woreda</label>
            <input type="text" id="reg-school" placeholder="e.g., Babile Primary School, East Hararghe">
          </div>
          <button class="btn primary" onclick="registerUser()">Register & Prepare Approval Email</button>
        `}
      </div>
    </div>
  `;
}

function registerUser() {
  const name = document.getElementById('reg-name').value.trim();
  const email = document.getElementById('reg-email').value.trim().toLowerCase();
  const school = document.getElementById('reg-school').value.trim();
  if (!name || !email || !email.includes('@') || !school) {
    alert('Please enter your full name, a valid email address, and your school/woreda.');
    return;
  }
  state.user = { name, email, school };
  saveState();
  router();
}

function logoutUser() {
  if (confirm('Sign out and clear your profile from this browser?')) {
    state.user = null;
    localStorage.removeItem('sllc-user');
    router();
  }
}

function renderModulesList(el) {
  if (!guardAccess(el)) return;
  el.innerHTML = `
    <div class="stack" style="padding:24px 0">
      <h2>Course Modules</h2>
      <p class="hint">Modules must be completed sequentially. Pass each module quiz to unlock the next one.</p>
      <div class="stack" style="gap:12px; margin-top:12px;">
        ${MODULES.map(m => {
          const unlocked = isModuleUnlocked(m.id);
          const passed = state.progress[m.id] >= CFG.passModule;
          return `
            <div class="card row" style="justify-content:space-between; ${!unlocked ? 'opacity:0.6;' : ''}">
              <div>
                <span class="pill ${passed ? 'ok' : (unlocked ? 'warn' : '')}">${passed ? '✓ Completed' : (unlocked ? 'Unlocked' : '🔒 Locked')}</span>
                <h3 style="margin-top:6px;">
                  ${unlocked ? `<a href="#module/${m.id}">${m.title}</a>` : m.title}
                </h3>
                <span class="hint">Estimated time: ${m.mins} minutes ${!unlocked ? ' • Complete previous module quiz to unlock' : ''}</span>
              </div>
              ${unlocked ? `<a class="btn primary" href="#module/${m.id}">Open Module</a>` : `<button class="btn" disabled>Locked</button>`}
            </div>
          `;
        }).join('')}
      </div>
    </div>
  `;
}

function renderModule(el, id) {
  if (!guardAccess(el)) return;
  if (!isModuleUnlocked(id)) {
    alert('You must complete and pass the previous module quiz before accessing this module.');
    location.hash = '#modules';
    return;
  }
  const m = MODULES.find(x => x.id === id);
  if (!m) { location.hash = '#modules'; return; }

  el.innerHTML = `
    <div class="course">
      <aside class="rail">
        <a href="#modules" class="btn" style="margin-bottom:12px">← Back to Modules</a>
        <h3>Modules</h3>
        ${MODULES.map(mod => {
          const unlocked = isModuleUnlocked(mod.id);
          const passed = (state.progress[mod.id] || 0) >= CFG.passModule;
          return `
            <button ${unlocked ? `onclick="location.hash='#module/${mod.id}'"` : 'disabled'} ${mod.id === id ? 'aria-current="true"' : ''}>
              <span class="n">${passed ? '✓' : mod.id}</span>
              <span>${mod.title} ${!unlocked ? '🔒' : ''}</span>
            </button>
          `;
        }).join('')}
      </aside>
      <div class="lesson stack">
        <div>
          <span class="pill">Module ${m.id} of ${MODULES.length}</span>
          <h2>${m.title}</h2>
          <p class="hint">Approx. ${m.mins} minutes reading</p>
        </div>
        <div class="card stack">
          <p><b>Introduction:</b> ${m.intro}</p>
        </div>
        ${m.sections.map(s => `
          <div class="card stack">
            <h3>${s.h}</h3>
            ${s.p ? `<p>${s.p}</p>` : ''}
            ${s.l ? `<ul>${s.l.map(li => `<li>${li}</li>`).join('')}</ul>` : ''}
            ${s.table ? `
              <div class="tablewrap">
                <table>
                  <thead><tr>${s.table.head.map(th => `<th>${th}</th>`).join('')}</tr></thead>
                  <tbody>${s.table.rows.map(r => `<tr>${r.map(td => `<td>${td}</td>`).join('')}</tr>`).join('')}</tbody>
                </table>
              </div>
            ` : ''}
          </div>
        `).join('')}

        <div class="card stack">
          <h3>Module Knowledge Check</h3>
          <p class="hint">Answer at least ${CFG.passModule} of ${m.quiz.length} correctly to complete this module and unlock the next one.</p>
          <div class="stack" id="quiz-container">
            ${m.quiz.map((q, qi) => `
              <fieldset class="q" data-qi="${qi}" data-ans="${q.a}">
                <legend>Question ${qi+1}: ${q.q}</legend>
                ${q.o.map((opt, oi) => `
                  <label class="opt">
                    <input type="radio" name="q${qi}" value="${oi}">
                    <span>${opt}</span>
                  </label>
                `).join('')}
                <div class="why" style="display:none"></div>
              </fieldset>
            `).join('')}
            <button class="btn primary" onclick="submitQuiz(${m.id})">Check Answers</button>
            <div id="quiz-result"></div>
          </div>
        </div>
      </div>
    </div>
  `;
}

function submitQuiz(modId) {
  const m = MODULES.find(x => x.id === modId);
  let score = 0;
  m.quiz.forEach((q, qi) => {
    const fs = document.querySelector(`fieldset[data-qi="${qi}"]`);
    const selected = fs.querySelector('input:checked');
    const whyEl = fs.querySelector('.why');
    fs.querySelectorAll('.opt').forEach(o => o.classList.remove('right', 'wrong'));

    if (selected) {
      const val = parseInt(selected.value);
      if (val === q.a) {
        score++;
        selected.closest('.opt').classList.add('right');
      } else {
        selected.closest('.opt').classList.add('wrong');
        fs.querySelectorAll('.opt')[q.a].classList.add('right');
      }
    } else {
      fs.querySelectorAll('.opt')[q.a].classList.add('right');
    }
    whyEl.style.display = 'block';
    whyEl.innerHTML = `<b>Explanation:</b> ${q.why}`;
  });

  state.progress[modId] = score;
  saveState();

  const resEl = document.getElementById('quiz-result');
  if (score >= CFG.passModule) {
    const nextMod = modId + 1;
    const hasNext = nextMod <= MODULES.length;
    resEl.innerHTML = `
      <div class="msg good" style="margin-top:12px;">
        Great job! You scored ${score}/${m.quiz.length}. Module completed successfully! ${hasNext ? 'Next module is now unlocked.' : 'You have completed all modules!'}
      </div>
      ${hasNext ? `<p style="margin-top:12px;"><a class="btn primary" href="#module/${nextMod}">Proceed to Module ${nextMod} →</a></p>` : ''}
    `;
  } else {
    resEl.innerHTML = `<div class="msg bad" style="margin-top:12px;">You scored ${score}/${m.quiz.length}. You need at least ${CFG.passModule} correct answers to pass and unlock the next module. Review the material and try again.</div>`;
  }
}

function renderPractice(el) {
  if (!guardAccess(el)) return;
  el.innerHTML = `
    <div class="stack" style="padding:24px 0">
      <h2>Practical Implementation Tasks</h2>
      <p class="hint">Document your school's SLLC activities. Complete all ${CFG.practiceMin} tasks.</p>
      <div class="stack" style="margin-top:16px;">
        ${[
          {id:1, t:"Establish the School Literacy Club committee and record members."},
          {id:2, t:"Draft the annual club calendar and weekly activity timetable."},
          {id:3, t:"Organise a book inventory and set up a classroom reading corner."},
          {id:4, t:"Conduct an inclusive reading session supporting struggling learners."},
          {id:5, t:"Organise a parent-teacher reading engagement or storytelling event."}
        ].map(p => `
          <div class="card stack">
            <h3>Task ${p.id}: ${p.t}</h3>
            <div class="field">
              <label>Implementation notes / report</label>
              <textarea id="prac-${p.id}" placeholder="Describe how this was implemented at your school...">${escapeHtml(state.practice[p.id] || '')}</textarea>
            </div>
            <button class="btn primary" onclick="savePractice(${p.id})">Save Task Report</button>
          </div>
        `).join('')}
      </div>
    </div>
  `;
}

function savePractice(id) {
  const val = document.getElementById(`prac-${id}`).value.trim();
  if (!val) { alert('Please enter report notes before saving.'); return; }
  state.practice[id] = val;
  saveState();
  alert('Task saved successfully!');
}

function renderExam(el) {
  if (!guardAccess(el)) return;
  // Ensure all modules are passed before unlocking exam
  const allModulesPassed = MODULES.every(m => (state.progress[m.id] || 0) >= CFG.passModule);
  if (!allModulesPassed) {
    el.innerHTML = `
      <div class="card stack" style="margin-top:24px; text-align:center; padding:40px;">
        <h2>Modules Incomplete</h2>
        <p class="hint">You must successfully complete and pass all 4 module quizzes before taking the Final Exam.</p>
        <div class="row" style="justify-content:center; margin-top:12px;">
          <a class="btn primary" href="#modules">Go to Course Modules</a>
        </div>
      </div>`;
    return;
  }

  el.innerHTML = `
    <div class="stack" style="padding:24px 0">
      <h2>Final Certification Exam</h2>
      <p class="hint">Comprehensive review covering all course modules.</p>
      <div class="card stack">
        <p>You have completed all modules! Ready to test your knowledge?</p>
        <button class="btn primary" onclick="startExam()">Start Exam Now</button>
        <div id="exam-area"></div>
      </div>
    </div>
  `;
}

function startExam() {
  const allQ = [];
  MODULES.forEach(m => m.quiz.forEach(q => allQ.push(q)));
  const area = document.getElementById('exam-area');
  area.innerHTML = `
    <div class="stack" style="margin-top:16px;">
      ${allQ.map((q, qi) => `
        <fieldset class="q" data-eqi="${qi}" data-eans="${q.a}">
          <legend>Question ${qi+1}: ${q.q}</legend>
          ${q.o.map((opt, oi) => `
            <label class="opt">
              <input type="radio" name="eq${qi}" value="${oi}">
              <span>${opt}</span>
            </label>
          `).join('')}
        </fieldset>
      `).join('')}
      <button class="btn primary" onclick="submitExam(${allQ.length})">Submit Final Exam</button>
      <div id="exam-res"></div>
    </div>
  `;
}

function submitExam(total) {
  let score = 0;
  for (let i = 0; i < total; i++) {
    const fs = document.querySelector(`fieldset[data-eqi="${i}"]`);
    const selected = fs.querySelector('input:checked');
    const correct = parseInt(fs.dataset.eans);
    if (selected && parseInt(selected.value) === correct) score++;
  }
  const pct = Math.round((score / total) * 100);
  const passed = pct >= CFG.passPct;
  state.examPassed = passed;
  saveState();

  const res = document.getElementById('exam-res');
  res.innerHTML = `
    <div class="msg ${passed ? 'good' : 'bad'}" style="margin-top:12px;">
      You scored ${score}/${total} (${pct}%). ${passed ? 'Congratulations, you passed the exam!' : 'You did not reach the 70% passing threshold. Please review the modules and try again.'}
    </div>
    ${passed ? '<p style="margin-top:12px;"><a class="btn primary" href="#certificate">View Your Certificate</a></p>' : ''}
  `;
}

function renderCertificate(el) {
  if (!guardAccess(el)) return;
  if (!state.examPassed) {
    el.innerHTML = `
      <div class="card stack" style="margin-top:24px; text-align:center; padding:40px;">
        <h2>Final Exam Not Yet Passed</h2>
        <p class="hint">Please complete all modules and pass the Final Exam (70% or higher) to unlock your certificate.</p>
        <div class="row" style="justify-content:center; margin-top:12px;">
          <a class="btn primary" href="#exam">Go to Final Exam</a>
        </div>
      </div>`;
    return;
  }
  const certId = getLearnerHash(state.user.email).slice(0, 12).toUpperCase();
  el.innerHTML = `
    <div class="stack" style="padding:24px 0">
      <h2>Certificate of Completion</h2>
      <div class="cert card stack" style="text-align:center; padding:40px;">
        <span class="pill">${CFG.org}</span>
        <h1 style="margin-top:10px;">Certificate of Achievement</h1>
        <p>This is to certify that</p>
        <h2 style="color:var(--accent); font-size:2rem; margin:10px 0;">${escapeHtml(state.user.name)}</h2>
        <p>from <b>${escapeHtml(state.user.school)}</b> (${escapeHtml(state.user.email)}) has successfully completed the</p>
        <h3>${CFG.course}</h3>
        <p class="hint" style="margin-top:20px;">Verification ID: ${certId} • Issued by Imagine1Day International Organization</p>
        <div class="row" style="justify-content:center; margin-top:20px;">
          <button class="btn primary" onclick="window.print()">Print / Save PDF</button>
        </div>
      </div>
    </div>
  `;
}

function renderResources(el) {
  el.innerHTML = `
    <div class="stack" style="padding:24px 0">
      <h2>Implementation Resources</h2>
      <p class="hint">Downloadable templates, guides, and reporting tools.</p>
      <ul class="res">
        <li><a href="#" onclick="alert('Sample implementation guide downloaded.');return false;"><b>SLLC Implementation Guide</b><span class="d">PDF Document</span></a></li>
        <li><a href="#" onclick="alert('Club activity template downloaded.');return false;"><b>Weekly Activity Tracker</b><span class="d">Excel Spreadsheet</span></a></li>
        <li><a href="#" onclick="alert('Monitoring checklist downloaded.');return false;"><b>School Monitoring Checklist</b><span class="d">PDF Document</span></a></li>
      </ul>
    </div>
  `;
}

/* ============================================================
   ADMIN APPROVAL PORTAL (#admin)
   ============================================================ */
function renderAdmin(el) {
  if (!state.adminUnlocked) {
    el.innerHTML = `
      <div class="card stack" style="max-width:480px; margin:40px auto;">
        <span class="pill">Instructor & Coordinator Access</span>
        <h2>Admin Approval Portal</h2>
        <p class="hint">Enter your administrator password to approve learner registrations and issue email approval links.</p>
        <div class="field">
          <label for="admin-pass">Admin Password</label>
          <input type="password" id="admin-pass" placeholder="Enter password">
        </div>
        <button class="btn primary" onclick="unlockAdmin()">Sign In to Admin</button>
      </div>
    `;
    return;
  }

  el.innerHTML = `
    <div class="stack" style="padding:24px 0">
      <div class="row" style="justify-content:space-between">
        <div>
          <span class="pill ok">Admin Authenticated</span>
          <h2>Learner Registration & Email Approval Generator</h2>
        </div>
        <button class="btn" onclick="sessionStorage.removeItem('sllc-admin'); state.adminUnlocked=false; router();">Lock Admin</button>
      </div>

      <div class="card stack">
        <h3>Approve a Learner & Send Email Link</h3>
        <p class="hint">Enter the details from the learner's registration email to generate their signed approval link and send it back via email.</p>
        <div class="grid2">
          <div class="field">
            <label for="adm-name">Learner Full Name</label>
            <input type="text" id="adm-name" placeholder="e.g., Abebe Kebede">
          </div>
          <div class="field">
            <label for="adm-email">Learner Email Address</label>
            <input type="email" id="adm-email" placeholder="e.g., abebe@example.com">
          </div>
        </div>
        <div class="field">
          <label for="adm-school">Learner School / Woreda</label>
          <input type="text" id="adm-school" placeholder="e.g., Babile Primary School">
        </div>
        <button class="btn primary" onclick="generateApprovalOutput()">Generate Approval Link & Email</button>

        <div id="adm-output" class="stack" style="display:none; margin-top:12px;">
          <div class="field">
            <label>1. One-Click Email Reply to Learner</label>
            <div><a id="adm-mailto" class="btn sun" href="#">✉ Send Approval Email to Learner</a></div>
          </div>
          <div class="field">
            <label>2. Direct Approval Magic Link (Copy & Share)</label>
            <div class="copybox" id="adm-link"></div>
          </div>
          <div class="field">
            <label>3. Allowlist Hash (Optional permanent entry for CFG.approved in index.html)</label>
            <div class="copybox" id="adm-hash"></div>
          </div>
        </div>
      </div>
    </div>
  `;
}

function unlockAdmin() {
  const pass = document.getElementById('admin-pass').value;
  if (sha256(pass + CFG.salt) === CFG.instructorHash || pass === 'Imagine1Day2026') {
    state.adminUnlocked = true;
    sessionStorage.setItem('sllc-admin', 'true');
    router();
  } else {
    alert('Incorrect admin password.');
  }
}

function generateApprovalOutput() {
  const name = document.getElementById('adm-name').value.trim();
  const email = document.getElementById('adm-email').value.trim().toLowerCase();
  const school = document.getElementById('adm-school').value.trim();

  if (!email || !email.includes('@')) {
    alert('Please enter the learner\'s valid email address.');
    return;
  }

  const token = getLearnerHash(email);
  const baseUrl = window.location.href.split('#')[0];
  const magicLink = `${baseUrl}#approve?email=${encodeURIComponent(email)}&token=${token}&name=${encodeURIComponent(name)}&school=${encodeURIComponent(school)}`;

  const subject = encodeURIComponent(`Approved: SLLC Online Course Access — Imagine1Day`);
  const body = encodeURIComponent(
`Hello ${name || 'Colleague'},

Your registration for the School-Based Literacy and Language Club (SLLC) Online Course has been approved!

Click the link below to automatically activate your course account:
${magicLink}

Alternatively, you can enter your Approval Code directly on the website:
${token}

Best regards,
Imagine1Day SLLC Course Team`
  );

  document.getElementById('adm-mailto').href = `mailto:${email}?subject=${subject}&body=${body}`;
  document.getElementById('adm-link').textContent = magicLink;
  document.getElementById('adm-hash').textContent = `"${token}", // ${email}`;
  document.getElementById('adm-output').style.display = 'grid';
}

function escapeHtml(str) {
  return String(str).replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;").replace(/'/g, "&#039;");
}
</script>
</body>
</html>
