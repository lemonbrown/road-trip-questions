<script>
    import { questions } from '../../stores/questions.js';
  
     // Reactive variable for selected category
     let selectedCategory = 'Weird'; 
  
    // Filter questions based on selected category
    let filteredQuestions = questions.filter(q => q.category === selectedCategory);
  </script>
  
  
  
  <main class="container my-2">
    <h1 class="text-center">150 Weird Road Trip Questions</h1>
    <ol class="question-container">
      {#each filteredQuestions as { question }, index}
        <li> {question}</li>
      {/each}
    </ol>

    <a href="/would-you-rather" class="category-card">
        Try 150 Would You Rather Questions
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
  