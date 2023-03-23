<body>
  <div class="container">
    <ul>
      <li> <a href="/dailies/2023-03-15-svelte-components/each-achievement"> Each Achievment</a> </li>
      <li> <a href= "dailies/2023-03-19-svelte-events/dom-element"> DOM Elements </a> </li>
      <li> <a href= "dailies/2023-03-20-js-objects/adventurers"> Adventurers </a> </li>
      <li> <a href= "dailies/2023-03-21-exported-todos/achievement18"> Exported Todo's</a> </li>
      <li> <a href="/dailies/2023-03-22-route-params/route-param-achievement-19"> Param's Achievemnts</a></li>
    </ul>
  </div>
  </body>    
  

<style>
  .container {
    display: flex;
    flex-direction: column;
    justify-content:center;
    align-items: center;
    flex-grow: 1;

    list-style: none;

    font-size: 26px;
    font-size: 24px; 
    font-family: 'Georgia', serif; 
    font-weight: 400; 
    line-height: 1.5; 
    color: #333; 
  }

  a {
    text-decoration: none;
  }

  ul li {
    display: flex;
    justify-content: center;
    align-items: center;
    border: 2px black solid;
    border-radius: 20px;
    margin: 2rem;
    padding: 10px;
    list-style-type: none;
  }

  ul li:hover {
    background-color: #f0f0f0;
    cursor: pointer;
    transition: background-colour 0.3s ease;
  }
  </style>

