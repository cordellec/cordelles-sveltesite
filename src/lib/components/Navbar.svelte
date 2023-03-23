<script>
  let links = [
    { name: 'Home', url: '/' },
    { name: 'Dailies', url: '/dailies' },
    { name: 'Journal', url: '/journal' },
  ];
</script>

<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Lora:400,700&display=swap" />


<nav class="navbar">
  <a href="/" class="nav-item">Cordelle's School Work Website</a>
  <div>
    {#each links as link}
      <a href="{link.url}" class="nav-item">{link.name}</a>
    {/each}
  </div>
</nav>

<style>
  .navbar {
    display: flex;
    justify-content: space-between;
    background-color: #e6dcdc;
    padding: 1rem;
    font-family:Georgia, 'Times New Roman', Times, serif
  }

  .nav-item {
    color: black;
    text-decoration: none;
    margin-left: 1rem;
    font-family: 'lora', serif;
    font-weight: 500;
  }

  .nav-item:hover {
    color: #666;
  }
</style>
