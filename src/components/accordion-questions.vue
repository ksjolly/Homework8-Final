<template>
    <div class="hello">
    <imageHeader></imageHeader>
    <main>
      <div class="row">
        <div class="col-md-12">
          <div class="body-container">
            <div>
              <h2 class="display-4">Mission Statement</h2>
              <p class="lead">
                To provide an optimal personalized education for each student.
                Following are some questions and answers for your students. Anim
                pariatur cliche reprehenderit, enim eiusmod high life accusamus
                terry richardson ad squid.Anim pariatur cliche reprehenderit,
                enim eiusmod high life accusamus terry richardson ad squid.Anim
                pariatur cliche reprehenderit, enim eiusmod high life accusamus
                terry richardson ad squid. Anim pariatur cliche reprehenderit,
                enim eiusmod high life accusamus terry richardson ad squid.
              </p>
              <p class="lead">
                Anim pariatur cliche reprehenderit, enim eiusmod high life
                accusamus terry richardson ad squid.Anim pariatur cliche
                reprehenderit, enim eiusmod high life accusamus terry richardson
                ad squid.
              </p>
              
                <div class="accordion" role="tablist">
                 <div v-for="object,index in objects" :key="index">
                  <b-card no-body class="mb-1">
                    <b-card-header header-tag="header" class="p-1" role="tab">
                      <b-button block v-b-toggle="'accordion-' + index" variant="info"
                        >{{object.question}}</b-button
                      >
                    </b-card-header>
                    <b-collapse
                      :id="'accordion-' + index"
                      visible
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body>
                        <b-card-text>{{ object.text }}</b-card-text>
                      </b-card-body>
                    </b-collapse>
                  </b-card>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </main>
  <footerNormal></footerNormal>
  </div>
</template>

<script>
import router from "../router";
import imageHeader from './imageHeader.vue'
import footerNormal from './footerNormal.vue'

export default {
  name: "Page2",
   data() {
    return {
      objects: [
        {
          question: 'How do I know Greywood is right for me?',
          text: `
          Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
          richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor
          brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon
          tempor, sunt aliqua put a bird on it squid single-origin coffee nulla
          assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore
          wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher
          vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
          synth nesciunt you probably haven't heard of them accusamus labore VHS.
        `
        },
        {
          question: 'Why do students choose Greywood over other schools? ',
          text: `
          Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
          richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor
          brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon
          tempor, sunt aliqua put a bird on it squid single-origin coffee nulla
          assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore
          wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher
          vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
          synth nesciunt you probably haven't heard of them accusamus labore VHS.
        `
        },
        {
          question: 'Who are the instructors here?',
          text: `
          Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
          richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor
          brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon
          tempor, sunt aliqua put a bird on it squid single-origin coffee nulla
          assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore
          wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher
          vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
          synth nesciunt you probably haven't heard of them accusamus labore VHS.
        `
        },
        {
          question: 'When are students back in class post covid?',
          text: `
          Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
          richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor
          brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon
          tempor, sunt aliqua put a bird on it squid single-origin coffee nulla
          assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore
          wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher
          vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
          synth nesciunt you probably haven't heard of them accusamus labore VHS.
        `
        },]
    }
    },
    components: {
        imageHeader,
        footerNormal
    }
}
</script>

<style scoped>
.body-container {
  margin: 1em;
  margin-right: 10em;
  margin-left: 10em;
  text-align: center;
}
.top-menu {
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.router-link {
  padding: 1em;
}
.button {
  background-color: #4caf50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 0.5em;
  cursor: pointer;
}

@media only screen and (min-width: 0px) {
  .body-container {
    margin: 0em;
    margin-right: 0em;
    margin-left: 0em;
    text-align: center;
  }
}

@media only screen and (min-width: 768px) {
  .body-container {
    margin: 1em;
    margin-right: 15em;
    margin-left: 15em;
    text-align: center;
  }
}

@media only screen and (min-width: 2000px) {
  .body-container {
    margin: 1em;
    margin-right: 40em;
    margin-left: 40em;
    text-align: center;
  }
}

.jumbotron {
  background-image: url("../img/blossoms.jpg");
  background-size: cover;
  display: flex;
  flex-direction: column;
  text-align: center;
}

.header-container {
  margin: 1em;
}
.body-container {
  margin: 1em;
  margin-right: 10em;
  margin-left: 10em;
  text-align: center;
}
.top-menu {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.footer-container {
  padding: 5em;
  background-color: rgb(59, 42, 133);
}
</style>