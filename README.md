<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For My Best Friend ❤️</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family: "Segoe UI", sans-serif;
}

body{
    min-height:100vh;
    background:linear-gradient(135deg,#ffdde1,#ee9ca7);
    color:#4a2630;
    overflow-x:hidden;
}

.container{
    max-width:900px;
    margin:auto;
    padding:25px;
}

.hero{
    min-height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
}

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
