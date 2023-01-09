<script>
    import { Router, Route, Link } from "svelte-navigator";
    export let ZodiacSign;

    let dob = 'Not Selected';
    let year,month,day;
    let arr;
    let horiscope = 'Date is not selected yet.';
    let temp = 0;
    
    const displaybtn = () => {
        arr = dob.split("-");
        year = Number(arr[0]);
        month = Number(arr[1]);
        day = Number(arr[2]);
        console.log(year);
        console.log(typeof(month));
        console.log(day);

        if(year == 0){
            temp = 1;
        }

        // Check the Zodiac Signs
        if(month == 3){
            if(day >= 21 && day <= 31){
                horiscope = 'Aries';
            }
        }
        if(month == 4){
            if(day >= 1 && day <= 19){
                horiscope = 'Aries';
            }
        }

        if(month == 4){
            if(day >= 20 && day <= 30){
                horiscope = 'Taurus';
            }
        }
        if(month == 5){
            if(day >= 1 && day <= 20){
                horiscope = 'Taurus';
            }
        }
        if(month == 5){
            if(day >= 21 && day <= 31){
                horiscope = 'Gemini';
            }
        }
        if(month == 6){
            if(day >= 1 && day <= 21){
                horiscope = 'Gemini';
            }
        }
        if(month == 6){
            if(day >= 22 && day <= 31){
                horiscope = 'Cancer';
            }
        }
        if(month == 7){
            if(day >= 1 && day <= 22){
                horiscope = 'Cancer';
            }
        }
        if(month == 7){
            if(day >= 23 && day <= 31){
                horiscope = 'Leo';
            }
        }
        if(month == 8){
            if(day >= 1 && day <= 22){
                horiscope = 'Leo';
            }
        }
        if(month == 8){
            if(day >= 23 && day <= 31){
                horiscope = 'Virgo';
            }
        }
        if(month == 9){
            if(day >= 1 && day <= 22){
                horiscope = 'Virgo';
            }
        }
        if(month == 9){
            if(day >= 23 && day <= 30){
                horiscope = 'Libra';
            }
        }
        if(month == 10){
            if(day >= 1 && day <= 23){
                horiscope = 'Libra';
            }
        }
        if(month == 10){
            if(day >= 24 && day <= 31){
                horiscope = 'Scorpius';
            }
        }
        if(month == 11){
            if(day >= 1 && day <= 21){
                horiscope = 'Scorpius';
            }
        }
        if(month == 11){
            if(day >= 22 && day <= 30){
                horiscope = 'Sagittarius';
            }
        }
        if(month == 12){
            if(day >= 1 && day <= 21){
                horiscope = 'Sagittarius';
            }
        }
        if(month == 12){
            if(day >= 22 && day <= 31){
                horiscope = 'Capricornus';
            }
        }
        if(month == 1){
            if(day >= 1 && day <= 19){
                horiscope = 'Capricornus';
            }
        }
        if(month == 1){
            if(day >= 20 && day <= 31){
                horiscope = 'Aquarius';
            }
        }
        if(month == 2){
            if(day >= 1 && day <= 18){
                horiscope = 'Aquarius';
            }
        }
        if(month == 2){
            if(day >= 19 && day <= 29){
                horiscope = 'Pisces';
            }
        }
        if(month == 3){
            if(day >= 1 && day <= 20){
                horiscope = 'Pisces';
            }
        }
    }
   
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
<div class="container DatePicker ">
    <div class="text-center">
        <p class="text-light fs-1 text-center">Zodiac Sign Calculator</p>
        <br>
        <label for="datePicker" class="form-label text-light">Enter the birth date : </label>
        <input type="date" bind:value={dob} required>
        <br>
        <!-- <label for="datePicker" class="form-label text-light" id = "result">Check Your input date here & then press Submit: {dob}</label> -->
        <!-- <br /> -->
        <button class="btn btn-primary mt-3" on:click={displaybtn}>Check</button>
    </div>
</div>
<!-- End the section of Enter the birth date. -->

