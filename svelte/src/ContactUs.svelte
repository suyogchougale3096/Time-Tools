<script>
    import { Router, Route, Link } from "svelte-navigator";
    export let ContactUsRoute;
</script>

<div class="container-fluid bg-light Contact">
    <div class="row">
        <div class="col-md-12 text-center Links">
            <p class = "fs-2">Contact Us On</p>
            <br>
            <!-- <a href="#" class="ms-1"><i class="fa-brands fa-instagram mb-2"></i></a><br /> -->
            <div class="Links">
                <i class="fa-brands fa-instagram mb-2"></i><a href="#" class="ms-1 link-dark">Instagram</a><br />
                <i class="fa-brands fa-facebook mb-2"></i><a href="#" class="ms-1 link-dark">Facebook</a><br />
                <i class="fa-brands fa-linkedin mb-2"></i><a href="#" class="ms-1 link-dark">Linkdin</a><br />
            </div>
        </div>
    </div>
</div>


<style>
    .Contact{
        padding-top: 100px;
        padding-bottom: 100px;
    }
    .Links{
        font-size: 21px;;
    }
    .link-dark{
        text-decoration: none;
    }
    .link-dark:hover{
        font-size: 25px;
    }
    .fa-instagram{
        color:rgb(236, 9, 175);
    }
    .fa-facebook{
        color: blue;
    }
    .fa-linkedin{
        color:blue
    }
</style>