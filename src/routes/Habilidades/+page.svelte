
<!-- JAVASCRIPT -->

<script>

  import AvatarHabilidades from '$lib/AvatarHabilidades.svelte'
  import Loading from '$lib/Loading.svelte';

	let loading = true

  let objAvatarHabilidades = [

    {key:'html',value:'https://i.ibb.co/6DVS5hS/image.png'},
    {key:'css',value:'https://i.ibb.co/NZBQYRC/image.png'},
    {key:'javascript',value:'https://i.ibb.co/Xsh9LBW/image.png'},
    {key:'tailwind',value:'https://i.ibb.co/3Njmxpm/image.png'},
    {key:'firebase',value:'https://i.ibb.co/ZG3CjtM/image.png'},
    {key:'svelte',value:'https://i.ibb.co/p2J035h/image.png'},
    {key:'figma',value:'https://i.ibb.co/rd6sTkh/image.png'},

  ]

</script>

{#if loading}<Loading/>{/if}


<!-- COMPONENTE HTML -->

  <section class="flex items-center justify-center h-screen w-full bg-base-200 px-10 max-lg:px-0">

    <div class="flex flex-col items-center justify-center gap-16">

      <h2 class="text-2xl lg:text-3xl font-semibold">Minhas habilidades</h2>

      <div class="grid grid-cols-3 gap-8 drop-shadow-lg flutuar max-lg:px-10">

        {#each objAvatarHabilidades as objAvatarHabilidade , i }

          <AvatarHabilidades 
            dataTip={objAvatarHabilidade.key} 
            src={objAvatarHabilidade.value}
            on:load={()=>loading=false}
          />

        {/each}
        

      </div>

    </div>


  </section>