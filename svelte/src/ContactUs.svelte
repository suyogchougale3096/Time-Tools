<script>
    import { Router, Route, Link } from "svelte-navigator";
    export let ContactUsRoute;
</script>

<div class="container-fluid bg-light Contact">
    <div class="row">
        <div class="col-md-12 text-center Links">
            <h2>Follow Us On</h2>
            <br>
            <i class="fa-brands fa-instagram mb-2"><a href="#" class="ms-1">Instagram</a></i><br />
            <i class="fa-brands fa-facebook mb-2"><a href="#" class="ms-1">Facebook</a></i><br />
            <i class="fa-brands fa-linkedin mb-2"><a href="#" class="ms-1">Linkdin</a></i><br />
            <i class="fa-brands fa-github mb-2"><a href="#" class="ms-1">GitHub</a></i>
        </div>
    </div>
</div>


<style>
    .Contact{
        padding-top: 100px;
        padding-bottom: 100px;
    }
</style>