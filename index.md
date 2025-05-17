---
layout: default
title: ""
---
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <style>
    * {
      box-sizing: border-box;
    }

    html, body {
      margin: 0;
      padding: 0;
      font-family: 'Georgia', serif;
      overflow-x: hidden;
      font-size: 16.5px;
    }

    a {
      text-decoration: none;
      color: darkblue;
    }

    a:hover {
      text-decoration: underline;
    }

    .container {
      display: flex;
      width: 100vw;
      padding-left: 10px;
      padding-right: 10px;
      gap: 20px;
      transform: translateX(-220px) scale(0.8);
      transform-origin: top left;
    }

    .left,
    .center,
    .right {
      padding-top: 10px;
      padding-bottom: 10px;
    }

    .left {
      flex: 1;
      min-width: 220px;
    }

    .center {
      flex: 2;
      min-width: 400px;
    }

    .right {
      flex: 1.2;
      min-width: 250px;
    }

    img.profile-photo {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
      margin-bottom: 20px;
    }

    section {
      margin-bottom: 30px;
    }

    @media screen and (max-width: 900px) {
      .container {
        flex-direction: column;
        padding-left: 10px;
        padding-right: 10px;
      }

      .left, .center, .right {
        width: 100%;
      }

      .center {
        min-width: auto;
      }
    }
  </style>
</head>
<body>

  <div class="construction-banner" style="font-size: 24px; margin: 20px; text-align: center;">
    <span style="color: red;">This</span>
    <span style="color: orange;">webpage</span>
    <span style="color: lightseagreen;">is</span>
    <span style="color: green;">currently</span>
    <span style="color: blue;">under</span>
    <span style="color: purple;">construction.</span>
  </div>

  <div style="font-size: 24px; margin-top: -10px; margin-bottom: 20px; text-align: center; color: black;">
    Zhiwei Yang
  </div>

  <div class="container">
    <!-- 左栏 -->
    <aside class="left">
      <img src="https://github.com/pkuphil/zhiweiyang/blob/main/WechatIMG826.jpg?raw=true" alt="Profile Photo" class="profile-photo">
      <p>
        I <a href="#">(CV)</a> am a third-year PhD student in the Department of Philosophy at Peking University and currently a visiting student at MIT. I mostly write about philosophy of mind and philosophy of perception.
        I enjoy cooking, wandering aimlessly, cycling, exploring narrative cinema, and reading personal biographies. I'm also a fan of the band Twenty One Pilots and Hong Kong singer Sam Hui.
      </p>

      <section>
        <h2>Interview</h2>
        <p><a href="https://blog.apaonline.org/2025/03/28/apa-member-interview-zhiwei-yang/" target="_blank">This is my APA Member interview</a></p>
      </section>
      
      <section>
        <h2>Language</h2>
        <p>
          Chinese (Native)<br>
          English (Okay, IELTS 8.0)
        </p>
      </section>

      <section>
        <h2>Contact</h2>
        <p>
          <a href="mailto:allenminesky@gmail.edu">allenminesky@gmail.com</a><br>
          <a href="mailto:yangjia@mit.edu">yangjia@mit.edu</a>
          <a href="mailto:2201110913@stu.pku.edu.cn">2201110913@stu.pku.edu.cn</a>
        </p>
      </section>
    </aside>

    <!-- 中栏 -->
    <main class="center">

      <section id="publications-section">
        <h2>Publications</h2>
        <div style="margin: 10px 0;" id="pub-tags"></div>
        <p data-tag="mind">forth. <a href="#">Is Rich Phenomenology Fragmented?</a> <em>Synthese</em>
          <a href="https://philpapers.org/archive/YANIRP.pdf" style="font-size: 0.85em; font-style: italic; color: gray; margin-left: 5px;">[draft]</a>.
        </p>
        <p style="font-size: 0.9em; color: #666; margin-top: -10px; margin-left: 20px;">
          <strong>Abstract:</strong> Some philosophers argue that the content of iconic memory is conscious, called the Rich View. However, critics claim that only fragments of the content of iconic memory are conscious, called the Fragment View. ...
        </p>
      </section>

      <section id="wip-section">
        <h2>Work In Progress</h2>
        <div style="margin: 10px 0;" id="wip-tags"></div>
        <p data-tag="mind language">Do Semantic Properties Involve the Future?</p>
        <p style="font-size: 0.9em; color: #666; margin-top: -10px; margin-left: 20px;">
          <strong>Abstract:</strong> Temporal externalism claims that a term’s meaning can depend not just on how it has been used in the past or present, but also on how it will be used in the future...
        </p>
      </section>
    </main>

    <!-- 右栏 -->
    <aside class="right">
      <section>
        <h2>Conference Presentations</h2>
        <div style="margin: 10px 0;" id="right-tags"></div>
        <p data-tag="CoRN">forth. <a href="#">Is Rich Phenomenology Fragmented?</a>, CoRN, Bangkok, Thailand. </p>
        <p data-tag="APA">2025.04. <a href="#">Do Semantic Properties Involve the Future?</a>, Colloquium, Pacific APA, San Francisco, CA, USA.</p>
        <p data-tag="APA">2025.02. <a href="#">Is Rich Phenomenology Fragmented?</a>, Colloquium, Central APA, Online.</p>
        <p data-tag="APA">2025.01. <a href="#">Do Semantics Include Future Properties?</a>, Work in Progress, Eastern APA, New York, NY, USA.</p>
        <p data-tag="AAP">2024.07. <a href="#">Methodological Challenges in Consciousness Concept Research</a>, Colloquium, Australasian Association of Philosophy, Perth, WA, Australia.</p>
        <p data-tag="WYSSP">2024.04. <a href="#">Methodological Challenges in Consciousness Concept Research</a>, Colloquium, Workshop for Young Scholars in Science and Philosophy, Beijing, China.</p>
      </section>
    </aside>
  </div>

  <!-- ✅ JavaScript for independent tag filtering -->
  <script>
    document.addEventListener("DOMContentLoaded", () => {
      setupTagFilters('right', ['APA', 'AAP', 'CoRN', 'WYSSP'], '.right');
      setupTagFilters('pub', ['mind'], '#publications-section');
      setupTagFilters('wip', ['mind', 'language'], '#wip-section');
    });

    function setupTagFilters(sectionId, tags, scopeSelector) {
      const container = document.querySelector(`#${sectionId}-tags`);
      const items = document.querySelectorAll(`${scopeSelector} [data-tag]`);
      const counts = {};

      items.forEach(item => {
        const tagList = item.dataset.tag.split(/\s+/);
        tagList.forEach(tag => {
          counts[tag] = (counts[tag] || 0) + 1;
        });
      });

      container.innerHTML = `<strong>Filter:</strong> <button onclick="filterByTag('${sectionId}', 'all', '${scopeSelector}')">All (${items.length})</button>`;

      tags.forEach(tag => {
        const btn = document.createElement('button');
        btn.textContent = `${tag} (${counts[tag] || 0})`;
        btn.setAttribute('onclick', `filterByTag('${sectionId}', '${tag}', '${scopeSelector}')`);
        container.appendChild(btn);
      });
    }

    function filterByTag(sectionId, tag, scopeSelector) {
      const items = document.querySelectorAll(`${scopeSelector} [data-tag]`);
      items.forEach(item => {
        const tags = item.dataset.tag.split(/\s+/);
        item.style.display = tag === 'all' || tags.includes(tag) ? 'block' : 'none';
      });
    }
  </script>

</body>
</html>
