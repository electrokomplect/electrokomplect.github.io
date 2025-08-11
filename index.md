<!-- minimal, clean business-card in Markdown with a bit of CSS -->
<style>
:root{
  --bg:#0b0f14; --card:#0f1521; --text:#e6edf3; --muted:#98a6b8; --border:#1f2a3a; --chip:#172132; --accent:#7dcfff;
}
*{box-sizing:border-box}
body{background:var(--bg); color:var(--text); font:16px/1.6 Inter, system-ui, Segoe UI, Roboto, Arial, sans-serif;}
.page{max-width:980px;margin:32px auto;padding:0 20px}
.card{background:linear-gradient(180deg,rgba(255,255,255,.02),rgba(255,255,255,0)),var(--card); border:1px solid var(--border); border-radius:18px; padding:22px 24px; box-shadow:0 10px 40px rgba(0,0,0,.35); }
h1{margin:.2rem 0 0;font-size:28px}
h2{margin:1.6rem 0 .8rem;font-size:18px}
.sub{color:var(--muted); margin-top:6px}
.row{display:grid; grid-template-columns:1.1fr .9fr; gap:18px}
@media(max-width:860px){.row{grid-template-columns:1fr}}
.badges{display:flex;flex-wrap:wrap;gap:8px;margin-top:10px}
.badge{font-size:12px;padding:6px 10px;border-radius:999px;background:var(--chip);border:1px solid var(--border)}
.stack,.chips{display:flex;flex-wrap:wrap;gap:8px}
.chip{background:var(--chip);border:1px solid var(--border);padding:8px 10px;border-radius:12px;font-size:13px}
.list{list-style:none;padding:0;margin:0;display:grid;gap:10px}
.item{display:flex;gap:10px}
.dot{width:8px;height:8px;border-radius:50%;background:var(--accent);margin-top:.6em;box-shadow:0 0 10px var(--accent)}
.links{display:flex;flex-wrap:wrap;gap:12px;margin-top:8px}
.btn{display:inline-block;text-decoration:none;color:var(--text);border:1px solid var(--border);background:linear-gradient(180deg,#1a2433,#121a28);padding:10px 14px;border-radius:12px;font-weight:600}
.btn:hover{border-color:#335173}
.small{color:var(--muted);font-size:13px}
.center{text-align:center;margin-top:16px}
.hr{height:1px;background:var(--border);margin:18px 0}
.logo-line{display:flex;flex-wrap:wrap;gap:10px}
.logo{padding:6px 10px;border:1px solid var(--border);border-radius:10px;background:var(--chip);font-size:13px}
</style>

<div class="page">
  <div class="card">
    <h1>Igor Melin</h1>
    <div class="sub">Data / Analytics Engineer — ETL/ELT • DWH • BI • DataOps</div>
    <div class="badges">
      <span class="badge">B2B / Remote (EU)</span>
      <span class="badge">RU / EN (B2)</span>
      <span class="badge">Postgres • ClickHouse • Airflow • dbt</span>
    </div>

<div class="hr"></div>

<div class="row">
  <div>
    <h2>Чем помогаю</h2>
    <ul class="list">
      <li class="item"><span class="dot"></span><div>Проектирую и поднимаю <b>DWH</b> под отчётность и продуктовую аналитику.</div></li>
      <li class="item"><span class="dot"></span><div>Собираю стабильные <b>ETL/ELT</b> пайплайны (Airflow, dbt, Python).</div></li>
      <li class="item"><span class="dot"></span><div>Оптимизирую <b>BI</b> контуры: модель, агрегаты, SLA, стоимость.</div></li>
      <li class="item"><span class="dot"></span><div>Внедряю <b>DataOps</b>: контейнеризация, CI/CD, тесты, мониторинг.</div></li>
    </ul>

    <h2>С кем работал</h2>
    <div class="logo-line">
      <span class="logo">Triafly</span>
      <span class="logo">Sber</span>
      <span class="logo">Heineken</span>
      <span class="logo">Power Machines</span>
      <span class="logo">Novardis</span>
      <span class="logo">OCRV (РЖД)</span>
    </div>

    <h2>Выбранные результаты</h2>
    <ul class="list">
      <li class="item"><span class="dot"></span><div>Вынес отчётность в внешнее хранилище на <b>ClickHouse</b> → прирост скорости и возможностей BI (Triafly).</div></li>
      <li class="item"><span class="dot"></span><div>Интегрировал <b>SAP BW → Power BI</b> для управления запасами (Heineken).</div></li>
      <li class="item"><span class="dot"></span><div>Моделировал хранилище на <b>SAP HANA</b>, отчёты в SAP Analysis (Sber, RE).</div></li>
      <li class="item"><span class="dot"></span><div>Запустил бюджетирование на <b>SAP IP</b> с интеграциями FM/OpenText (Power Machines).</div></li>
    </ul>
  </div>

  <div>
    <h2>Технологии</h2>
    <div class="stack">
      <span class="chip">Airflow</span><span class="chip">dbt</span><span class="chip">Python</span><span class="chip">Kafka</span>
      <span class="chip">Spark</span><span class="chip">Docker</span><span class="chip">GitHub Actions</span>
      <span class="chip">Postgres</span><span class="chip">ClickHouse</span><span class="chip">SAP HANA</span>
      <span class="chip">Databricks/Fabric</span><span class="chip">Power BI</span><span class="chip">Superset</span>
      <span class="chip">Linux</span>
    </div>

    <h2>Пишу и выступаю</h2>
    <ul class="list">
      <li class="item"><span class="dot"></span><div><a class="btn" href="https://habr.com/ru/post/658895/">Habr: Аналитика профессии в три клика</a></div></li>
      <li class="item"><span class="dot"></span><div><a class="btn" href="https://habr.com/ru/articles/716374/">Habr: Market analytics of a profession</a></div></li>
      <li class="item"><span class="dot"></span><div><a class="btn" href="https://medium.com/@gorin.igor/how-to-connect-to-sap-hana-from-power-bi-6376b9df4747">Medium: Power BI ↔ SAP HANA</a></div></li>
    </ul>

    <h2>Контакты</h2>
    <div class="links">
      <a class="btn" href="mailto:melin.igor@gmail.com">melin.igor@gmail.com</a>
      <a class="btn" href="https://t.me/electronic_555">Telegram</a>
      <a class="btn" href="https://github.com/electrokomplect">GitHub</a>
    </div>

    <p class="small" style="margin-top:10px">Мальта • Remote • B2B</p>
  </div>
</div>

<div class="hr"></div>
<div class="center small">© Igor Melin. Open to short audits, PoC и долгосрочные контракты.</div>

  </div>
</div>
