<script>
  /************/
  /* Player 1 */
  /************/

  // Player 1 general
  // const player1Name = 'Ryan Reynolds';
  // const player1Race = 'human';
  // const player1Class = 'rogue';
  // let player1Level = 1;
  // let player1Health = 8;

  // Player 1 effects
  // let player1Poisoned = true;

  // Player 1 items
  // let player1Backpack = [
  //     'rusty knife',
  //     'gem',
  //     'journal'
  //   ];

  const player1 = {
    name: 'Ryan Reynolds',
    race: 'human',
    class: 'rogue',
    level: 1,
    health: 8,
    poisoned: true,
    backpack: [
      'rusty knife',
      'gem',
      'journal'
    ]
  }

  /************/
  /* Player 2 */
  /************/

  const player2 = {
    name: "Gyda",
    race: "dwarf",
    class: "fighter",
    level: 1,
    health: 12,
    poisoned: false,
    backpack: [
      'sword',
      'leather armour',
      'rations'
    ]
  }
  /************/
  /* Player 3 */
  /************/

  const player3 = {
    name: "Anna",
    race: "elf",
    class: "wizard",
    level: 1,
    health: 9,
    poisoned: true,
    backpack: [
      'staff',
      'cloak',
      'spell book'
    ]

  }
</script>
<div class="container">
<main>
  
  <h1>List of Adventurers</h1>
  <div class="card">
  <h2>Rogue</h2>
    <h3>{player1.name}</h3>
    <ul>
      <li>Race: {player1.race}</li>
      <li>Class: {player1.class}</li>
      <li>Level: {player1.level}</li>
      <li>Health: {player1.health}</li>
      <li>Poisoned: {player1.poisoned}</li>
      <li>Backpack:
        <ul>
          {#each player1.backpack as item}
            <li>{item}</li>
          {/each}
        </ul>
      </li>
    </ul>
  </div>
  <div class="card">
  <h2>Fighter</h2>
    <h3>{player2.name}</h3>
    <ul>
      <li>Race: {player2.race}</li>
      <li>Class: {player2.class}</li>
      <li>Level: {player2.level}</li>
      <li>Health: {player2.health}</li>
      <li>Poisoned: {player2.poisoned}</li>
      <li>Backpack:
        <ul>
          {#each player2.backpack as item}
            <li>{item}</li>
          {/each}
        </ul>
      </li>
    </ul>
  </div>
  <div class="card">
  <h2>Wizard</h2>
    <h3>{player3.name}</h3>
    <ul>
      <li>Race: {player3.race}</li>
      <li>Class: {player3.class}</li>
      <li>Level: {player3.level}</li>
      <li>Health: {player3.health}</li>
      <li>Poisoned: {player3.poisoned}</li>
      <li>Backpack:
        <ul>
          {#each player3.backpack as item}
            <li>{item}</li>
          {/each}
        </ul>
      </li>
    </ul>
  </div>
</main>
</div>

<style>
  .card {
    border: 1px black solid;
    border-radius: 20px;
    padding: 2rem;
    margin: 2rem;
    box-sizing: border-box;
    box-shadow: 2px 2px;
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