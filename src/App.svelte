<script>
  import Hello from './lib/helllo.svelte'

  class pernocta{
    constructor(brand, model, owner){
        this.brand = brand,
        this.model = model,
        this.owner = owner
    }
}

const pernoctas = []

// pernoctas.push(new pernocta('ford', 'fiesta', "luis"))
// pernoctas.push(new pernocta('toyota', 'corolla', 'samuel'))

console.log(pernoctas)


</script>

<main class="flex justify-center">

  <section class="w-11/12 h-screen">
    <table class="flex relative w-full min-h-1/2 max-h-auto flex-col border-gray-1px text-center">
      <tr>
        <header class="flex justify-evenly">
          <th>Marca</th>
          <th>Modelo</th>
          <th>Propietario</th>
        </header>
      </tr>
      {#if !pernoctas.length}
          <h1 class="absolute top-1/2 left-">No hay pernoctas registradas!</h1>
      {/if}
      {#each pernoctas as pernocta}
      <tr class="flex justify-evenly">
        <td>{pernocta.brand}</td>
        <td>{pernocta.model}</td>
        <td>{pernocta.owner}</td>
      </tr>
      {/each}
    </table> 
  </section>
  
</main>

<style>

</style>
