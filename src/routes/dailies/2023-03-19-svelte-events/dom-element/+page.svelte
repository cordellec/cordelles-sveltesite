<script>
  let src = "https://picsum.photos/seed/picsum/400/400";

  let counter = 0;
  let countList = [];
  const handleClick = () => {
    counter++;
    // Method 1: Adding to arrays in SvelteKit
    countList.push(counter);
    countList = countList;
    // Method 2
    // countList[countList.length] = counter;
    // Method 3 (advanced-ish)
    // countList = [...countList, counter];
    // console.log(countList);
  }

 /*  if (counter % 15 === 0) {
    console.log("FizzBuzz");
  } else if ( counter % 5  === 0 ) {
    console.log("Buzz")
  } else if ( counter % 3 === 0) {
    console.log ("Fizz")
  } else {
    console.log(counter)
  }
*/
</script>
<div class="container">
<main>
  <img src="{src}" alt="Random Image">
  <h3>This is a card.</h3>
  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi, porro!</p>
</main>

<div class="container"></div>

<main>
  <h1>Push of a FizzBuzz</h1>
  <button on:click={handleClick}>Counter: {counter}</button>
  <ul>
    {#each countList as count}
      {#if count % 15 === 0}
        <li>FizzBuzz</li>
      {:else if count % 3 === 0}
        <li>Fizz</li>
      {:else if count % 5 === 0}
        <li>Buzz</li>
      {:else}
        <li>{count}</li>
      {/if}
    {/each}
  </ul>
</main>
</div>



<style>
main {
  width: 30ch;
  border: 2px solid black;
  background-color: cadetblue;
  padding: 2rem;
  margin: auto;
  
}

img {
  width: 100%;
  height: auto;
  display: block;
}



.container {
	display: flex;
	flex-direction: column;
	justify-content:center;
	align-items: center;
	flex-grow: 1;
  margin: 2rem;
}

</style>