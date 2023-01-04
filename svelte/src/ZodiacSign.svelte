<script>
    import { Router, Route, Link } from "svelte-navigator";
    export let ZodiacSign;

    let dob = '';
    let year,month,day;
    let arr;
    
    const displaybtn = () => {
        arr = dob.split("-");
        year = arr[0];
        month = arr[1];
        day = arr[2];
    };

    console.log(typeof(dob));
</script>

<!-- Start of carousel -->
<div class="container carousel">
    <div class="text-center text-light fs-2">
        <b>Zodiac Signs</b>
    </div>
    <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="false">
        <div class="carousel-indicators">
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="0"
                class="active"
                aria-current="true"
                aria-label="Slide 1"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="1"
                aria-label="Slide 2"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="2"
                aria-label="Slide 3"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="3"
                aria-label="Slide 4"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="4"
                aria-label="Slide 5"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="5"
                aria-label="Slide 6"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="6"
                aria-label="Slide 7"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="7"
                aria-label="Slide 8"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="8"
                aria-label="Slide 9"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="9"
                aria-label="Slide 10"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="10"
                aria-label="Slide 11"
            />
            <button
                type="button"
                data-bs-target="#carouselExampleCaptions"
                data-bs-slide-to="11"
                aria-label="Slide 12"
            />
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img
                    src="https://images.hindustantimes.com/img/2022/03/30/1600x900/Leo_(1)_1648665755515_1648665782738.jpg"
                    class="d-block rounded mx-auto d-block w-75"
                    alt="These is Leo Image"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Leo</h5>
                    <p>
                        Leo is represented by the lion, and these spirited fire signs are the kings and
                        queens of the celestial jungle.
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://www.uniguide.com/wp-content/uploads/2022/04/sagittarius-ultimate-guide-sq.jpeg"
                    class="d-block rounded mx-auto d-block w-50"
                    alt="..."
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Sagittarius</h5>
                    <p>
                        The ninth astrological sign, which is associated with the constellation <br
                        />Sagittarius and spans 240–270th degrees of the zodiac.
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://blog.prepscholar.com/hubfs/zodiac-sign-4374412_1920.jpg"
                    class="d-block rounded mx-auto d-block w-50"
                    alt="Scorpio"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Scorpio</h5>
                    <p>
                        Scorpio (♏︎) is the eighth astrological sign in the zodiac, originating from the<br
                        />
                        constellation of Scorpius.
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://static.toiimg.com/thumb/msid-88128028,width-400,resizemode-4/88128028.jpg"
                    class="d-block rounded mx-auto d-block w-50"
                    alt="Scorpio"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Taurus</h5>
                    <p>
                        Taurus (♉︎) is the second astrological sign in the modern zodiac. <br />It spans
                        from 30° to 60° of the zodiac.
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://static.toiimg.com/photo/msid-88563906/88563906.jpg"
                    class="d-block rounded mx-auto d-block w-50"
                    alt="Virgo"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Virgo</h5>
                    <p>
                        Virgo (♍︎) (Greek: Παρθένος, Parthenos) is the sixth astrological sign in the
                        zodiac.
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://c8.alamy.com/zooms/9/eaf76d71a3be489dbfb8e60b36a575cc/w6j40p.jpg"
                    class="d-block rounded mx-auto d-block w-50"
                    alt="Libra"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Libra</h5>
                    <p>
                        Libra (♎︎) is the seventh astrological sign in the zodiac. It spans 180°–210°
                        celestial longitude.
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://cdn.images.express.co.uk/img/dynamic/130/590x/Gemini-zodiac-star-sign-dates-Symbols-and-meaning-for-Gemini-1307042.jpg?"
                    class="d-block rounded mx-auto d-block w-75"
                    alt="Gemini"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Gemini</h5>
                    <p>
                        Gemini (♊︎) (/ˈdʒɛmɪnaɪ/ JEM-in-eye, Latin for "twins") is the third astrological
                        sign in the zodiac.
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://static.toiimg.com/photo/msid-84376765/84376765.jpg"
                    class="d-block rounded mx-auto d-block w-75"
                    alt="Pisces"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Pisces</h5>
                    <p>
                        Pisces (♓︎) (/ˈpaɪsiːz/; Ancient Greek: Ἰχθύες Ikhthyes) is the twelfth and final
                        astrological sign in the zodiac. It is a negative, mutable sign.
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://cdn.pixabay.com/photo/2019/07/31/06/03/zodiac-sign-4374404__340.jpg"
                    class="d-block rounded mx-auto d-block w-75"
                    alt="Aries"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Aries</h5>
                    <p>
                        Aries (♈︎) (Greek: Κριός Kriós, Latin for "ram") is the first astrological sign in
                        the zodiac
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://www.pinkvilla.com/files/styles/amp_metadata_content_image/public/cancer_1_17.jpg"
                    class="d-block rounded mx-auto d-block w-50"
                    alt="Cancer"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Cancer</h5>
                    <p>
                        Cancer (♋︎) ("crab" in Latin) is the fourth astrological sign in the zodiac,<br />
                        originating from the constellation of Cancer. It spans from 90° to 120° celestial longitude.
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://cdn.images.express.co.uk/img/dynamic/130/590x/Capricorn-zodiac-star-sign-dates-Symbols-and-meaning-for-Capricorn-1303903.jpg"
                    class="d-block rounded mx-auto d-block w-50"
                    alt="Capricorn"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Capricorn</h5>
                    <p>
                        Capricorn (♑︎) is the tenth astrological sign in the zodiac out of twelve total <br
                        />
                        zodiac signs, originating from the constellation of Capricornus, the goat.
                    </p>
                </div>
            </div>
            <div class="carousel-item">
                <img
                    src="https://askastrology.com/wp-content/uploads/2020/07/aquarius_astrology_sign.jpg"
                    class="d-block rounded mx-auto d-block w-50"
                    alt="Aquarius"
                />
                <div class="carousel-caption d-none d-md-block">
                    <h5>Aquarius</h5>
                    <p>
                        Aquarius is the eleventh astrological sign in the zodiac, originating from the <br
                        />
                        constellation Aquarius. Under the tropical zodiac, the Sun is in the Aquarius sign between
                        <br />
                        about January 20 and about February 18.
                    </p>
                </div>
            </div>
        </div>
        <button
            class="carousel-control-prev"
            type="button"
            data-bs-target="#carouselExampleCaptions"
            data-bs-slide="prev"
        >
            <span class="carousel-control-prev-icon" aria-hidden="true" />
            <span class="visually-hidden">Previous</span>
        </button>
        <button
            class="carousel-control-next"
            type="button"
            data-bs-target="#carouselExampleCaptions"
            data-bs-slide="next"
        >
            <span class="carousel-control-next-icon" aria-hidden="true" />
            <span class="visually-hidden">Next</span>
        </button>
    </div>
