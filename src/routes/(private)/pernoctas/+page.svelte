<script>
  class pernocta{
    constructor(brand, model, plate, owner, tlf, inDate, debt){
        this.brand = brand,
        this.model = model,
        this.plate = plate,
        this.owner = owner,
        this.tlf = tlf,
        this.date = inDate,
        this.debt = debt
    }
}

const pernoctas = []



// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))



// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))


// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))

// pernoctas.push(new pernocta('ford', 'fiesta', "ADL56S", "Pedro Perez", "04243342354", new Date().toLocaleString(), 20))




</script>

<section class="w-11/12 h-screen">
    <table class="flex relative table w-full min-h-1/2 max-h-auto flex-col border-gray-1px text-center">

        <header id="header-categories" class="grid grid-cols-7 mb-2 [&>*]: ">
          
          <th>Marca</th>
          <th>Modelo</th>
          <th>Placa</th>
          <th>Propietario</th>
          <th>Telefono</th>
          <th>Fecha de Ingreso</th>
          <th>Debe pagar:</th>
        </header>
      
      {#if !pernoctas.length}
          <h1 class="absolute top-1/2  left-[calc(50%-105.5px)]">No hay pernoctas registradas!</h1>
      {/if}
      {#each pernoctas as pernocta}
      <tr class="grid grid-cols-7  [&>*]: flex justify-center align-middle">
        <td>{pernocta.brand}</td>
        <td>{pernocta.model}</td>
        <td>{pernocta.plate}</td>
        <td>{pernocta.owner}</td>
        <td>{pernocta.tlf}</td>
        <td>{pernocta.date}</td>
        <td>{`${pernocta.debt}$`}</td>
      </tr>
      {/each}
    </table> 
  </section>

  <style></style>
  