<template>
  <div class="hobbies">
    <div class="page-title">
      <h2>{{ hobbiePageTitle }}</h2>
    </div>

    <div class="hobbie">
        <h2>{{title}}</h2>
      <p>{{ hobbie }}</p>
    </div>

    <div class="others">
      <h2>{{ othersTitle }}</h2>
      <p>{{ others }}</p>
    </div>
  </div>
</template>

<style scoped>
.hobbies{
    padding: 10px;
}
.hobbie{
    text-align: center;
}
.hobbie p {
    padding: 0rem 10rem 0rem 10rem;
}
.others{
    text-align: center;
}

</style>

<script>
export default {
  name: 'Hobbies',
  data () {
    return {
      /** Hobbies */
      title: 'Hobbies',
      hobbiePageTitle: 'Hobbies e interesses',
      hobbie: 'Os meus maiores Hoobies são: ler livros relacionados com temas actuais e tecnológicos, jogar capoeira, fazer stand Up Comedy e teatro, andar de bicicleta em tempos livres e tocar guitarra',
      /** Others */
      othersTitle: 'Outros',
      others: 'As vezes uma vez ou outra, gosto de ir a praia, ir ao cinama e fazer compras'
    }
  }
}
</script>
