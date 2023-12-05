
<!-- JAVASCRIPT -->

<script>

  import Loading from '$lib/Loading.svelte';

	let loading = true

</script>


<!-- COMPONENTE HTML -->

  {#if loading}<Loading/>{/if}

  <section class="h-screen w-full hero bg-base-200 px-10 max-lg:px-4">

    <div class="hero-content flex-col lg:flex-row justify-between gap-20 max-lg:gap-10">

      <figure class="w-1/3 max-xl:w-1/3 max-lg:w-[100%] max-sm:w-full max-lg:h-64 max-sm:h-52 overflow-hidden rounded-xl">

          <img 
          src="https://i.ibb.co/CthJqky/image.png" 
          class="max-lg:scale-[1] max-sm:scale-[1] origin-top w-full h-96 max-sm:-translate-y-2 rounded-x" on:load={()=>loading=false}/>
     
      </figure>
  
      <div class="max-w-xl space-y-6">

        <h1 class="text-3xl max-lg:text-2xl font-bold">Dando vida a ideias com <strong>criatividade e código 👨‍💻</strong></h1>

        <p class="lg:text-lg">Minha jornada é sobre <strong>transformar visões em realidade.</strong> Cada linha de código que escrevo é uma expressão da minha <strong>paixão</strong> por <strong>criar experiências digitais únicas.</strong> Transformando conceitos de design em <strong>interfaces interativas e funcionais.</strong></p>
    

      </div>

    </div>

  </section>