<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#ff6b9d">

<title>For My Best Friend ❤️</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:"Segoe UI",Arial,sans-serif;
    background:linear-gradient(135deg,#ffe0e9,#ffd1dc,#fbc2eb);
    color:#4a2630;
    overflow-x:hidden;
}

/* =========================
   WELCOME SCREEN
========================= */

#welcome{
    min-height:100vh;
    min-height:100svh;
    display:flex;
    justify-content:center;
    align-items:center;
    padding:20px;
}

.welcome-card{
    width:min(650px,100%);
    padding:50px 30px;
    text-align:center;
    background:rgba(255,255,255,.82);
    backdrop-filter:blur(15px);
    -webkit-backdrop-filter:blur(15px);
    border:1px solid rgba(255,255,255,.7);
    border-radius:35px;
    box-shadow:0 25px 70px rgba(100,30,60,.22);
    animation:cardIn 1.2s ease;
}

.big-heart{
    font-size:75px;
    display:inline-block;
    animation:heartbeat 1.2s infinite;
}

.welcome-card h1{
    margin:18px 0 12px;
    color:#d6336c;
    font-size:clamp(32px,6vw,55px);
}

.welcome-card p{
    font-size:clamp(16px,3vw,20px);
    line-height:1.7;
}

.open-btn,
.secret-btn{
    border:0;
    outline:0;
    margin-top:28px;
    padding:15px 30px;
    border-radius:50px;
    background:linear-gradient(135deg,#d6336c,#e64980);
    color:white;
    font-size:17px;
    font-weight:600;
    cursor:pointer;
    box-shadow:0 10px 25px rgba(214,51,108,.3);
    transition:.3s;
}

.open-btn:hover,
.secret-btn:hover{
    transform:translateY(-3px) scale(1.04);
}

/* =========================
   MAIN WEBSITE
========================= */

#mainWebsite{
    display:none;
}

.container{
    width:min(1100px,100%);
    margin:auto;
    padding:0 20px;
}

section{
    padding:70px 0;
}

.section-title{
    text-align:center;
    color:#c2255c;
    font-size:clamp(28px,5vw,38px);
    margin-bottom:30px;
}

/* Message */

.message-box{
    max-width:850px;
    margin:auto;
    background:rgba(255,255,255,.88);
    padding:35px;
    border-radius:28px;
    box-shadow:0 15px 40px rgba(70,20,40,.12);
    line-height:1.9;
    font-size:18px;
}

.message-box p{
    margin-bottom:18px;
}

.center{
    text-align:center;
}

/* Memories */

.memories{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:20px;
}

.memory-card{
    background:rgba(255,255,255,.9);
    padding:28px 20px;
    border-radius:25px;
    text-align:center;
    box-shadow:0 12px 30px rgba(70,20,40,.1);
    transition:.3s;
}

.memory-card:hover{
    transform:translateY(-8px);
}

.memory-icon{
    font-size:48px;
    margin-bottom:12px;
}

.memory-card h3{
    color:#d6336c;
    margin-bottom:10px;
}

.memory-card p{
    line-height:1.6;
    font-size:15px;
}

/* Final surprise */

.final-section{
    text-align:center;
}

.secret{
    display:none;
    max-width:750px;
    margin:30px auto 0;
    padding:35px 25px;
    background:rgba(255,240,246,.95);
    border-radius:28px;
    box-shadow:0 15px 40px rgba(70,20,40,.12);
    line-height:1.8;
    font-size:19px;
    animation:fadeUp .8s ease;
}

.secret.show{
    display:block;
}

.big-final{
    font-size:35px;
    margin-top:20px;
}

/* Footer */

footer{
    text-align:center;
    padding:35px 20px 45px;
    color:#713445;
}

footer .heart-footer{
    font-size:25px;
}

/* Floating hearts */

.floating-heart{
    position:fixed;
    bottom:-40px;
    z-index:9999;
    pointer-events:none;
    font-size:22px;
    animation:floatUp linear forwards;
}

/* =========================
   ANIMATIONS
========================= */

@keyframes heartbeat{
    0%,100%{
        transform:scale(1);
    }
    50%{
        transform:scale(1.2);
    }
}

@keyframes cardIn{
    from{
        opacity:0;
        transform:translateY(35px) scale(.95);
    }
    to{
        opacity:1;
        transform:translateY(0) scale(1);
    }
}

@keyframes fadeUp{
    from{
        opacity:0;
        transform:translateY(25px);
    }
    to{
        opacity:1;
        transform:translateY(0);
    }
}

