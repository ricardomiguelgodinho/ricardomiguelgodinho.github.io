---
layout: archive
title: "Fieldwork"
permalink: /fieldwork/
author_profile: true
---

I've been involved in the excavation of burial sites spanning from the Mesolithic to the 20th century. Here is a selection of some of the contexts.

<div class="image-carousel">
  <button class="carousel-arrow prev" aria-label="Previous image">&#10094;</button>

  <div class="carousel-viewport">
    <div class="carousel-track">
      <img src="/images/fieldwork/horta_joao_moura_1.JPG" alt="Fieldwork at Horta João Moura">
      <img src="/images/fieldwork/outeiro_alto_1.jpg" alt="Fieldwork at Outeiro Alto">
      <img src="/images/fieldwork/outeiro_alto_2.jpg" alt="Fieldwork at Outeiro Alto">
      <img src="/images/fieldwork/outeiro_alto_3.jpg" alt="Fieldwork at Outeiro Alto">
      <img src="/images/fieldwork/outeiro_alto_4.jpg" alt="Fieldwork at Outeiro Alto">
      <img src="/images/fieldwork/outeiro_alto_5.jpg" alt="Fieldwork at Outeiro Alto">
      <img src="/images/fieldwork/outeiro_alto_6.jpg" alt="Fieldwork at Outeiro Alto">
      <img src="/images/fieldwork/parque_anel_verde_1.png" alt="Fieldwork at Parque Anel Verde">
      <img src="/images/fieldwork/ribeira_sao_domingos_1.jpg" alt="Fieldwork at Ribeira São Domingos">
      <img src="/images/fieldwork/xancra_1.png" alt="Fieldwork at Xancra">
    </div>
  </div>

  <button class="carousel-arrow next" aria-label="Next image">&#10095;</button>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const carousel = document.querySelector(".image-carousel");
  if (!carousel) return;

  const track = carousel.querySelector(".carousel-track");
  const images = Array.from(track.querySelectorAll("img"));
  const prevBtn = carousel.querySelector(".carousel-arrow.prev");
  const nextBtn = carousel.querySelector(".carousel-arrow.next");

  let currentIndex = 0;

  function updateCarousel() {
    track.style.transform = `translateX(-${currentIndex * 100}%)`;
    prevBtn.disabled = currentIndex === 0;
    nextBtn.disabled = currentIndex === images.length - 1;
  }

  prevBtn.addEventListener("click", function () {
    if (currentIndex > 0) {
      currentIndex--;
      updateCarousel();
    }
  });

  nextBtn.addEventListener("click", function () {
    if (currentIndex < images.length - 1) {
      currentIndex++;
      updateCarousel();
    }
  });

  updateCarousel();
});
</script>
