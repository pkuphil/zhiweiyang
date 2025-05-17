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

    .left, .center, .right {
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

    .toggle-title {
      cursor: pointer;
      font-weight: 500;
      display: flex;
      align-items: center;
      gap: 8px;
      font-size: 1em;
      color: #444;
      transition: color 0.3s ease;
      user-select: none;
      padding: 5px 0;
    }

    .toggle-title:hover {
      color: #000;
    }

    .toggle-icon {
      width: 14px;
      height: 14px;
      transition: transform 0.3s ease;
      transform: rotate(0deg);
    }

    .toggle-title.expanded .toggle-icon {
      transform: rotate(90deg);
    }

    .wip-abstract {
      max-height: 0;
      overflow: hidden;
      opacity: 0;
      transition: max-height 0.4s ease, opacity 0.3s ease;
      color: #777;
    }

    .wip-abstract.show {
      max-height: 1000px;
      opacity: 1;
    }
  </style>
</head>
<body>
  <!-- 页面结构保持不变，只折叠功能升级 -->

  <!-- 中栏 Work In Progress 部分示例 -->
  <section id="wip-section">
    <h2>Work In Progress</h2>
    <div style="margin: 10px 0;" id="wip-tags"></div>

    <div data-tag="mind language" class="wip-item">
      <p class="toggle-title expanded" onclick="toggleAbstract(this)">
        <svg class="toggle-icon" viewBox="0 0 20 20" fill="currentColor"><path d="M6 4l8 6-8 6V4z"/></svg>
        Do Semantic Properties Involve the Future?
      </p>
      <div class="wip-abstract show">
        <p style="font-size: 0.9em; margin-top: -10px; margin-left: 20px;">
          <strong>Abstract:</strong> Temporal externalism claims that a term’s meaning can depend not just on how it has been used in the past or present, but also on how it will be used in the future... 
        </p>
      </div>
    </div>

    <div data-tag="perception mind" class="wip-item">
      <p class="toggle-title" onclick="toggleAbstract(this)">
        <svg class="toggle-icon" viewBox="0 0 20 20" fill="currentColor"><path d="M6 4l8 6-8 6V4z"/></svg>
        Cross-modal Experiences and the Problem of Phenomenal Overlap
      </p>
      <div class="wip-abstract">
        <p style="font-size: 0.9em; margin-top: -10px; margin-left: 20px;">
          <strong>Abstract:</strong> This paper discusses the challenge posed by Mehta’s “phenomenal overlap argument” to naïve realism...
        </p>
      </div>
    </div>
  </section>

  <script>
    function toggleAbstract(element) {
      const abstract = element.nextElementSibling;
      const isVisible = abstract.classList.contains('show');
      element.classList.toggle('expanded', !isVisible);
      abstract.classList.toggle('show', !isVisible);
    }
  </script>
</body>
</html>
