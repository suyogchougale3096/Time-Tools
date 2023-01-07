<script>
    import { Router, Route, Link } from "svelte-navigator";
    export let LeapYear;

    let dob = 'NULL';
    let year,month,day;
    let arr;
    let temp = -1;


    const displayBtn1 = () =>{
        year = dob;
        console.log(typeof(year))
        if(Number(year) % 4 == 0){
            temp = 1;
        }
        else{
            temp = 0;
        }
    }
</script>

<div class="container LeapContents">
    <div class="row">
        <div class="col">
            <div class="info text-light text-center">
            <p class = "fs-2">About Leap Year Checking.</p>
                This is a quick online utility for testing if the given year is a leap year. Just as a reminder, 
            a leap year has 366 days, which is one more day than a common year. This extra day is added to the month of 
            February and it falls on February 29th. There's a simple mathematical formula for calculating if the given year is a 
            leap year. Leap years are those years that are divisible by 4 but not divisible by 100, as well as years that are divisible by 
            100 and 400 simultaneously. Our algorithm checks each input year using this formula and outputs the year's status. For example, 
            if you enter the value "2025" as input, the program will display "2025 is not a leap year.", and for the value "2028", the status 
            will be "2028 is a leap year.".
            </div>
        </div>
    </div>
</div>

<div class="container YearCheck text-center">
    <p class = 'fs-2 text-light'>Detect Leap Year or Not</p>
    <label for="datePicker" class="form-label text-light">Enter the date : </label>
    <input type="number" min = "1900" max = "2099"bind:value={dob} placeholder = 'Year'required>
    <!-- <p class = 'fs-5 text-light'>{dob}</p> -->
    <br>
    <button class="btn btn-primary mt-3" on:click={displayBtn1}>Check</button>
    {#if year != 'NULL'}
        {#if temp != -1}
            {#if temp == 0}
                <p class="text-light text-center fs-5 mt-4">It is not leap year</p>
            {:else}
                <p class="text-light text-center fs-5 mt-4">It is leap year</p>
            {/if}
        {/if}
    {/if}
</div>


<style>
    .LeapContents{
        margin-top: 50px;
        margin-bottom: 50px;
    }
    .YearCheck {
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
    .YearCheck:hover {
		font-size: large;
	}
</style>