
<!-- JAVASCRIPT -->

<script>
  
  let selected = 'Início'; 
  
  const menuItems = ['Início', 'Sobre', 'Habilidades', 'Trabalhos', 'Contato'];

  function selecionar(item) {
    selected = item;
  }

</script>

<!-- COMPONENTE HTML -->


  {#each menuItems as item}
    <li>
      <a href="/{item=='Início'?'':item}" class:active={selected === item} on:click={() => selecionar(item)}>{item}</a>
    </li>
  {/each}

