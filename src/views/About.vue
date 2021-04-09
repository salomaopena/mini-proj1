<template>
  <div class="about">
    <div class="page-title">
        <h2>{{pageTitle}}</h2>
    </div>

    <div class="job-experience">
        <h2>{{jobExperienceTitle}}</h2>
        <p>{{jobExp1}}</p>
    </div>

    <div class="languages">
        <h2>{{laguageTitle}}</h2>
        {{portuguese}} <br/>{{english}}
    </div>
    <div class="events">
        <h2>{{eventTitle}} </h2>
        {{event1}} <br/> {{event2}} <br/>{{event3}}<br/>{{event4}} <br/>{{event5}} <br/>{{event6}} <br/>{{event7}}
    </div>
  </div>
</template>

<style  scoped>
.job-experience{
  text-align: center;
}
.job-experience p{
  padding: 0rem 10rem 0rem 10rem;
}
.languages{
  text-align: center;
}

.events{
  text-align: center;
  background-color:#F5F5F7;
}
</style>

<script>

export default {
  name: 'About',
  data () {
    return {
      pageTitle: 'O que faço?',
      /** Job experiences */
      jobExperienceTitle: 'Experiência de trabalho',
      jobExp1: 'Actualmente trabalho como Professor no Instituto Superior de Ciências de Educação da Huíla (ISCED-Huíla). De Julho, 2017 – até a data actual, trabalho também com Gestor de Projectos, Programador de aplicações para dispositivos móveis com Flutter na StartUp Fênix Innovation, Soluções, Serviçoes e Treinamentos Lda. Já fui Líder da Área Técnico-Científica da Associação de Estudantes do Instituto Superior de Ciências de Educação da Huíla de 2015 a 2018.',
      /** Laguages Spoken */
      laguageTitle: 'Línguas faladas',
      portuguese: 'Português - Fluentemente',
      english: 'Inglês - Fluentemente',
      /** Events */
      eventTitle: 'Eventos',
      event1: 'Desaprenda: semana do professor - Instituto Ânima',
      event2: 'Membro da comunidade de aprendizagem do Instituto Ânima - Brasil',
      event3: 'Hackthon na Disruption Lab, powered by Antlântico, Banco Antlântico - Angola',
      event4: 'Workshop do Fullstack Angular e Spring - Algaworks',
      event5: 'Participou no 19th South African Regional ACM Collegiate Programming Competition em 2017',
      event6: 'Participou no Concurso de programação Angolan Collegiate Programming Contest 2017',
      event7: 'Participou no Workshop em Ciências da Computação tendências e desafios: I&D em Angola 2017'
    }
  }
}
</script>
