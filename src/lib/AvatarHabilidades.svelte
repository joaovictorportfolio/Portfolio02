
<!-- JAVASCRIPT -->

<script>

  export let dataTip
  export let src


</script>


<!-- COMPONENTE HTML -->

  <div class="tooltip flutuar " data-tip={dataTip}>

    <div class="avatar">

      <div class="w-20 max-lg:w-16 rounded-full hover:ring ring-primary ring-offset-base-100 ring-offset-2 ">

        <img class="scale-75 overflow-visible" {src} on:load />

      </div>

    </div>

  </div>