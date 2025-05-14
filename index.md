<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Zhiwei Yang CV</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
<div class="construction-banner">
  ⚠️ This webpage is currently under construction.
</div>

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
        My research focuses on the philosophy of mind and perception. 
      </p>
    </aside>

    <!-- Center Column: Main Content -->
    <main class="column center">

      <!-- Publications -->
      <section>
        <h2>Publications</h2>
        <p>
          forth. <a href="#">Is Rich Phenomenology Fragmented?</a> <em>Synthese</em>.
        </p>
      </section>

      <!-- Conference Presentations -->
      <section>
        <h2>Conference Presentations</h2>
        <p>forth. <a href="#">Is Rich Phenomenology Fragmented?</a>, CoRN, Bangkok. </p>
        <p>2025.04. <a href="#">Do Semantic Properties Involve the Future?</a>, Pacific APA, San Francisco.</p>
        <p>2025.02. <a href="#">Is Rich Phenomenology Fragmented?</a>, Central APA, Online.</p>
        <p>2025.01. <a href="#">Do Semantics Include Future Properties?</a>, Eastern APA, New York.</p>
        <p>2024.07. <a href="#">Methodological Challenges in Consciousness Concept Research</a>, AAP, Perth.</p>
        <p>2024.04. <a href="#">Methodological Challenges in Consciousness Concept Research</a>, Workshop for Young Scholars in Science and Philosophy, Beijing.</p>
      </section>

    <!-- Right Column: Contact Info -->
    <aside class="column right">
      <h2>Contact</h2>
      <p>
        Department of Philosophy<br>
        Peking University<br>
        550 Memorial Drive<br>
        Cambridge, MA 02136<br>
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