<!-- Print the result -->
<div class="container ResultDatePicker">
    <div class="text-center">
        <p class="text-light fs-1 text-center">Zodiac Sign Result</p>
        <p class="text-light fs-2 text-center" bind:textContent={horiscope} contenteditable="false">{horiscope}</p>
        {#if temp == 0}
        {#if horiscope == 'Aries'}
        <p class="text-light fs-4 text-center pb-2">In astrology, Aries is the first sign of the zodiac, considered as governing the period from about March 21 to about April 19. Its representation as a ram is identified with the Egyptian god Amon and, in Greek mythology, with the ram with the golden fleece, on the back of which Phrixus, the son of King Athamas, safely fled Thessaly to Colchis, where he sacrificed the ram to Zeus, who placed it in the heavens as the constellation. The ram’s golden fleece was recovered by Jason, leader of the Argonauts.</p>
    {:else if horiscope == 'Taurus'}
    <p class="text-light fs-4 text-center pb-2">Taurus, (Latin: “Bull”) in astronomy, zodiacal constellation lying in the northern sky between Aries and Gemini, at about 4 hours 20 minutes right ascension and 16° north declination. The constellation’s brightest star, Aldebaran (Arabic for “the follower”; also called Alpha Tauri), is the 14th brightest star in the sky, with a magnitude of 0.85. The constellation also contains the Crab Nebula (M1) and the Pleiades and Hyades star clusters.
        In astrology, Taurus is the second sign of the zodiac, considered as governing that portion of the year from about April 20 to about May 20. Its representation as a bull is related to the Greek myth of Zeus, who assumed the form of a bull to abduct Europa.
    </p>
    {:else if horiscope == 'Gemini'}
    <p class="text-light fs-4 text-center pb-2">
        Gemini, (Latin: “Twins”) in astronomy, zodiacal constellation lying in the northern sky between Cancer and Taurus, at about 7 hours right ascension and 22° north declination. Its brightest stars are Castor and Pollux (Alpha and Beta Geminorum); Pollux is the brighter of the two, with a magnitude of 1.15, and is the 17th brightest star in the sky. The summer solstice, the northernmost point reached by the Sun in its annual apparent journey among the stars, lies in Gemini. This constellation also contains the isolated pulsar Geminga.
        In astrology, Gemini is the third sign of the zodiac, considered as governing the period from about May 21 to about June 21. It is represented by a set of twins (or in Egyptian astrology by a pair of goats and in Arabian astrology by a pair of peacocks). In addition to their identification as Castor and Pollux, the twins have also been related to other celebrated pairs, such as the younger and older Horus or Romulus and Remus.
    </p>
    {:else if horiscope == 'Cancer'}
    <p class="text-light fs-4 text-center">
        Cancer, (Latin: “Crab”) in astronomy, zodiacal constellation lying in the northern sky between Leo and Gemini, at about 8 hours 25 minutes right ascension and 20° north declination. It contains the well-known star cluster called Praesepe, or the Beehive. Its brighest star, Al Tarf (Arabic for “the end” [of one of the crab’s legs]), also called Beta Cancri, is quite dim, with a magnitude of 3.6.
        In astrology, Cancer is the fourth sign of the zodiac, considered as governing the period from about June 22 to about July 22. Its representation as a crab (or lobster or crayfish) is related to the crab in Greek mythology that pinched Heracles while he was fighting the Lernaean hydra. Crushed by Heracles, the crab was rewarded by Heracles’ enemy, Hera, by being placed in the heavens.
    </p>
    {:else if horiscope == 'Leo'}
    <p class="text-light fs-4 text-center">
        Leo, (Latin: “Lion”) in astronomy, zodiacal constellation lying in the northern sky between Cancer and Virgo, at about 10 hours 30 minutes right ascension and 15° north declination. Regulus (Latin for “little king”; also called Alpha Leonis), the brightest star, is of magnitude 1.35. The November meteor shower called the Leonids has its radiant, or point of apparent origin, in Leo. Many of the stars in Leo form an asterism called the Sickle.
This Month in Astrology: Leo
This Month in Astrology: LeoSee all videos for this article
In astrology, Leo is the fifth sign of the zodiac, considered as governing the period from about July 23 to about August 22. Its representation as a lion is usually linked with the Nemean lion slain by Heracles (Hercules).
    </p>
    {:else if horiscope == 'Virgo'}
        <p class="text-light fs-4 text-center">
Virgo, (Latin: “Virgin”) in astronomy, zodiacal constellation lying in the southern sky between Leo and Libra, at about 13 hours right ascension and 2° south declination. The constellation’s brightest star, Spica (Latin for “head of grain,” also called Alpha Virginis), is the 15th brightest star in the sky, with a magnitude of 1.04. Virgo contains the nearest large cluster of galaxies, the Virgo cluster, in which is located the giant elliptical galaxy Virgo A and PSR 1257+12, the pulsar around which the first extrasolar planets were discovered in 1992.

This Month in Astrology: Virgo
This Month in Astrology: VirgoSee all videos for this article
In astrology, Virgo is the sixth sign of the zodiac, considered as governing the period from about August 23 to about September 22. It is represented as a young maiden carrying a sheaf of wheat. She is variously identified as a fertility goddess (the Babylonian and Assyrian Ishtar, among others) or the harvest maiden (the Greek Persephone and others).
        </p>

    {:else if horiscope == 'Libra'}
        <p class="text-light fs-4 text-center">
            Libra, (Latin: “Balance”) in astronomy, zodiacal constellation in the southern sky lying between Scorpius and Virgo, at about 15 hours 30 minutes right ascension and 15° south declination. Its stars are faint; the brightest star, Zubeneschamali (Arabic for “northern claw,” as it was earlier regarded as part of Scorpius; also called Beta Librae), has a magnitude of 2.6.
In astrology, Libra is the seventh sign of the zodiac, considered as governing the period from about September 22 to about October 23. It is represented by a woman (sometimes identified with Astraea, the Roman goddess of justice), holding a balance scale or by the balance alone.
        </p>
    {:else if horiscope == 'Scorpius'}
    <p class="text-light fs-4 text-center">
        Scorpius, (Latin: “Scorpion”) also called Scorpio, in astronomy, zodiacal constellation lying in the southern sky between Libra and Sagittarius, at about 16 hours 30 minutes right ascension and 30° south declination. Its brightest star, Antares (Alpha Scorpii), the 15th brightest star in the sky, has a magnitude of 1.1. Its name comes from the Greek for “rival of Ares” (i.e., rival of the planet Mars) and was probably given because of the star’s red colour and brightness. The brightest X-ray source in the sky, Scorpius X-1, is found in this constellation.
In astrology, Scorpius (or Scorpio) is the eighth sign of the zodiac, considered as governing the period from about October 24 to about November 21. Its representation as a scorpion is related to the Greek legend of the scorpion that stung Orion to death (said to be why Orion sets as Scorpius rises in the sky). Another Greek myth relates that a scorpion caused the horses of the Sun to bolt when they were being driven for a day by the inexperienced youth Phaeton.
    </p>
    {:else if horiscope == 'Sagittarius'}
        <p class="text-light fs-4 text-center">
            Sagittarius, (Latin: “Archer”) in astronomy, zodiacal constellation in the southern sky lying between Capricornus and Scorpius, at about 19 hours right ascension and 25° south declination. The centre of the Milky Way Galaxy lies in the radio source Sagittarius A*. Near the western border of Sagittarius is the winter solstice, the southernmost point reached by the Sun in its apparent annual journey among the stars. This constellation also contains the Lagoon and Trifid nebulas. The brightest star is Kaus Australis (from the Arabic for “bow” and the Latin for “southern,” respectively; it is also called Epsilon Sagittarii), with a magnitude of 1.9. Many of the stars are arranged in the prominent asterism called the Teapot.
            In astrology, Sagittarius is the ninth sign of the zodiac, considered as governing the period from about November 22 to about December 21. It is represented either by a centaur shooting a bow and arrow or by an arrow drawn across a bow. The identification of Sagittarius as a mounted archer was made by the Babylonians as early as the 11th century BCE.
        </p>
        {:else if horiscope == 'Capricornus'}
        <p class="text-light fs-4 text-center">
            Capricorn, (from Latin: “Goat-Horned”) also called Capricornus and the Goat, in astrology, the 10th sign of the zodiac, considered as governing the period from about December 22 to about January 19. One explanation of the fishtail with which the goat is often represented is found in the Greek myth of Pan, who, to avoid the monster Typhon, jumped into the water just as he was changing into animal shape. The half above water assumed the shape of a goat while the lower half, the tail, assumed the shape of a fish.
In astronomy, Capricornus is a zodiacal constellation lying in the southern sky between Aquarius and Sagittarius, at about 21 hours right ascension and 20° south declination. Its stars are faint; Deneb Algedi (Arabic for “kid’s tail”) is the brightest star, with a magnitude of 2.9. Capricornus usually refers to the constellation, and Capricorn usually refers to the astrological sign.
        </p>
        {:else if horiscope == 'Aquarius'}
        <p class="text-light fs-4 text-center">
            Aquarius, (Latin: “Water Bearer”) in astronomy, zodiacal constellation lying in the southern sky between Capricornus and Pisces, at about 22 hours right ascension and 10° south declination. It lacks striking features, the brightest star, Sadalmelik (Arabic for “the lucky stars of the king”), being of magnitude 3.0.
In astrology, Aquarius is the 11th sign of the zodiac, considered as governing the period from about January 20 to about February 18. Its representation as a man pouring a stream of water out of a jug came about, it has been suggested, because in ancient times the rising of Aquarius coincided in the Middle East with a period of floods and rain.
        </p>
        {:else if horiscope == 'Pisces'}
        <p class="text-light fs-4 text-center">
            Pisces, (Latin: “Fishes”) in astronomy, zodiacal constellation in the northern sky between Aries and Aquarius, at about 1 hour right ascension and 15° north declination. The vernal equinox, the point where the Sun’s annual apparent path takes it north of the celestial equator and from which celestial longitude and right ascension are measured, lies in Pisces. The constellation contains only faint stars without any striking grouping; the brightest star, Eta Piscium, has a magnitude of 3.6.
In astrology, Pisces is the 12th sign of the zodiac, considered as governing the period from about February 19 to about March 20. Its representation as two fish tied together is usually related to the Greek myth of Aphrodite and Eros, who jumped into a river to escape the monster Typhon and changed into fish, or, alternatively, the two fish that carried them to safety.
        </p>
    {/if}
    {:else}
    <p class="text-light fs-4 text-center">Please select an date.</p>
        {/if}

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
        padding-bottom: 50px;
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