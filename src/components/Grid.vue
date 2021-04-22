<template>
  <div id="app">
        <imageHeader></imageHeader>
           <main>
        <div class="row">
            <div class="col-md-12">
                <div class="body-container">
                    <h2 class="display-4">OUR BOOKS</h2>
                    <p class="lead">OUR INSTRUCTORS HAVE BEEN HARD AT WORK FINDING BOOKS FOR OUR STUDENTS! WE HOPE YOU
                        ENJOY THIS MONTHS' BOOKS. </p>
                    <div class="container">
                        <div class="row">
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../img/book1.jpg" alt="Card image cap">
                                    <div class="card-body">
                                        <h4 class="card-title">The Wee Free Men</h4>
                                        <p class="card-text">
                                            Some information about this book
                                        </p>
                                        <a href="#!" class="btn btn-primary">Buy Me!</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../img/book2.jpg" alt="Card image cap">
                                    <div class="card-body">
                                        <h4 class="card-title">The Wee Free Men</h4>
                                        <p class="card-text">
                                            Some information about this book
                                        </p>
                                        <a href="#!" class="btn btn-primary">Buy Me!</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../img/book3.jpg" alt="Card image cap">
                                    <div class="card-body">
                                        <h4 class="card-title">The Wee Free Men</h4>
                                        <p class="card-text">
                                            Some information about this book
                                        </p>
                                        <a href="#!" class="btn btn-primary">Buy Me!</a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="container">
                        <div class="row">
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../img/book4.jpg" alt="Card image cap">
                                    <div class="card-body">
                                        <h4 class="card-title">The Wee Free Men</h4>
                                        <p class="card-text">
                                            Some information about this book
                                        </p>
                                        <a href="#!" class="btn btn-primary">Buy Me!</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../img/book1.jpg" alt="Card image cap">
                                    <div class="card-body">
                                        <h4 class="card-title">The Wee Free Men</h4>
                                        <p class="card-text">
                                            Some information about this book
                                        </p>
                                        <a href="#!" class="btn btn-primary">Buy Me!</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col">
                                <div class="card">
                                    <img class="card-img-top" src="../img/book2.jpg" alt="Card image cap">
                                    <div class="card-body">
                                        <h4 class="card-title">The Wee Free Men</h4>
                                        <p class="card-text">
                                            Some information about this book
                                        </p>
                                        <a href="#!" class="btn btn-primary">Buy Me!</a>
                                    </div>
                                </div>
                            </div>
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
import imageHeader from './imageHeader.vue'
import footerNormal from './footerNormal.vue'

export default {
  name: 'Grid',
  components: {
      imageHeader,
      footerNormal,
  }
}
</script>

<style>
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
    background-color: #4CAF50; /* Green */
    border: none;
    color: white;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: .5em;
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




</style>
