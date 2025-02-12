---
layout: post
title: "Connections: The Long Chain"
date: 2025-02-02
featured_image:
tags: [Connections, Questioning Life, Technology, History]
---

<a href="https://archive.org/details/bbc-connections-1978/Connections/S01/S01E07+-+The+Long+Chain.mkv" target="_blank">
  <img src="/images/posts/Blog2/Connections.jpg" alt="Connections: The Long Chain">
</a>

<div class="carousel">
  <div class="carousel-items">
    <div class="carousel-item">
      <a href="https://en.wikipedia.org/wiki/Fluyt" target="_blank">
        <img src="/images/posts/Blog2/Fluyt.jpg" alt="Fluyt">
        <h3>Fluyt</h3>
      </a>
    </div>
    <div class="carousel-item">
      <a href="https://en.wikipedia.org/wiki/Lloyd%27s_of_London" target="_blank">
        <img src="/images/posts/Blog2/Lloid.jpg" alt="Lloyd's Coffee House">
        <h3>Lloyd's Coffee House</h3>
      </a>
    </div>
    <div class="carousel-item">
      <a href="https://en.wikipedia.org/wiki/Tar" target="_blank">
        <img src="/images/posts/Blog2/Tar.jpg" alt="Connection 3">
        <h3>Tar</h3>
      </a>
    </div>
    <div class="carousel-item">
      <a href="https://en.wikipedia.org/wiki/Gas_lighting" target="_blank">
        <img src="/images/posts/Blog2/Gaslighting.jpg" alt="Connection 3">
        <h3>Gas Lighting</h3>
      </a>
    </div>
    <div class="carousel-item">
      <a href="https://en.wikipedia.org/wiki/Mackintosh" target="_blank">
        <img src="/images/posts/Blog2/Mackintosh.jpg" alt="Connection 3">
        <h3>Mackintosh</h3>
      </a>
    </div>
    <div class="carousel-item">
      <a href="https://en.wikipedia.org/wiki/Mauveine" target="_blank">
        <img src="/images/posts/Blog2/Mauv2.jpg" alt="Connection 3">
        <h3>Mauveine</h3>
      </a>
    </div>
    <div class="carousel-item">
      <a href="https://en.wikipedia.org/wiki/Fertilizer" target="_blank">
        <img src="/images/posts/Blog2/Fertilizer.jpg" alt="Connection 3">
        <h3>Fertilizer</h3>
      </a>
    </div>
    <div class="carousel-item">
      <a href="https://en.wikipedia.org/wiki/TNT" target="_blank">
        <img src="/images/posts/Blog2/TNT.jpg" alt="Connection 3">
        <h3>Explosives</h3>
      </a>
    </div>
    <div class="carousel-item">
      <a href="https://en.wikipedia.org/wiki/World_War_I" target="_blank">
        <img src="/images/posts/Blog2/World_War_I.jpg" alt="Connection 3">
        <h3>World War I</h3>
      </a>
    </div>
    <div class="carousel-item">
      <a href="https://en.wikipedia.org/wiki/Plastic" target="_blank">
        <img src="/images/posts/Blog2/plastic.jpeg" alt="Connection 3">
        <h3>Plastic</h3>
      </a>
    </div>
  </div>
  <button class="prev" onclick="moveToPreviousSlide()"> ❮ </button>
  <button class="next" onclick="moveToNextSlide()"> ❯ </button>
</div>

<style>
/* Improved Carousel Styling */
.carousel {
  position: relative;
  width: 100%;
  max-width: 1200px;
  margin: 2rem auto;
  overflow: hidden;
}

.carousel-items {
  display: flex;
  transition: transform 0.5s ease;
  min-height: 400px; /* Set minimum height for consistency */
}

.carousel-item {
  min-width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 20px;
  box-sizing: border-box;
}

.carousel-item a {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-decoration: none;
  color: #333;
  height: 100%;
  width: 100%;
}

.carousel img {
  max-width: 100%;
  max-height: 70vh; /* Limits image height while maintaining aspect ratio */
  width: auto;
  height: auto;
  object-fit: contain;
  margin: 0 auto;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.carousel h3 {
  margin: 15px 0 0 0;
  font-size: 1.2rem;
  text-align: center;
  padding: 0 20px;
  color: #2c3e50;
}

/* Updated Navigation Buttons with Black Background */
.prev, .next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(0,0,0,0.7); /* Black with 70% opacity */
  border: none;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  cursor: pointer;
  box-shadow: 0 2px 8px rgba(0,0,0,0.3);
  transition: all 0.3s ease;
  align-items: center;
  justify-content: center;
}


.prev:hover, .next:hover {
  background: rgba(0,0,0,0.9); /* Darker on hover */
  transform: translateY(-50%) scale(1.1);
}

.prev::after, .next::after {
  content: '';
  width: 12px;
  height: 12px;
  border-top: 2px solid white; /* White arrows */
  border-right: 2px solid white; /* White arrows */
}

/* Keep the rest of your existing styles */

.prev::after {
  transform: rotate(-135deg);
  margin-left: 4px;
}

.next::after {
  transform: rotate(45deg);
  margin-right: 4px;
}

.prev { left: 20px; }
.next { right: 20px; }

/* Responsive Design */
@media (max-width: 768px) {
  .carousel-items {
    min-height: 300px;
  }
  
  .carousel img {
    max-height: 50vh;
  }
  
  .prev, .next {
    width: 32px;
    height: 32px;
  }
  
  .carousel h3 {
    font-size: 1rem;
  }
}
</style>

<script>
  window.addEventListener('resize', () => {
  document.querySelector('.carousel-items').style.transform = 
    `translateX(-${currentIndex * 100}%)`;
});
  let currentIndex = 0;
  const items = document.querySelectorAll('.carousel-item');
  const totalItems = items.length;

  function moveToNextSlide() {
    currentIndex = (currentIndex + 1) % totalItems;
    updateCarousel();
  }

  function moveToPreviousSlide() {
    currentIndex = (currentIndex - 1 + totalItems) % totalItems;
    updateCarousel();
  }

  function updateCarousel() {
    const offset = -currentIndex * 100;
    document.querySelector('.carousel-items').style.transform = `translateX(${offset}%)`;
  }
</script>
