<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>10th Grade Notes - Karnataka</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #eaf6f6;
      margin: 0;
      padding: 0;
      text-align: center;
    }
    h1 {
      margin: 20px;
      color: #333;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 20px;
      padding: 20px;
      max-width: 1000px;
      margin: auto;
    }
    .card {
      background: #fff;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .card h2 {
      font-size: 18px;
      margin: 10px 0;
      color: #222;
    }
    .card p {
      font-size: 14px;
      color: #555;
    }
    .btn {
      display: inline-block;
      margin-top: 10px;
      padding: 8px 16px;
      background: teal;
      color: #fff;
      border-radius: 5px;
      text-decoration: none;
      transition: 0.3s;
    }
    .btn:hover {
      background: darkcyan;
    }
  </style>
</head>
<body>

  <h1>10th Grade Notes - Karnataka</h1>

  <div class="grid">
    <div class="card">
      <h2>Maths Chapter 1 Notes</h2>
      <p>Subject: Maths</p>
      <a class="btn" href="C:\Users\DELL\Downloads" target="_blank">Open PDF</a>
    </div>

    <div class="card">
      <h2>Science Chapter 1 Notes</h2>
      <p>Subject: Science</p>
      <a class="btn" href="C:\Users\DELL\Downloads\SPOORTHI-Eng-Final.pdf" target="_blank">Open PDF</a>
    </div>

    <div class="card">
      <h2>English Grammar Notes</h2>
      <p>Subject: English</p>
      <a class="btn" href="C:\Users\DELL\Downloads\1st-Lang-English.pdf" target="blank
      <!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>PDF Viewer - 10th Grade Notes</title>
<style>
  :root{
    --sidebar-w: 240px;
    --bg: #f4fbfb;
    --accent: #0b91a8;
    --muted: #666;
  }
  body{
    margin:0;
    font-family: Arial, sans-serif;
    background:var(--bg);
    color:#111;
    height:100vh;
    display:flex;
    gap:12px;
  }
  .sidebar{
    width:var(--sidebar-w);
    background:#fff;
    border-right:1px solid #e6f0f0;
    padding:16px;
    display:flex;
    flex-direction:column;
    gap:12px;
  }
  .logo { font-weight:700; color:var(--accent); font-size:16px }
  .list{flex:1; overflow:auto; padding-top:6px}
  .list button{
    width:100%;
    text-align:left;
    padding:10px;
    border-radius:8px;
    border:1px solid transparent;
    background:transparent;
    cursor:pointer;
    margin-bottom:6px;
  }
  .list button:hover{ background:#f7fdfd; border-color:#e0f2f4 }
  .main{
    flex:1;
    display:flex;
    flex-direction:column;
    height:100vh;
    padding:12px;
    gap:8px;
  }
  .toolbar{
    display:flex; gap:8px; align-items:center; flex-wrap:wrap;
    background:#fff;
    padding:8px; border-radius:8px; box-shadow: 0 1px 2px rgba(0,0,0,0.05);
  }
  .toolbar button {
    padding:6px 10px; border-radius:6px; border:1px solid #ddd; background:#fff; cursor:pointer;
  }
  .viewer-wrap{
    flex:1;
    background:#fff;
    border:1px solid #e7f0f0;
    border-radius:8px;
    overflow:hidden;
    position:relative;
    display:flex;
    flex-direction:column;
  }
  #pdfViewer{
    width:100%;
    height:100%;
    border:0;
    background:#ddd;
    transform-origin: top left;
  }
</style>
</head>
<body>
  <aside class="sidebar">
    <div class="logo">📘 Subjects</div>
    <div class="list" id="pdfList"></div>
  </aside>

  <main class="main">
    <div class="toolbar">
      <button id="zoomIn">Zoom +</button>
      <button id="zoomOut">Zoom -</button>
      <button id="resetZoom">Reset</button>
      <div style="flex:1"></div>
      <span id="currentInfo" style="font-size:13px;color:#666">none</span>
    </div>

    <div class="viewer-wrap">
      <iframe id="pdfViewer"></iframe>
    </div>
  </main>

<script>
const samplePDFs = [
  {title: "Maths Chapter 1", url: "C:\Users\DELL\Downloads"},
  {title: "Science Chapter 1", url: "C:\Users\DELL\Downloads\SPOORTHI-Eng-Final.pdf"},
  {title: "English Grammar", url: "C:\Users\DELL\Downloads"},
  {title: "Kannada Chapter 1", url: "C:\Users\DELL\Downloads"},
  {title: "Social Science Chapter 1", url: "C:\Users\DELL\Downloads"}
];

const pdfList = document.getElementById('pdfList');
const pdfViewer = document.getElementById('pdfViewer');
const zoomIn = document.getElementById('zoomIn');
const zoomOut = document.getElementById('zoomOut');
const resetZoom = document.getElementById('resetZoom');
const currentInfo = document.getElementById('currentInfo');

let currentURL = null;
let scale = 1;

function addListItem(title, url){
  const btn = document.createElement('button');
  btn.textContent = title;
  btn.onclick = ()=> loadPDF(url, title);
  pdfList.appendChild(btn);
}
samplePDFs.forEach(p => addListItem(p.title, p.url));

function loadPDF(url, title){
  currentURL = url;
  pdfViewer.src = url;
  scale = 1;
  pdfViewer.style.transform = scale(${scale});
  currentInfo.textContent = title;
}

zoomIn.onclick = ()=> { scale += 0.2; pdfViewer.style.transform = scale(${scale}); };
zoomOut.onclick = ()=> { scale = Math.max(0.2, scale - 0.2); pdfViewer.style.transform = scale(${scale}); };
resetZoom.onclick = ()=> { scale = 1; pdfViewer.style.transform = scale(${scale}); };
</script>
</body>
</html>
