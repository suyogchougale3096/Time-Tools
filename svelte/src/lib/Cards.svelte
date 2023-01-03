<script>
  import { Router, Route, Link } from "svelte-navigator";
  import ZodiacSign from "../ZodiacSign.svelte";
</script>

<Router>
  <div class="card" style="width: 18rem;">
    <img src="https://cdn.britannica.com/45/104045-050-116C1F93/Signs-of-the-Zodiac-astrology.jpg" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title">zodiac sign</h5>
      <p class="card-text">In Western astrology, and formerly astronomy, the zodiac is divided into twelve signs, each occupying 30° of celestial longitude and roughly corresponding to the following star constellations.</p>
      <!-- <a href="#" class="btn btn-primary">Go somewhere</a> -->
      <Link to="zodiacsign" class = "btn btn-primary">Go</Link>
    </div>
  </div>
  <Route path = "zodiacsign/*ZodiacSign"component= {ZodiacSign} />
</Router>

<style>
    .card{
   margin-top: 100px;
   margin-bottom: 80px;
 }

 .card:hover{
   font-size: large;
 }
</style>