@keyframes floatUp{
    0%{
        transform:translateY(0) rotate(0deg);
        opacity:1;
    }

    100%{
        transform:translateY(-110vh) rotate(360deg);
        opacity:0;
    }
}

/* =========================
   TABLET
========================= */

@media(max-width:900px){

    .memories{
        grid-template-columns:repeat(2,1fr);
    }

}

/* =========================
   MOBILE
========================= */

@media(max-width:600px){

    #welcome{
        padding:15px;
    }

    .welcome-card{
        padding:40px 20px;
        border-radius:28px;
    }

    .big-heart{
        font-size:60px;
    }

    .welcome-card h1{
        font-size:34px;
    }

    .welcome-card p{
        font-size:16px;
    }

    .open-btn{
        width:100%;
        max-width:280px;
    }

    .container{
        padding:0 15px;
    }

    section{
        padding:50px 0;
    }

    .message-box{
        padding:25px 20px;
        font-size:16px;
        line-height:1.8;
    }

    .memories{
        grid-template-columns:1fr;
        gap:15px;
    }

    .memory-card{
        padding:25px 20px;
    }

    .secret{
        padding:28px 20px;
        font-size:17px;
    }
}

/* Very small phones */

@media(max-width:380px){

    .welcome-card h1{
        font-size:29px;
    }

    .big-heart{
        font-size:52px;
    }

    .section-title{
        font-size:27px;
    }
}
</style>
</head>


<body>


<!-- =====================================
     FIRST SCREEN
===================================== -->

<div id="welcome">

    <div class="welcome-card">

        <div class="big-heart">❤️</div>

        <h1>Hey Bestie...</h1>

        <p>
            I made something special for you. 🥹
            <br>
            But there's only one way to see it...
        </p>

        <button class="open-btn" onclick="openWebsite()">
            🎁 Open Your Surprise
        </button>

    </div>

</div>



<!-- =====================================
     MAIN WEBSITE
===================================== -->

<div id="mainWebsite">

    <div class="container">


        <!-- MESSAGE -->

        <section>

            <h2 class="section-title">
                A Little Something For You 💌
            </h2>

            <div class="message-box">

                <p>
                    There are many people we meet in life,
                    but only a few become truly special. ❤️
                </p>

                <p>
                    You're not just my best friend.
                    You're someone with whom I can laugh,
                    fight, share stupid things, talk about
                    completely random topics and still never
                    get bored. 😂
                </p>

                <p>
                    Sometimes you're sweet...
                    sometimes irritating...
                    and sometimes completely crazy! 😭😂
                </p>

                <p>
                    But honestly, I wouldn't want you to change.
                    Because that's what makes you...
                    <b>YOU.</b> 🌸
                </p>

                <p class="center">
                    Thank you for being my Best Friend.
                    🫶🏻❤️
                </p>

            </div>

        </section>



        <!-- FRIENDSHIP -->

        <section>

            <h2 class="section-title">
                Our Friendship ✨
            </h2>

            <div class="memories">


                <div class="memory-card">

                    <div class="memory-icon">
                        😂
                    </div>

                    <h3>Crazy Moments</h3>

                    <p>
                        The stupid jokes, random talks
                        and those moments that somehow
                        become our best memories.
                    </p>

                </div>



                <div class="memory-card">

                    <div class="memory-icon">
                        🥹
                    </div>

                    <h3>Always There</h3>

                    <p>
                        Good days or bad days,
                        having a best friend makes
                        everything a little better.
                    </p>

                </div>



                <div class="memory-card">

                    <div class="memory-icon">
                        🤝
                    </div>

                    <h3>Forever Team</h3>

                    <p>
                        Different personalities,
                        different opinions,
                        but somehow the perfect team.
                    </p>

                </div>



                <div class="memory-card">

                    <div class="memory-icon">
                        ❤️
                    </div>

                    <h3>Special Bond</h3>

                    <p>
                        Some friendships don't need
                        a reason. They simply become
                        a beautiful part of life.
                    </p>

                </div>


            </div>

        </section>



        <!-- FINAL SURPRISE -->

        <section class="final-section">

            <h2 class="section-title">
                One Last Surprise 🎁
            </h2>

            <p>
                Think you've seen everything? 😏
            </p>

            <button class="secret-btn" onclick="showSecret()">
                Don't Click This 😜
            </button>


            <div id="secret" class="secret">

                <b>
                    Okay... you clicked it! 😂❤️
                </b>

                <br><br>

                If someday life gets busy,
                people change and everything
                becomes different...

                <br><br>

                I just hope one thing never changes...

                <br><br>

                <b>
                    Our Friendship. 🫶🏻
                </b>

                <br><br>

                No matter where life takes us,
                you'll always have a special place
                in my memories. 🌸

                <div class="big-final">
                    ❤️ 🫶🏻 ♾️
                </div>

            </div>

        </section>


    </div>


    <!-- FOOTER -->

    <footer>

        <div class="heart-footer">
            ❤️
        </div>

        Made with love specially for my Best Friend

        <br>

        <small>
            — From someone who is lucky to have you 🫶🏻
        </small>

    </footer>