</div>
<!-- End of carousel -->

<!-- Start the section of Enter the birth date. -->
<div class="container DatePicker">
    <div class="text-center">
        <p class="text-light fs-1 text-center">Zodiac Sign Calculator</p>
        <label for="datePicker" class="form-label text-light">Enter the birth date : </label>
        <input type="date" bind:value={dob} required>
        <br />
        <button class="btn btn-primary mt-3" on:click={displaybtn}>Submit</button>
    </div>
</div>
<!-- End the section of Enter the birth date. -->

<!-- Print the result -->
<div class="container ResultDatePicker">
    <div class="text-center">
        <p class="text-light fs-1 text-center">Zodiac Sign Result</p>
        <label for="datePicker" class="form-label text-light" id = "result">{dob}</label>
    </div>
</div>

<style>
    .carousel {
		margin-top: 50px;
	}
    .DatePicker {
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
	.ResultDatePicker {
		padding-top: 50px;
		margin-bottom: 100px;
		background: rgb(62, 44, 62);
		background: radial-gradient(circle, rgba(62, 44, 62, 1) 0%, rgba(54, 50, 48, 1) 0%);
		border-radius: 10px;
		box-shadow: 18px -11px 19px 18px rgba(0, 0, 0, 0.75);
		-webkit-box-shadow: 18px -11px 19px 18px rgba(0, 0, 0, 0.75);
		-moz-box-shadow: 18px -11px 19px 18px rgba(0, 0, 0, 0.75);
	}
	.DatePicker:hover {
		font-size: large;
	}

</style>