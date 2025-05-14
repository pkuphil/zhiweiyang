<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Zhiwei Yang CV</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <!-- Image Carousel -->
  <div class="carousel">
    <div class="carousel-images">
      <img src="photo1.jpg" alt="Slide 1">
      <img src="photo2.jpg" alt="Slide 2">
      <img src="photo3.jpg" alt="Slide 3">
    </div>
    <button class="prev">&#10094;</button>
    <button class="next">&#10095;</button>
  </div>

  <div class="container">
    
    <!-- Left Column: Bio -->
    <aside class="column left">
      <p>
        I am a PhD student in the Department of Philosophy at Peking University,
        currently a visiting student at the Department of Linguistics and Philosophy at MIT.
        My research focuses on the philosophy of mind and perception. I am currently working on my dissertation.
      </p>
    </aside>

    <!-- Center Column: Main Content -->
    <main class="column center">

      <!-- Publications -->
      <section>
        <h2>Publications</h2>
        <p>
          Forthcoming. <a href="#">Is Rich Phenomenology Fragmented?</a> <em>Synthese</em>.
        </p>
      </section>

      <!-- Conference Presentations -->
      <section>
        <h2>Conference Presentations</h2>
        <p>2025.07 – <a href="#">Is Rich Phenomenology Fragmented?</a>, CoRN, Bangkok. <span class="source">[forthcoming]</span></p>
        <p>2025.04 – <a href="#">Do Semantic Properties Involve the Future?</a>, Pacific APA, San Francisco.</p>
        <p>2025.02 – <a href="#">Is Rich Phenomenology Fragmented?</a>, Central APA, Online.</p>
        <p>2025.01 – <a href="#">Do Semantics Include Future Properties?</a>, Eastern APA, New York.</p>
        <p>2024.07 – <a href="#">Methodological Challenges in Consciousness Concept Research</a>, AAP, Perth.</p>
        <p>2024.04 – <a href="#">Methodological Challenges in Consciousness Concept Research</a>, Chinese Academy of Sciences, Beijing.</p>
      </section>

      <!-- Graduate Coursework -->
      <section>
        <h2>Graduate Coursework <small>(* indicates auditor status)</small></h2>
        <ul>
          <li>Good Food: The Ethics & Politics of Food* – Spring 2025, MIT</li>
          <li>Minds and Machines* – Spring 2025, MIT</li>
          <li>The Problems of Philosophy* – Spring 2025, MIT</li>
          <li>Ethics of Technology* – Spring 2025, MIT</li>
          <li>Philosophy: Research and Writing* – Fall 2024, Peking University</li>
          <li>Philosophy: Research and Writing* – Spring 2024, Peking University</li>
          <li>Epistemology* – Spring 2024, Peking University</li>
          <li>Selected Reading of Medieval Philosophy – Spring 2023, Peking University</li>
          <li>Philosophy: Research and Writing – Spring 2023, Peking University</li>
          <li>Phenomenology and Ethics – Spring 2023, Peking University</li>
          <li>Philosophy of Language – Fall 2022, Peking University</li>
          <li>Philosophical Methods – Fall 2022, Peking University</li>
          <li>Philosophy of Mind – Fall 2021, Shandong University</li>
          <li>Proseminar – Fall 2021, Shandong University</li>
          <li>Philosophy of Cognitive Science – Fall 2021, Shandong University</li>
          <li>Logic and Philosophy – Fall 2021, Shandong University</li>
          <li>Logic and Language – Spring 2020, Shandong University</li>
          <li>Philosophy of Science – Spring 2020, Shandong University</li>
        </ul>
      </section>

      <!-- Teaching Experience -->
      <section>
        <h2>Teaching Experience</h2>
        <ul>
          <li>Teaching Assistant, “Epistemology” – Fall 2024, Peking University</li>
          <li>Teaching Assistant, “Epistemology” – Spring 2024, Peking University</li>
          <li>Teaching Assistant, “Introduction to Philosophy” – Fall 2023, Peking University</li>
          <li>Teaching Assistant, “Introduction to Philosophy” – Fall 2022, Peking University</li>
          <li>Teaching Assistant, “Applied Logic” – Fall 2021, Shandong University</li>
          <li>Teaching Assistant, “Applied Logic” – Fall 2020, Shandong University</li>
        </ul>
      </section>

      <!-- Awards and Fellowships -->
      <section>
        <h2>Awards and Fellowships</h2>
        <ul>
          <li>Peking University Presidential Scholarship – 2024</li>
          <li>Peking University International Study Grant – 2024</li>
          <li>Graduate Student Stipend, Pacific APA – 2024</li>
          <li>Graduate Student Stipend, Central APA – 2024</li>
          <li>Travel Stipend, Eastern APA – 2024</li>
        </ul>
      </section>
    </main>

    <!-- Right Column: Contact Info -->
    <aside class="column right">
      <h2>Contact</h2>
      <p>
        Department of Philosophy<br>
        Peking University<br>
        550 Memorial Drive<br>
        Cambridge, MA 02136<br>
        Office: +1 617-233-3173
      </p>
      <p>
        <a href="mailto:allenminesky@gmail.edu">allenminesky@gmail.edu</a><br>
        <a href="mailto:yangjia@mit.edu">yangjia@mit.edu</a>
      </p>
    </aside>
  </div>

  <!-- JavaScript for Carousel -->
  <script>
    let index = 0;
    const images = document.querySelector('.carousel-images');
    const totalSlides = images.children.length;

    function showSlide(i) {
      index = (i + totalSlides) % totalSlides;
      images.style.transform = `translateX(-${index * 100}%)`;
    }

    document.querySelector('.prev').addEventListener('click', () => showSlide(index - 1));
    document.querySelector('.next').addEventListener('click', () => showSlide(index + 1));

    setInterval(() => {
      showSlide(index + 1);
    }, 5000);
  </script>
</body>
</html>
