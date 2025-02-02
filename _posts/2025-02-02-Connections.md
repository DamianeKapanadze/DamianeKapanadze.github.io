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
        <img src="/images/posts/Blog2/plastic.jpg" alt="Connection 3">
        <h3>Plastic</h3>
      </a>
    </div>
  </div>
  <button class="prev" onclick="moveToPreviousSlide()">❮</button>
  <button class="next" onclick="moveToNextSlide()">❯</button>
</div>

<style>
.carousel {
  display: flex;
  align-items: center; /* Vertically centers the items */
  position: relative;
  width: 100%;
  overflow: hidden;
}

.carousel-items {
  display: flex;
  transition: transform 0.5s ease;
}

.carousel-item {
  min-width: 100%;
  box-sizing: border-box;
  display: flex;
  justify-content: center; /* Horizontally centers the content */
  align-items: center; /* Vertically centers the content */
}

.carousel img {
  width: 75%;
  height: auto;
  object-fit: contain; /* Ensures the entire image is visible */
}

.prev, .next {
  position: absolute;
  top: 50%;
  padding: 16px;
  font-size: 18px;
  color: white;
  background-color: rgba(0, 0, 0, 0.5);
  border: none;
  cursor: pointer;
  border-radius: 3px;
  transform: translateY(-50%);
}

.prev {
  left: 0;
}

.next {
  right: 0;
}

.prev:hover, .next:hover {
  background-color: rgba(0, 0, 0, 0.8);
}


</style>

<script>
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