</div>



<script>

/* =====================================
   OPEN WEBSITE
===================================== */

function openWebsite(){

    // Hide first screen
    document.getElementById("welcome").style.display = "none";

    // Show complete website
    document.getElementById("mainWebsite").style.display = "block";

    // Start heart animation
    createHearts(25);

    // Go to top
    window.scrollTo({
        top:0,
        behavior:"smooth"
    });
}



/* =====================================
   SECRET MESSAGE
===================================== */

function showSecret(){

    const secret =
        document.getElementById("secret");

    secret.classList.add("show");

    createHearts(40);

    setTimeout(function(){

        secret.scrollIntoView({
            behavior:"smooth",
            block:"center"
        });

    },200);

}



/* =====================================
   FLOATING HEARTS
===================================== */

function createHearts(amount){

    const hearts = [
        "❤️",
        "💖",
        "💕",
        "💗",
        "💓",
        "💞",
        "🌸",
        "✨"
    ];

    for(let i=0;i<amount;i++){

        const heart =
            document.createElement("div");

        heart.className =
            "floating-heart";

        heart.innerHTML =
            hearts[
                Math.floor(
                    Math.random()*hearts.length
                )
            ];

        heart.style.left =
            Math.random()*100 + "vw";

        heart.style.fontSize =
            (18 + Math.random()*18) + "px";

        heart.style.animationDuration =
            (3 + Math.random()*3) + "s";

        document.body.appendChild(heart);


        setTimeout(function(){

            heart.remove();

        },6500);

    }

}

</script>

</body>
</html>}

.card{
    background:rgba(255,255,255,.82);
    backdrop-filter:blur(12px);
    border-radius:30px;
    padding:45px 25px;
    box-shadow:0 20px 50px rgba(100,30,50,.2);
    animation:appear 1.5s ease;
}

.heart{
    font-size:70px;
    animation:beat 1.2s infinite;
}

h1{
    font-size:45px;
    margin:15px 0;
    color:#d6336c;
}

.subtitle{
    font-size:20px;
    line-height:1.6;
}

.btn{
    border:none;
    margin-top:25px;
    padding:14px 28px;
    border-radius:30px;
    background:#d6336c;
    color:white;
    font-size:17px;
    cursor:pointer;
    box-shadow:0 8px 20px rgba(214,51,108,.3);
    transition:.3s;
}

.btn:hover{
    transform:scale(1.08);
}

section{
    padding:60px 0;
}

.section-title{
    text-align:center;
    font-size:32px;
    color:#c2255c;
    margin-bottom:25px;
}

.message{
    background:white;
    border-radius:25px;
    padding:30px;
    line-height:1.8;
    font-size:18px;
    box-shadow:0 10px 30px rgba(0,0,0,.1);
}

.memories{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
}

.memory{
    background:white;
    padding:25px;
    border-radius:22px;
    text-align:center;
    transition:.3s;
}

.memory:hover{
    transform:translateY(-8px);
}

.memory span{
    font-size:45px;
}

.memory h3{
    margin:12px 0;
    color:#d6336c;
}

.surprise{
    text-align:center;
}

.hidden{
    display:none;
}

#secret{
    margin-top:25px;
    background:#fff0f6;
    padding:30px;
    border-radius:25px;
    font-size:20px;
    line-height:1.7;
    animation:appear 1s ease;
}

footer{
    text-align:center;
    padding:30px;
    font-size:16px;
}

.floating-heart{
    position:fixed;
    bottom:-30px;
    font-size:22px;
    animation:floatUp 5s linear forwards;
    pointer-events:none;
}

@keyframes beat{
    50%{transform:scale(1.2);}
}

