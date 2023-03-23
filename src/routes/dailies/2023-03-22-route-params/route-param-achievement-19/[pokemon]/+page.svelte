<script>
  import { page } from '$app/stores'

  console.log($page.params.pokemon);
</script>



<div class="container">

<h1> {$page.params.pokemon}</h1>

</div>


<style>
  .container {
	display: flex;
	flex-direction: column;
	justify-content:center;
	align-items: center;
	flex-grow: 1;
  margin: 2rem;
}

</style>