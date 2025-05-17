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
      <section>
        <h2>Research</h2>
        <section>
        <h3>Publications</h3>
        <p>
          forth. <a href="#">Is Rich Phenomenology Fragmented?</a> <em>Synthese</em>
  <a href="https://philpapers.org/archive/YANIRP.pdf" style="font-size: 0.85em; font-style: italic; color: gray; margin-left: 5px;">[draft]</a>.
        </p>
        <p style="font-size: 0.9em; color: #666; margin-top: -10px; margin-left: 20px;">
          <strong>Abstract:</strong> Some philosophers argue that the content of iconic memory is conscious, called the Rich View. However, critics claim that only fragments of the content of iconic memory are conscious, called the Fragment View. Both sides cite different psychological experimental data to support their positions. Proponents of the Fragment View tend to assert that their view uniquely explains the data they rely on. The uniqueness of the Fragment View is challenged here. Newly introduced evidence suggests that the data supporting the Fragment View may also be compatible with the Rich View. Given the theoretical advantages of the Rich View in other respects, there are reasons to consider it the superior one.
        </p>
      </section>

      <section>
        <h3>Work In Progress</h3>
        <p>Do Semantic Properties Involve the Future?</p>
        <p style="font-size: 0.9em; color: #666; margin-top: -10px; margin-left: 20px;">
          <strong>Abstract:</strong> Temporal externalism claims that a term’s meaning can depend not just on how it has been used in the past or present, but also on how it will be used in the future. This paper challenges that view through an analysis of the Druid case, arguing that to account for semantic continuity, temporal externalists must assume that speakers hold a stable, unconscious (placeholder) belief that lets a term keep tracking the same properties over time—even before future contexts arise. But this assumption is problematic: either it credits speakers with hidden knowledge of the future, which over-intellectualizes everyday language use, or it relies on vague dispositions with little explanatory value. The paper argues that neither option convincingly supports the idea that future use can determine past meaning. Without a clearer link between current mental states and future linguistic practice, temporal externalism falls short of improving on standard externalist theories.
        </p>
      </section>
    </main>

    <!-- 右栏 -->
    <aside class="right">
      <section>
        <h2>Conference Presentations</h2>

        <!-- ✅ 筛选标签按钮 -->
        <div style="margin: 10px 0;">
          <strong></strong>
          <!-- 按钮将在 JS 中动态生成 -->
        </div>

        <!-- ✅ 添加标签到每条记录 -->
        <p data-tag="CoRN">forth. <a href="#">Is Rich Phenomenology Fragmented?</a>, CoRN, Bangkok, Thailand. </p>
        <p data-tag="APA">2025.04. <a href="#">Do Semantic Properties Involve the Future?</a>, Colloquium, Pacific APA, San Francisco, CA, USA.</p>
        <p data-tag="APA">2025.02. <a href="#">Is Rich Phenomenology Fragmented?</a>, Colloquium, Central APA, Online.</p>
        <p data-tag="APA">2025.01. <a href="#">Do Semantics Include Future Properties?</a>, Work in Progress, Eastern APA, New York, NY, USA.</p>
        <p data-tag="AAP">2024.07. <a href="#">Methodological Challenges in Consciousness Concept Research</a>, Colloquium, Australasian Association of Philosophy, Perth, WA, Australia.</p>
        <p data-tag="WYSSP">2024.04. <a href="#">Methodological Challenges in Consciousness Concept Research</a>, Colloquium, Workshop for Young Scholars in Science and Philosophy, Beijing, China.</p>
      </section>
    </aside>
  </div>

  <!-- ✅ JavaScript for tag filtering with counts -->
  <script>
    document.addEventListener("DOMContentLoaded", () => {
      const events = document.querySelectorAll('[data-tag]');
      const counts = {};

      // Count occurrences of each tag
      events.forEach(el => {
        const tag = el.dataset.tag;
        counts[tag] = (counts[tag] || 0) + 1;
      });

      const tags = ['APA', 'AAP', 'CoRN', 'WYSSP'];
      const filterDiv = document.querySelector('div[style*="margin: 10px 0"]');

      // Create "All" button
      filterDiv.innerHTML = '<strong>Filter:</strong> <button onclick="filterEvents(\'all\')">All (' + events.length + ')</button>';

      // Create a button for each tag
      tags.forEach(tag => {
        const count = counts[tag] || 0;
        const button = document.createElement('button');
        button.textContent = `${tag} (${count})`;
        button.setAttribute('onclick', `filterEvents('${tag}')`);
        filterDiv.appendChild(button);
      });
    });

    function filterEvents(tag) {
      const events = document.querySelectorAll('[data-tag]');
      events.forEach(el => {
        el.style.display = (tag === 'all' || el.dataset.tag === tag) ? 'block' : 'none';
      });
    }
  </script>

</body>
</html>
