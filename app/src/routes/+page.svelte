<head>
  <meta name="description" content="A collection of 150 fun questions for your road trip!">
  <meta name="keywords" content="road trip, fun questions, weird questions, road trip questions, travel, conversation starters">
  <meta name="robots" content="index, follow">
  <meta property="og:title" content="Road Trip Questions">
  <meta property="og:description" content="Find fun questions to ask on your next road trip.">
  <meta property="og:image" content="URL_TO_IMAGE"> <!-- Replace with an actual image URL -->
  <meta property="og:url" content="https://www.yourwebsite.com">
</head>

<script context="module" lang="ts">
  import { questions } from '../stores/questions.js';

   // Reactive variable for selected category
   let selectedCategory = 'Fun';

  // Filter questions based on selected category
  let filteredQuestions = questions.filter(q => q.category === selectedCategory);

  export const prerender = true;
</script>



<main class="container my-2">
  <h1 class="text-center">150 Fun Road Trip Questions</h1>
  <ol class="question-container">
    {#each filteredQuestions as { question }, index}
      <li> {question}</li>
    {/each}
  </ol>

  <a href="/weird" class="category-card">
    Try 150 Weird Questions
  </a>
</main>

  <!-- Footer -->
  <footer class="bg-light text-center text-lg-start mt-5">
    <div class="container p-4">
      <p>&copy; 2024 Road Trip Questions | All rights reserved</p>
      <div>
        <a href="#" class="me-4 text-decoration-none">Privacy</a>
        <a href="#" class="me-4 text-decoration-none">Terms</a>
        <a href="#" class="me-4 text-decoration-none">Contact</a>
      </div>
    </div>
  </footer>

<style>


  main {
    max-width: 900px;
    margin: 0 auto;
    padding-top: 50px;
  }

  h1 {
    font-family: 'Arial', sans-serif;
    color: #007BFF;
    margin-bottom: 30px;
  }


  /* Heading styling */
  h1 {
    text-align: center;
    font-size: 2rem;
    color: #333;
  }


</style>
