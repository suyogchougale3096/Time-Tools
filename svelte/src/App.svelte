<script>
  import { Router, Route, Link, link } from "svelte-navigator";
  import AboutUs from "./AboutUs.svelte";
  import ContactUs from "./ContactUs.svelte";
  import DaysCalculate from "./DaysCalculate.svelte";
  import LeapYear from "./LeapYear.svelte";
  import Cards from "./lib/Cards.svelte";
  import Footer from "./lib/Footer.svelte";
  import HeaderContent from "./lib/HeaderContent.svelte";
  import Logo from "./lib/Logo.svelte";
  import ZodiacSign from "./ZodiacSign.svelte";
</script>


<Router>
  <div class="container-fluid bg-dark">
    <!-- Header Section starts -->
    <div class="row header pt-2 pb-1">
      <div class="col-lg-4 col-sm-12">
        <Logo />
      </div>
      <div class="col-lg-8 col-sm-12 text-light text-center pt-3">
        <HeaderContent />
        <!-- Navbar Starts -->
        <nav>
          <nav class="navbar navbar-expand-lg bg-light mb-2">
              <div class="container-fluid">
                  <!-- <a class="navbar-brand" href="https://www.ieee.org/"></a> -->
                  <button
                      class="navbar-toggler"
                      type="button"
                      data-bs-toggle="collapse"
                      data-bs-target="#navbarNavAltMarkup"
                      aria-controls="navbarNavAltMarkup"
                      aria-expanded="false"
                      aria-label="Toggle navigation"
                  >
                      <span class="navbar-toggler-icon" />
                  </button>
                  <div class="collapse navbar-collapse justify-content-end" id="navbarNavAltMarkup">
                      <div class="navbar-nav">
                          <!-- <Link to="/" class = "nav-link test">Home</Link> -->
                          <a href="/" class="nav-link">Home</a>
                          <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                              Tools
                            </a>
                            <ul class="dropdown-menu">
                              <!-- <Link to = "zodiacsign" class = "nav-link">Zodiac Sign Calculator</Link> -->
                              <a href="zodiacsign" class="nav-link text-center">Zodiac Sign Calculator</a>
                              <a href="leapyear" class="nav-link text-center">Leap Year Check</a>
                              <a href="daycount" class="nav-link text-center">Count Days</a>
                            </ul>
                          </li>
                          <!-- <Link to = "aboutus" class = "nav-link">About Us</Link> -->
                          <a href="aboutus" class = "nav-link">About Us</a>
                          <!-- <Link to = "contactus" class = "nav-link">Contact Us</Link> -->
                          <a href="contactus" class = "nav-link">Contact Us</a>
                      </div>
                  </div>
              </div>
          </nav>
        </nav>
        <!-- Navbar Ends. -->
      </div>
    </div>
    <!-- Header Section End -->
    <Route>
      <div class="container Info">
        <!-- <Cards /> -->
        <div class="text-center text-light">
          <p class = "fs-1">What is Online Time Tool?</p>
          <p>Online time tools is a collection of useful browser-based time and date calculation utilities. All time tools are simple, free and easy to use. There are no ads, popups or other garbage, just time utilities that work right in your browser. And all utilities work exactly the same way and have the same user interface.</p>
          <p>Online Time Tools offers a collection of simple, free, and easy-to-use date and time calculation utilities. There are no intrusive ads, popups, or other garbage, just time utilities that work in your browser. Load a clock time or a calendar date in the input and instantly get the result in the output!</p>
          <p>At Browserling we're building a network of online tools websites. Each site focuses on one and only one tool category. Each tool does one and only one thing.</p>
        </div>
      </div>
    </Route>

    <Route path = "zodiacsign/*ZodiacSign" component = {ZodiacSign}/>

    <Route path = "aboutus/*AboutUsRoute" component = {AboutUs} />

    <Route path = "contactus/*ContactUsRoute" component = {ContactUs} />

    <Route path = "leapyear/*LeapYear" component = {LeapYear} />

    <Route path = "daycount/*DaysCalculate" component = {DaysCalculate} />

    <Footer />
  </div>
</Router>


<style>
  .header {
		background: rgb(62, 44, 62);
		background: radial-gradient(circle, rgba(62, 44, 62, 1) 0%, rgba(138, 82, 42, 1) 0%);
	}
  .Info{
    padding-top: 100px;
    padding-bottom: 100px;
  }

  .nav-link{
    color:black;
  }
  .nav-link:hover{
    color:white;
    background: rgb(62, 44, 62);
		background: radial-gradient(circle, rgba(62, 44, 62, 1) 0%, rgba(138, 82, 42, 1) 0%);
    border-radius: 10px;
  }
  
</style>