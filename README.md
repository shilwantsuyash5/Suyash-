# Suyash-
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Suyash — Personal Profile</title>
  <meta name="description" content="Personal profile of Suyash. Student, learner, and aspiring professional." />
  <style>
    :root{
      --bg:#f7f9fb;
      --card:#ffffff;
      --accent:#246BFD;
      --muted:#666;
      --radius:12px;
      --max-width:900px;
      --gap:18px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      color:#12202b;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background:linear-gradient(180deg,var(--bg),#eef4ff 60%);
      display:flex;
      align-items:flex-start;
      justify-content:center;
      padding:32px;
      min-height:100vh;
    }
    .container{
      width:100%;
      max-width:var(--max-width);
      background:var(--card);
      border-radius:var(--radius);
      box-shadow:0 8px 30px rgba(16,40,60,0.08);
      padding:28px;
      display:grid;
      grid-template-columns: 220px 1fr;
      gap:var(--gap);
      align-items:start;
    }
    header{
      grid-column:1 / -1;
      display:flex;
      align-items:center;
      gap:18px;
      margin-bottom:4px;
    }
    .avatar{
      width:96px;
      height:96px;
      border-radius:12px;
      overflow:hidden;
      flex:0 0 96px;
      box-shadow:0 4px 14px rgba(36,107,253,0.12);
    }
    .avatar img{width:100%;height:100%;object-fit:cover;display:block}
    h1{font-size:20px;margin:0}
    .intro{color:var(--muted);font-size:14px}
    .left{
      display:flex;
      flex-direction:column;
      gap:14px;
    }
    .card{
      background:linear-gradient(180deg,#fff,#fbfdff);
      border-radius:10px;
      padding:14px;
      box-shadow:0 4px 12px rgba(12,30,50,0.04);
    }
    .section{
      margin-bottom:8px;
    }
    .personal-details dt{font-weight:600}
    .personal-details dd{margin:6px 0 0 0;color:var(--muted)}
    table{
      width:100%;
      border-collapse:collapse;
      font-size:14px;
    }
    th,td{
      padding:10px 12px;
      border-bottom:1px solid #eef2f6;
      text-align:left;
    }
    th{background:#fbfdff;font-weight:600}
    ul.skills{list-style:none;padding:0;margin:0;display:flex;flex-wrap:wrap;gap:8px}
    ul.skills li{
      background:#eef5ff;color:var(--accent);
      padding:6px 10px;border-radius:8px;font-weight:600;font-size:13px;
    }
    .achievements li{margin-bottom:8px}
    .right{
      display:flex;
      flex-direction:column;
      gap:14px;
    }
    footer{grid-column:1 / -1;text-align:center;color:var(--muted);font-size:13px;margin-top:6px}
    @media (max-width:780px){
      .container{grid-template-columns:1fr;padding:18px}
      .avatar{width:80px;height:80px;flex:0 0 80px}
      header{flex-direction:row;align-items:center}
    }
  </style>
</head>
<body>
  <main class="container" role="main" aria-label="Suyash personal profile">
    <header>
      <div class="avatar" aria-hidden="false">
        <img src="https://via.placeholder.com/400" alt="Profile photo of Suyash">
      </div>
      <div>
        <h1>Suyash</h1>
        <div class="intro">Student • Lifelong learner • Improving every day</div>
      </div>
    </header>

    <aside class="left" aria-label="Sidebar">
      <section class="card section" aria-labelledby="about-heading">
        <h2 id="about-heading" style="margin:0 0 10px 0;font-size:15px">About Me</h2>
        <p>Hello! My name is <strong>Suyash</strong>. I am a student who loves learning new skills and improving myself every day.</p>
        <p><strong>Career Objective:</strong> <mark>To become a successful professional and contribute to the growth of the organization.</mark></p>
        <dl class="personal-details" aria-label="Personal details">
          <dt>Name:</dt><dd>Suyash</dd>
          <dt>City:</dt><dd>Solapur</dd>
          <dt>Country:</dt><dd>India</dd>
        </dl>
      </section>

      <section class="card section" aria-labelledby="education-heading">
        <h3 id="education-heading" style="margin:0 0 10px 0">Education</h3>
        <figure style="margin:0">
          <table role="table" aria-label="Educational details">
            <caption style="text-align:left;padding:6px 12px 0 0;font-weight:600;color:var(--muted)">Educational Details</caption>
            <thead>
              <tr><th scope="col">Class</th><th scope="col">Institute</th><th scope="col">Year</th></tr>
            </thead>
            <tbody>
              <tr><td>SSC</td><td>ABC School</td><td>2022</td></tr>
              <tr><td>HSC</td><td>XYZ College</td><td>2024</td></tr>
            </tbody>
          </table>
        </figure>
      </section>
    </aside>

    <section class="right" aria-label="Main content">
      <div class="card section" aria-labelledby="skills-heading">
        <h3 id="skills-heading" style="margin:0 0 10px 0">Skills</h3>
        <ul class="skills" aria-label="Skills list">
          <li>C Programming</li>
          <li>HTML</li>
          <li>Communication</li>
        </ul>
      </div>

      <div class="card section" aria-labelledby="hobbies-heading">
        <h3 id="hobbies-heading" style="margin:0 0 10px 0">Hobbies</h3>
        <ul>
          <li>Sports</li>
          <li>Reading</li>
          <li>Travelling</li>
        </ul>
      </div>

      <div class="card section" aria-labelledby="achievements-heading">
        <h3 id="achievements-heading" style="margin:0 0 10px 0">Achievements</h3>
        <ol class="achievements">
          <li><strong>Participated in GitHub Weekly Commit Challenge</strong></li>
          <li><strong>Won Coding Competition</strong></li>
        </ol>
      </div>
    </section>

    <footer>
      Built with ❤️ • Last updated: 2026-01-11
    </footer>
  </main>
</body>
</html>
