
<!-- JAVASCRIPT -->

<script>

  import ItensMenu from  '$lib/ItensMenu.svelte'
  

</script>


<!-- COMPONENTE HTML -->

  <header class="navbar bg-base-100 drop-shadow-md fixed w-full z-10">

    <!-- NAVBAR START -->
    <div class="navbar-start">

      <!-- DROPDOWN MENU -->
      <div class="dropdown">

        <!-- ICON HAMBURGUER -->
        <div tabindex="0" role="button" class="btn btn-ghost lg:hidden">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h8m-8 6h16" /></svg>
        </div>

        <!-- LISTA MENU -->
        <ul tabindex="0" class="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow bg-base-100 rounded-box w-52">

          <!-- ITENS MENU -->
          <ItensMenu/>

        </ul>

      </div>

      <!-- LOGO -->
      <a href="/" class="btn btn-ghost">
        <img class="w-28" src="https://i.ibb.co/JscvfxN/Group-26.png" alt="logo">
      </a>

    </div>

    <!-- NAVBAR END -->
    <div class="navbar-end hidden lg:flex">

      <!-- LISTA MENU -->
      <ul class="menu menu-horizontal px-1">

         <!-- ITENS MENU -->
          <ItensMenu/>
   
      </ul>

    </div>


  </header>
