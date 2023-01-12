<script>
    import { Router, Route, Link } from "svelte-navigator";
    export let DaysCalculate;

    let date1 = 'Not Selected';
    let date2 = 'Not Selected';
    
    let Odate1;
    let Odate2;

    let str1;
    let str2;

    let arr;
    let arr2;

    let temp = -1;
    
    let time_difference; 

    let days_difference = -1; 

    let DayCalculatorFunction = () => {
        arr = date1.split('-');
        arr2 = date2.split('-');
        str1 = arr[1] + "/" + arr[2] + "/" + arr[0];
        str2 = arr2[1] + "/" + arr2[2] + "/" + arr2[0];
        Odate1 = new Date(str1);
        Odate2 = new Date(str2);
        time_difference = Odate2.getTime() - Odate1.getTime();
        days_difference = time_difference / (1000 * 60 * 60 * 24); 
        console.log(Odate2)
    }
</script>

<div class="container DayCalculator text-center">
    <p class = 'fs-2 text-light'>Count Number of days.</p>
    <div class="row">
        <div class="col mt-4">
            <label for="datePicker" class="form-label text-light">Enter the date : (From)</label>
            <input type="date" bind:value={date1} required>
            <br>
            <!-- <label for="datePicker" class="form-label text-light" id = "result">Check Your input date here & then press Submit: {date1}</label> -->
        </div>
        <div class="col mt-4">
            <label for="datePicker" class="form-label text-light">Enter the date : (To)</label>
            <input type="date" bind:value={date2} required>
            <br>
            <!-- <label for="datePicker" class="form-label text-light" id = "result">Check Your input date here & then press Submit: {date2}</label> -->
        </div>
    </div>
    <button class = "btn btn-primary" on:click={DayCalculatorFunction}>Check</button>

    {#if Odate2 != 'Invalid Date' && Odate1 != 'Invalid Date'}
        {#if days_difference == -1}
            <p class="form-label text-warning mt-4" id = "result">Select valid dates.</p>
        {:else}
            {#if days_difference >= 0}
                <p class="form-label text-warning mt-4" id = "result">The number of days : {days_difference}</p>
            {:else}
                <p class="form-label text-warning mt-4" id = "result">You entered wrong dates.</p>
            {/if}
        {/if}
    {:else}
        <p class="form-label text-warning mt-4" id = "result">Select valid dates.</p>
    {/if}
</div>


<style>
    .DayCalculator {
		margin-top: 100px;
		margin-bottom: 100px;
		padding-top: 50px;
		padding-bottom: 50px;
		background: rgb(62, 44, 62);
		background: radial-gradient(circle, rgba(62, 44, 62, 1) 0%, rgba(54, 50, 48, 1) 0%);
		border-radius: 10px;
		box-shadow: 18px -11px 19px 18px rgba(0, 0, 0, 0.75);
		-webkit-box-shadow: 18px -11px 19px 18px rgba(0, 0, 0, 0.75);
		-moz-box-shadow: 18px -11px 19px 18px rgba(0, 0, 0, 0.75);
	}
    .DayCalculator:hover {
		font-size: large;
	}
</style>