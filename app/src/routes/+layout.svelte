<script>
    let categories = ["Fun", "Weird", "Icebreaker"];
</script>

<nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="/">Road Trip Questions</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="/">Fun</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="/weird">Weird</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="/icebreaker">Icebreakers</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="/would-you-rather">Would you rather</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <slot/>

<style>
       /* Card styling */
   .category-card {
    display: block;
    margin: 20px auto;
    padding: 20px;
    max-width: 300px;
    background-color: #ff5722;
    color: white;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    text-decoration: none;
    font-weight: bold;
    transition: background-color 0.3s ease;
  }

  .category-card:hover {
    background-color: #e64a19;
    transform: translateY(-5px);
  }
</style>
