<template>
  <div class="home">
    <Index msg="Quem sou eu?" />
    <div class="wrapper">
      <div class="me">
        <div class="foto">
          <img src="../assets/me4.jpg" alt="Perfil" />
        </div>
        <div class="myself">
          <h3>{{ name }}</h3>
          <table>
            <tr>
              <td>
                <b>{{ nationality }}</b>
              </td>
              <td>{{ country }}</td>
            </tr>
            <tr>
              <td>
                <b>{{ from }}</b>
              </td>
              <td>{{ province }}</td>
            </tr>
            <tr>
              <td>
                <b>{{ bithday }}</b>
              </td>
              <td>{{ date }}</td>
            </tr>
            <tr>
              <td>
                <b>{{ residence }}</b>
              </td>
              <td>{{ street }}</td>
            </tr>
            <tr>
              <td>
                <b>{{ contact }}</b>
              </td>
              <td>{{ phone }}</td>
            </tr>
            <tr>
              <td>
                <b>{{ othersContact }}</b>
              </td>
              <td>{{ email1 }} | {{ email2 }}</td>
            </tr>
          </table>
        </div>
      </div>

      <div class="information">
        <div class="profile">
          <h2>{{ profileTitle }}</h2>
          {{ profile }}
        </div>
        <div class="about-me">
          <h2>{{ aboutMeTitle }}</h2>
          {{ message1 }} <br />
          {{ message2 }} <br />
          {{ message3 }}
        </div>
      </div>
      <div class="education">
        <h2>{{ educationTitle }}</h2>
        <p>{{ year }}</p>
        <p>
          <b>{{ course }}</b>
        </p>
        <p>
          <i>{{ institution }}</i>
        </p>
      </div>
      <div class="course">
        <h2>{{ courseTitle }}</h2>

        <div v-for="x in courses" :key="x.name">
          <b>{{ x.name }}</b> {{ x.course }}
        </div>
      </div>
      <div class="events">
        <h2>{{ eventTitle }}</h2>
        {{ event1 }} <br />
        {{ event2 }} <br />{{ event3 }}<br />{{ event4 }} <br />{{ event5 }}
        <br />{{ event6 }} <br />{{ event7 }}
      </div>
    </div>
  </div>
</template>

<style scoped>
.home {
  background-color: #fbfbfd;
}
.me{
display: flex;
}
.me .foto{
  padding: 0rem 0rem 0rem 7rem;
  text-align: center;
}
.me .foto img{
  border-radius: 360px;
  height: auto;
  width: 50%;
}

.me .myself{
  padding: 2rem 7rem 0rem 0rem;
}
.me .myself h3{
  color:#0071E3;
  font-weight: bold;
}

.information{
  width: 100%;
  display: flex;
  background-color:#F5F5F7;
}
.profile{
  padding: 2rem;
  float: left;
  width:50%;
  text-align:justify;
}
.about-me{
  padding: 2rem;
  float: right;
  width: 50%;
  text-align:justify;
}

.education{
  text-align:center;
}
.course{
  text-align: center;
  background-color:#F5F5F7;
}
.events{
  text-align: center;
}
</style>

<script>
// @ is an alias to /src
import Index from '@/components/Index.vue'

export default {
  name: 'Home',
  components: {
    Index
  },
  data () {
    return {
      pageTitle: 'Quem sou eu?',
      name: 'Salomao Bento Nilo Pena',
      nationality: 'Nacionalidade:',
      country: 'Angolana',
      from: 'Naturalidade:',
      province: 'Bié',
      bithday: 'Nascido:',
      date: '22 de Março de 1991',
      residence: 'Residência:',
      street: 'Rua 8 de Fevereiro, Senhora do Monte, Lubango-Huíla',
      contact: 'Contactos:',
      phone: '(+244) 928079933 | 997079933',
      othersContact: 'Email:',
      email1: 'spenna.live@gmail.com',
      email2: 'salomao.pena@isced-huila.ed.ao',
      /* Profile */
      profileTitle: 'Perfil',
      profile: 'Licenciado em Informática pelo ISCED-HUILA, Programador e desenvolvedor de sistemas Java web based e sites dinâmicos com 4 anos de experiências de trabalho.Ser eficiente e mostrar profissionalismos ao trabalho que lhe for atribuído é o principal objectivo para mostrar o seu potencial.',
      /* About me */
      aboutMeTitle: 'Sobre mim',
      message1: 'Jovem organizado, altamente motivando a aceitar a responsabilidade, gostando de trabalhar em alto nível de integridade.',
      message2: 'Sua mentalidade e personalidade permitem-lhe associar-se a outras pessoas.',
      message3: 'Honestidade, pontualidade, simpatia, assiduidade, respeito às autoridades e ao próximo.',
      /* Education */
      educationTitle: 'Educação',
      year: '2014-2017',
      course: 'Licenciatura em informática',
      institution: 'ISCED-HUILA',
      /* Courses */
      courseTitle: 'Cursos complementares',
      courses: [
        { name: 'Avaliação e evidências de aprendizagem', course: ' Instituto Ânima' },
        { name: 'Educação empreendedora', course: ' Instituto Ânima' },
        { name: 'Experiências de aprendizagem', course: ' Instituto Ânima' },
        { name: 'Formação do ensino básico', course: ' Instituto Ânima' },
        { name: 'Gamificação em aulas on-line: da teoria a prática ', course: ' Instituto Ânima' },
        { name: 'Metodologias de ensino e aprendizagem na educação empreendedora ', course: ' Instituto Ânima' },
        { name: 'Planeamento reverso para aulas on-line ', course: ' Instituto Ânima' },
        { name: 'Java EE ', course: '– Avançado' },
        { name: 'Microsoft Visual C# ', course: '– Avançado' },
        { name: 'Redes de computadores', course: '– Avançado' },
        { name: 'Desenho técnico ', course: '– Intermédio' },
        { name: 'MicrosoftSony Acid Pro 6 ', course: '– Intermédio' },
        { name: 'Sony Vagas 6,7 e 8 Pro ', course: '– Intermédio' },
        { name: 'Condução ', course: '– Ligeiro profissional' },
        { name: 'Python + Django ', course: '– Avançado' },
        { name: 'Desenvolvimento sustentável FAO ', course: ' – Avançado' },
        { name: 'Dart + Flutter ', course: ' – Avançado' },
        { name: 'Android nativo com Java', course: ' – Avançado' }
      ],
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