@keyframes appear{
    from{
        opacity:0;
        transform:translateY(30px);
    }
    to{
        opacity:1;
        transform:translateY(0);
    }
}

@keyframes floatUp{
    to{
        transform:translateY(-110vh) rotate(360deg);
        opacity:0;
    }
}

@media(max-width:600px){
    h1{font-size:34px;}
    .subtitle{font-size:17px;}
    .card{padding:35px 18px;}
}
</style>
</head>

<body>

<div class="container">

    <!-- HERO -->
    <div class="hero">
        <div class="card">

            <div class="heart">❤️</div>

            <h1>Hey Bestie...</h1>

            <p class="subtitle">
                This little website is not for everyone...<br>
                It's specially made for <b>YOU</b> ✨
            </p>

            <button class="btn" onclick="openMessage()">
                Open Your Surprise 🎁
            </button>

        </div>
    </div>


    <!-- MESSAGE -->
    <section id="messageSection">

        <h2 class="section-title">
            A Little Something For You 💌
        </h2>

        <div class="message">

            <p>
                There are many people we meet in life,
                but only a few become truly special. ❤️
            </p>

            <br>

            <p>
                You're not just my best friend.
                You're someone with whom I can laugh,
                fight, share stupid things,
                talk about random topics and still never get bored. 😂
            </p>

            <br>

            <p>
                Sometimes you are sweet...
                sometimes irritating...
                and sometimes completely crazy! 😭😂
            </p>

            <br>

            <p>
                But honestly, I wouldn't want you to change.
                Because that's what makes you...
                <b>YOU.</b> 🌸
            </p>

            <br>

            <p style="text-align:center;font-size:22px;">
                Thank you for being my Best Friend. 🫶🏻❤️
            </p>

        </div>

    </section>


    <!-- MEMORIES -->
    <section>

        <h2 class="section-title">
            Our Friendship ✨
        </h2>

        <div class="memories">

            <div class="memory">
                <span>😂</span>
                <h3>Crazy Moments</h3>
                <p>
                    The stupid jokes and random conversations
                    that somehow become our best memories.
                </p>
            </div>

            <div class="memory">
                <span>🥹</span>
                <h3>Always There</h3>
                <p>
                    Good days or bad days,
                    having a best friend makes everything better.
                </p>
            </div>

            <div class="memory">
                <span>🤝</span>
                <h3>Forever Team</h3>
                <p>
                    Different minds, different personalities,
                    but somehow the perfect friendship.
                </p>
            </div>

            <div class="memory">
                <span>❤️</span>
                <h3>Special Bond</h3>
                <p>
                    Some friendships don't need a reason.
                    They just become a part of your life.
                </p>
            </div>

        </div>

    </section>


    <!-- SURPRISE -->
    <section class="surprise">

        <h2 class="section-title">
            One Last Surprise 🎁
        </h2>

        <button class="btn" onclick="showSecret()">
            Don't Click This 😜
        </button>

        <div id="secret" class="hidden">

            <b>Okay... you clicked it! 😂❤️</b>

            <br><br>

            If someday life gets busy,
            people change and everything becomes different...

            <br><br>

            I just hope one thing never changes...

            <br><br>

            <b>
                Our Friendship. 🫶🏻
            </b>

            <br><br>

            No matter where life takes us,
            you'll always have a special place
            in my memories. 🌸

            <br><br>

            <span style="font-size:30px;">
                ❤️ 🫶🏻 ♾️
            </span>

        </div>

    </section>


    <footer>
        Made with ❤️ specially for my Best Friend
        <br>
        <small>— From someone who is lucky to have you 🫶🏻</small>
    </footer>

</div>


<script>

function openMessage(){

    document.getElementById("messageSection")
    .scrollIntoView({
        behavior:"smooth"
    });

    createHearts();
}

function showSecret(){

    document.getElementById("secret")
    .classList.remove("hidden");

    createHearts();

    setTimeout(createHearts,500);
    setTimeout(createHearts,1000);
}

function createHearts(){

    for(let i=0;i<15;i++){

        let heart=document.createElement("div");

        heart.className="floating-heart";

        heart.innerHTML=[
            "❤️","💖","💕","💗","💓","🌸","✨"
        ][Math.floor(Math.random()*7)];

        heart.style.left=Math.random()*100+"vw";
        heart.style.animationDuration=(3+Math.random()*3)+"s";

        document.body.appendChild(heart);

        setTimeout(()=>{
            heart.remove();
        },6000);
    }
}
 
</script>

</body>
</html>
