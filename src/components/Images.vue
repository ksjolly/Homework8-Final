<template>
  <div id="app">
    <imageHeader></imageHeader>
    <main>
      <div class="row">
        <div class="col-md-12">
          <div class="body-container">
            <h2 class="display-4">OUR INSTRUCTORS</h2>
            <p class="lead">
              GREYWOOD INSTRUCTORS COMBINE CONTENT FLUENCY, PEDAGOGICAL ACUMEN,
              AND STRONG RAPPORT WITH STUDENTS TO CREATE A RESPECTFUL, DYNAMIC,
              AND INVITING LEARNING ENVIRONMENT.
            </p>
            
            <div class="instructor-container">
              <div class="card-instructor">
              <section v-if="cardComponents">
                <cardComponent
                  v-for="cardComponent in cardComponents"
                  v-bind:cardComponent="cardComponent"
                  v-bind:key="cardComponent.name"
                  >
                </cardComponent>
              </section>
              </div>
            </div>
          </div>
      </div>
      </div>
    </main>
    <footerNormal></footerNormal>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>


<script>
import cardComponent from './cardComponent.vue';
import {imageMixin} from '../mixins/imageMixin';
import imageHeader from './imageHeader.vue'
import footerNormal from './footerNormal.vue'

export default {
  name: "Images",
  mixins: [imageMixin],
  created: function() {
    console.log(this.$data)
  },
  components: {
    cardComponent,
    imageHeader,
    footerNormal,
  },
  data() {
    return {
    cardComponents: [
      {
        name: "John Doe",
        title: "Instructor",
        image: [require("../img/headshot.jpg")],
        Teaching: "Spanish, English",
        Experience: "3 years",
        School: "UW",
        Bio:
          "Lorem ipsum dolor sit amet, consectetur...adipiscing elit, sed do eiusmod tempor incididunt utlabore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu",
      },
      {
        name: "Sam  Stone",
        title: "Instructor",
        image: [require("../img/headshot2.jpg")],
        Teaching: "Math, English",
        Experience: "3 years",
        School: "WSU",
        Bio:
          "Lorem ipsum dolor sit amet, consectetur...adipiscing elit, sed do eiusmod tempor incididunt utlabore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu",
      },
      {
        name: "Ron Doe",
        title: "Instructor",
        image: [require("../img/headshot2.jpg")],
        Teaching: "Drama, English",
        Experience: "3 years",
        School: "MIT",
        Bio:
          "Lorem ipsum dolor sit amet, consectetur...adipiscing elit, sed do eiusmod tempor incididunt utlabore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu",
      },
      {
        name: "Mary Doe",
        title: "Instructor",
        image: [require("../img/headshot4.jpg")],
        Teaching: "Science, English",
        Experience: "3 years",
        School: "Harvard",
        Bio:
          "Lorem ipsum dolor sit amet, consectetur...adipiscing elit, sed do eiusmod tempor incididunt utlabore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu",
      },
    ],
      }
  }
};
</script>


<style>
.body-container {
  margin: 1em;
  margin-right: 10em;
  margin-left: 10em;
  text-align: center;
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

.card-instructor {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  transition: 0.3s;
  width: 100%;
  margin: 0em;
  margin-bottom: 0.5em;
}

.main {
  padding: 0;
}


</style>
