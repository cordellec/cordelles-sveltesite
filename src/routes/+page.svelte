<script>
  import Header from '$lib/components/Header.svelte';
  import Wrapper from '$lib/components/Wrapper.svelte';
</script>
<body>
<div class="container">
  <div class="card">
    <p>
      Hello, my name is Cordelle, and this is my Website that I have created
      for school for my Web Dev program! I will be using this website as a way
      to track my work, and as a journal through my coding adventures.
    </p>
  </div>
</div>
</body>

<style>
  :global(body) {
    margin: 0;
    font-family:'Times New Roman', Times, serif;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    background: linear-gradient(#ffecd2, #fcb69f);
  }

  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-grow: 1;
  }

  .card {
    background-color: #f0f0f0;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    max-width: 80%;
    text-align: center;
  }

  p {
    margin: 0;
  }
</style>
