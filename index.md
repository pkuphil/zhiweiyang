<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Zhiwei Yang CV</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Georgia, serif;
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
      width: 100%;
      max-width: none;
      margin: 0;
    }

    .column {
      padding: 10px;
    }

    .left {
      width: 25%;
    }

    .center {
      width: 50%;
    }

    .right {
      width: 25%;
    }

    img.profile-photo {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
      margin-bottom: 20px;
    }

    section {
      margin-bottom: 20px;
    }

    .construction-banner {
      font-size: 24px;
      padding: 20px 10px;
      text-align: center;
    }

    @media screen and (max-width: 900px) {
      .container {
        flex-direction: column;
      }

      .left, .center, .right {
        width: 100%;
      }
    }
  </style>
</head>
<body>

  <div class="construction-banner">
    <span style="color: red;">This</span>
    <span style="color: orange;">webpage</span>
    <span style="color: lightseagreen;">is</span>
    <span style="color: green;">currently</span>
    <span style="color: blue;">under</span>
    <span style="color: purple;">construction.</span>
  </div>

  <div class="container">
    <!-- 左：照片 + 简介 -->
    <aside class="column left">
      <img src="https://github.com/pkuphil/zhiweiyang/blob/main/WechatIMG826.jpg?raw=true" alt="Profile Photo" class="profile-photo">
      <p>
        I <a href="#">(CV)</a> am a third-year PhD student in the Department of Philosophy at Peking University and currently a visiting student at MIT. I mostly write about philosophy of mind and philosophy of perception.
        I enjoy cooking, wandering aimlessly, cycling, exploring narrative cinema, and reading personal biographies. I'm also a fan of the band Twenty One Pilots and Hong Kong singer Sam Hui.
      </p>
    </aside>

    <!-- 中：Publications + Work In Progress -->
    <main class="column center">
      <section>
        <h2>Publications</h2>
        <p>
          forth. <a href="https://philpapers.org/archive/YANIRP.pdf">Is Rich Phenomenology Fragmented?</a> <em>Synthese</em>.
        </p>
        <p style="font-size: 0.9em; color: #666; margin-top: -10px; margin-left: 20px;">
          <strong>Abstract:</strong> Some philosophers argue that the content of iconic memory is conscious, called the Rich View. However, critics claim that only fragments of the content of iconic memory are conscious, called the Fragment View...
        </p>
      </section>

      <section>
        <h2>Work In Progress</h2>
        <p>Do Semantic Properties Involve the Future?</p>
        <p style="font-size: 0.9em; color: #666; margin-top: -10px; margin-left: 20px;">
          <strong>Abstract:</strong> Temporal externalism claims that a term’s meaning can depend not just on how it has been used in the past or present, but also on how it will be used in the future...
        </p>
      </section>
    </main>

    <!-- 右：会议 + 语言 + 联系 -->
    <aside class="column right">
      <section>
        <h2>Conference Presentations</h2>
        <p>forth. <a href="#">Is Rich Phenomenology Fragmented?</a>, CoRN, Bangkok, Thailand.</p>
        <p>2025.04. <a href="#">Do Semantic Properties Involve the Future?</a>, Pacific APA, San Francisco.</p>
        <p>2025.02. <a href="#">Is Rich Phenomenology Fragmented?</a>, Central APA, Online.</p>
        <p>2025.01. <a href="#">Do Semantics Include Future Properties?</a>, Eastern APA, New York.</p>
        <p>2024.07. <a href="#">Methodological Challenges in Consciousness Concept Research</a>, AAP, Perth.</p>
        <p>2024.04. <a href="#">Methodological Challenges</a>, Workshop, Beijing.</p>
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
        </p>
      </section>
    </aside>
  </div>
</body>
</html>
