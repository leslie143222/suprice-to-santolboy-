<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>For My Santolboy 💜</title>

<style>

*{
    box-sizing:border-box;
}

body{
    margin:0;
    font-family:"Comic Sans MS","Trebuchet MS",sans-serif;
    background:
        radial-gradient(circle at 10% 10%, #ffffff 0 2%, transparent 3%),
        linear-gradient(135deg,#eadcff,#d9c3f5,#f5eaff);
    color:#49345f;
    overflow-x:hidden;
}


/* FLOATING HEARTS */

.heart{
    position:fixed;
    bottom:-30px;
    color:#a875d1;
    font-size:25px;
    animation:float 8s linear infinite;
    opacity:.6;
    z-index:0;
}

@keyframes float{

    0%{
        transform:translateY(0) rotate(0deg);
        opacity:0;
    }

    20%{
        opacity:.7;
    }

    100%{
        transform:translateY(-110vh) rotate(360deg);
        opacity:0;
    }

}


/* PAPER */

.paper{
    position:relative;
    z-index:2;
    width:92%;
    max-width:850px;
    margin:35px auto;
    background:#fffaff;
    padding:35px 25px;
    border-radius:8px;
    box-shadow:0 12px 35px rgba(81,45,104,.25);
    transform:rotate(-.3deg);
}

.paper:before{
    content:"";
    position:absolute;
    top:-10px;
    left:20px;
    width:90px;
    height:25px;
    background:#cda9eb;
    opacity:.7;
    transform:rotate(-5deg);
}


/* INTRO */

#intro{
    min-height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    padding:20px;
}

.intro-content{
    text-align:center;
}

.small{
    font-size:15px;
    letter-spacing:3px;
    color:#9364b6;
}

h1{
    font-size:clamp(42px,10vw,75px);
    margin:10px 0;
    color:#7846a0;
}

.subtitle{
    font-size:18px;
    line-height:1.7;
}

button{
    border:none;
    background:#9b68c4;
    color:white;
    padding:13px 25px;
    border-radius:25px;
    font-size:16px;
    cursor:pointer;
    margin:8px;
    box-shadow:0 5px 12px rgba(102,62,130,.25);
    transition:.25s;
}

button:hover{
    transform:translateY(-3px) rotate(-1deg);
    background:#824fa9;
}

.sticker{
    display:inline-block;
    background:#f0dfff;
    padding:10px 18px;
    border-radius:50%;
    transform:rotate(-8deg);
    margin:10px;
}


/* MAIN */

#main{
    display:none;
}


/* NAVIGATION */

.nav{
    display:flex;
    gap:8px;
    flex-wrap:wrap;
    justify-content:center;
    margin-bottom:25px;
}

.nav button{
    font-size:13px;
    padding:9px 15px;
    background:#d5b7ec;
    color:#56386d;
}

.section{
    margin:45px 0;
}

.title{
    text-align:center;
    font-size:32px;
    color:#75459b;
}

.center{
    text-align:center;
}


/* PHOTO SCRAPBOOK */

.photos{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:18px;
    margin-top:25px;
}

.photo{
    background:white;
    padding:10px;
    box-shadow:0 7px 15px rgba(70,40,90,.18);
    transform:rotate(-2deg);
}

.photo:nth-child(even){
    transform:rotate(3deg);
}

.photo img{
    width:100%;
    height:230px;
    object-fit:cover;
    display:block;
    background:#e8d5f5;
}

.caption{
    text-align:center;
    padding:8px 3px;
    font-size:13px;
}


/* QUESTION CARDS */

.question{
    background:#f7efff;
    border:2px dashed #c397df;
    padding:25px;
    border-radius:15px;
    margin:25px 0;
    text-align:center;
}

.question h3{
    font-size:24px;
}

.result{
    display:none;
    background:#fff;
    padding:20px;
    border-radius:15px;
    margin-top:15px;
    animation:pop .4s ease;
}

@keyframes pop{

    from{
        transform:scale(.7);
        opacity:0;
    }

    to{
        transform:scale(1);
        opacity:1;
    }

}


/* ================================= */
/* QUESTION #1 YES / NO GAME */
/* ================================= */

#beautyQuestion{
    overflow:hidden;
}

.button-area{
    position:relative;
    width:100%;
    min-height:220px;

    display:flex;
    justify-content:center;
    align-items:center;

    gap:15px;

    overflow:hidden;
}


/* YES */

#yesBeauty{
    transition:all .4s ease;
    z-index:5;

    background:#9b68c4;
    color:white;

    border:none;
    border-radius:30px;

    padding:13px 25px;

    font-size:16px;
    font-weight:bold;

    cursor:pointer;

    box-shadow:0 5px 12px rgba(102,62,130,.25);
}


/* NO */

#noBeauty{
    transition:all .25s ease;
    z-index:10;

    background:#eeeeee;
    color:#555;

    border:none;
    border-radius:30px;

    padding:13px 25px;

    font-size:16px;
    font-weight:bold;

    cursor:pointer;

    box-shadow:0 5px 12px rgba(80,80,80,.15);
}


/* MESSAGE */

.no-message{
    background:#fff;

    border:2px solid #d6b3eb;

    padding:15px;

    border-radius:15px;

    margin-top:15px;

    animation:popMessage .4s ease;

    color:#70488a;

    font-size:15px;

    line-height:1.6;
}

@keyframes popMessage{

    0%{
        transform:scale(.5) rotate(-3deg);
        opacity:0;
    }

    70%{
        transform:scale(1.05) rotate(2deg);
    }

    100%{
        transform:scale(1) rotate(0);
        opacity:1;
    }

}


/* LETTER */

.letter{
    background:#fffdfd;
    padding:30px;
    line-height:1.9;
    font-size:16px;
    border-left:6px solid #c59be4;
    box-shadow:0 5px 15px rgba(70,40,90,.12);
}

.signature{
    text-align:right;
    font-style:italic;
}


/* ENVELOPES */

.surprises{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:15px;
}

.envelope{
    background:#ead6fa;
    padding:25px 10px;
    text-align:center;
    border-radius:15px;
    cursor:pointer;
    transition:.3s;
}

.envelope:hover{
    transform:scale(1.04) rotate(1deg);
}

.envelope-icon{
    font-size:45px;
}


/* SECRET */

.secret{
    text-align:center;
    background:#f0e1fb;
    padding:30px;
    border-radius:20px;
}

#secretText{
    display:none;
    margin-top:20px;
    padding:20px;
    background:white;
    border-radius:15px;
    line-height:1.8;
}


/* FOOTER */

footer{
    text-align:center;
    padding:40px 10px;
    color:#80618f;
    font-size:14px;
}


/* MOBILE */

@media(max-width:600px){

    .paper{
        width:95%;
        padding:25px 15px;
    }

    .photos{
        grid-template-columns:1fr 1fr;
    }

    .photo img{
        height:170px;
    }

    .surprises{
        grid-template-columns:1fr 1fr;
    }

    .title{
        font-size:27px;
    }

    .button-area{
        min-height:240px;
    }

}

</style>

</head>


<body>


<!-- FLOATING HEARTS -->

<div class="heart" style="left:5%;animation-delay:0s;">♡</div>

<div class="heart" style="left:20%;animation-delay:2s;">💜</div>

<div class="heart" style="left:40%;animation-delay:4s;">♡</div>

<div class="heart" style="left:65%;animation-delay:1s;">💜</div>

<div class="heart" style="left:85%;animation-delay:3s;">♡</div>



<!-- INTRO -->

<div id="intro">

<div class="paper intro-content">

<div class="sticker">
💜
</div>

<div class="small">
A VERY IMPORTANT WEBSITE
</div>

<h1>
Hi, Santolboy! 😭💜
</h1>

<p class="subtitle">
I made something for you...<br>
and unfortunately, you cannot escape it.
</p>

<p>
You have been warned. 😌
</p>

<button onclick="startWebsite()">
CLICK ME 👀
</button>

<br>

<small>
made with love, kalokohan, and questionable decisions
</small>

</div>

</div>



<!-- MAIN -->

<div id="main">

<div class="paper">



<!-- NAVIGATION -->

<div class="nav">

<button onclick="goTo('questions')">
💭 Questions
</button>

<button onclick="goTo('memories')">
📸 Memories
</button>

<button onclick="goTo('letter')">
💌 My Message
</button>

<button onclick="goTo('surprises')">
🎁 Surprises
</button>

<button onclick="goTo('secret')">
🤫 Secret
</button>

</div>



<!-- QUESTIONS -->

<div class="section" id="questions">

<h2 class="title">
💭 VERY IMPORTANT QUESTIONS
</h2>

<p class="center">
Answer honestly. I'm watching. 👁️👄👁️
</p>



<!-- QUESTION 1 -->

<div class="question" id="beautyQuestion">

<h3>
Question #1
</h3>

<p>
Maganda ba ako? 😌
</p>


<div class="button-area">

<button id="yesBeauty" onclick="yesBeauty()">
YES po baby
</button>

<button id="noBeauty" onclick="noBeauty()">
No
</button>

</div>


<div class="result" id="beautyResult"></div>

</div>



<!-- QUESTION 2 -->

<div class="question">

<h3>
Question #2
</h3>

<p>
Sino ang mas cute? 🤨
</p>

<button onclick="cuteMe()">
ikaw
</button>

<button onclick="cuteMe()">
you
</button>

<div class="result" id="cuteResult"></div>

</div>



<!-- QUESTION 3 -->

<div class="question">

<h3>
Question #3
</h3>

<p>
Gusto mo pa ba ako kahit makulit ako? 😭
</p>

<button onclick="loveAnswer()">
YES NAMAN
</button>

<button onclick="loveAnswer()">
OO NAMAN
</button>

<div class="result" id="loveResult"></div>

</div>



<!-- QUESTION 4 -->

<div class="question">

<h3>
LAST QUESTION
</h3>

<p>
do u miss me? 😌
</p>

<button onclick="luckyAnswer()">
yess halos mabaliw nanga ako kakaisip sayo
</button>

<button onclick="luckyAnswer()">
opo subra
</button>

<div class="result" id="luckyResult"></div>

</div>

</div>



<!-- MEMORIES -->

<div class="section" id="memories">

<h2 class="title">
📸 Our Little Memories
</h2>

<p class="center">
Some random pictures of my favorite Santolboy. 😭
</p>

<div class="photos">


<div class="photo">

<img src="PHOTO1.jpg">

<div class="caption">
santolboy being santolboy
</div>

</div>



<div class="photo">

<img src="PHOTO2.jpg">

<div class="caption">
bakit ang cute mo dito 😭
</div>

</div>



<div class="photo">

<img src="PHOTO3.jpg">

<div class="caption">
proof na may childhood ka pala
</div>

</div>



<div class="photo">

<img src="PHOTO4.jpg">

<div class="caption">
eto yung gusto kitang hampasin ng kaldero 😭
</div>

</div>



<div class="photo">

<img src="PHOTO5.jpg">

<div class="caption">
okay fine... cute ka.
</div>

</div>


</div>

</div>



<!-- LETTER -->

<div class="section" id="letter">

<h2 class="title">
💌 A Little Message
</h2>


<div class="letter">


<p>
Dear <b>Kiven Carl Mejos</b>, aka <b>my Santolboy</b> 😭💜
</p>


<p>
Gusto ko lang sabihin na thank you kasi dumating ka sa life ko.
Hindi ko naman in-expect na may taong kayang magpasaya sa akin
sa simpleng paraan lang.
</p>


<p>
Alam kong minsan inaaway kita, pinipikon kita, at kung minsan
parang hobby ko na talaga mang-inis. 😭
Pero kahit gano'n, thank you kasi lagi ka pa rin nandyan.
</p>


<p>
Thank you kasi lagi mo akong pinapasaya, kinakausap,
at pinaparamdam na hindi ako mag-isa.
Kahit minsan ang kulit ko at parang gusto mo na akong
itapon sa basurahan, salamat kasi hindi mo pa rin ako tinatapon. 😭
</p>


<p>
Diba ang sweet ko? May pa-website website pa ako.
Daig ko pa yung lalaki, feeling ko ako pa yung nanliligaw sa'yo. 😭
Like... <b>ang kapal mo naman, sineswerte ka.</b>
</p>


<p>
Sarap mong hampasin gamit ang kaldero...
<br>
<b>kidding lang. 😭 HAHAHA</b>
</p>


<p>
Pero seryoso, I'm really thankful that you came into my life.
I appreciate you more than I sometimes know how to say.
</p>


<p>
Thank you for always being there for me.
Thank you for making me smile.
And thank you for being one of the people who made my days
a little happier.
</p>


<p>
I hope you know that you are appreciated,
even on the days when I annoy you for absolutely no reason. 😭
</p>


<p>
<b>
I'm really glad you came into my life, Santolboy. 💜
</b>
</p>


<p class="signature">
</p>


</div>

</div>



<!-- SURPRISES -->

<div class="section" id="surprises">

<h2 class="title">
🎁 Little Surprises
</h2>

<p class="center">
Click each one. Yes, ALL of them. 👀
</p>


<div class="surprises">


<div class="envelope" onclick="surprise1()">

<div class="envelope-icon">
💌
</div>

Open me

</div>



<div class="envelope" onclick="surprise2()">

<div class="envelope-icon">
💜
</div>

Open this

</div>



<div class="envelope" onclick="surprise3()">

<div class="envelope-icon">
😭
</div>

Last one

</div>



<div class="envelope" onclick="surprise4()">

<div class="envelope-icon">
👀
</div>

Definitely click

</div>


</div>

</div>



<!-- SECRET -->

<div class="section" id="secret">

<div class="secret">

<h2 class="title">
🤫 SECRET MESSAGE
</h2>

<p>
You really thought we're done?
</p>

<button onclick="showSecret()">
REVEAL IT 👀
</button>


<div id="secretText">

<p>
Okay fine... 😭
</p>

<p>
If you made it this far,
I hope you know how much effort I put into this.
</p>

<p>
I know it's just a website,
but I wanted to make something that you could
keep and look at whenever you want.
</p>

<p>
So here's your final reminder:
</p>

<h2>
I'm really glad you're here. 💜
</h2>

<p>
And yes, you're still my Santolboy.
No refunds. 😭
</p>

</div>

</div>

</div>



<!-- FOOTER -->

<footer>

Made with 💜, kalokohan, and a little bit of pagiging OA.

<br><br>

<b>
for my Santolboy, Kiven Carl Mejos ♡
</b>

</footer>


</div>

</div>



<script>


/* ========================= */
/* START WEBSITE */
/* ========================= */

function startWebsite(){

    document.getElementById("intro").style.display="none";

    document.getElementById("main").style.display="block";

    window.scrollTo(0,0);

}



/* ========================= */
/* NAVIGATION */
/* ========================= */

function goTo(id){

    document.getElementById(id).scrollIntoView({

        behavior:"smooth"

    });

}



/* ================================= */
/* QUESTION #1 YES / NO GAME */
/* ================================= */

let noClicks = 0;


const noMessages = [

    "di yan dapat yung pipindotin mo",

    "over naman sa no. 😭",

    "click na ng yes o sasapakin kita? 😭",

    "isa 🙄 wala kang kiss sakin",

    "ang kulit naman pinipilit talaga na No noh.",

    "Fine. Since you won't choose YES... I'll make YES bigger. 😌💅",

    "na love at first kanga sakin eh tas di pa maganda🙄",

    "Last warning... aminin mona kasi na maganda ako."

];



function noBeauty(){

    noClicks++;


    const yesButton =
        document.getElementById("yesBeauty");

    const noButton =
        document.getElementById("noBeauty");

    const result =
        document.getElementById("beautyResult");

    const area =
        document.querySelector(".button-area");



    /* YES GETS BIGGER */

    let newSize =
        16 + (noClicks * 4);

    let newPadding =
        13 + (noClicks * 3);


    yesButton.style.fontSize =
        newSize + "px";


    yesButton.style.padding =
        newPadding + "px " +
        (newPadding * 1.7) + "px";



    /* MOVE NO RANDOMLY */

    const maxX =
        Math.max(
            5,
            area.clientWidth -
            noButton.offsetWidth -
            10
        );


    const maxY =
        Math.max(
            5,
            area.clientHeight -
            noButton.offsetHeight -
            10
        );


    const randomX =
        5 + Math.random() *
        Math.max(1,maxX - 5);


    const randomY =
        5 + Math.random() *
        Math.max(1,maxY - 5);


    noButton.style.position =
        "absolute";


    noButton.style.left =
        randomX + "px";


    noButton.style.top =
        randomY + "px";



    /* SHOW DIFFERENT MESSAGE */

    let messageIndex =
        Math.min(
            noClicks - 1,
            noMessages.length - 1
        );


    result.style.display =
        "block";


    result.innerHTML =

        "<div class='no-message'>" +

        noMessages[messageIndex] +

        "</div>";



    /* AFTER 5 NO CLICKS */

    if(noClicks >= 5){

        yesButton.innerHTML =
            "YES na nganii";

    }


    /* AFTER 8 NO CLICKS */

    if(noClicks >= 8){

        yesButton.innerHTML =
            "Mag yes kana kasi no choice kanaman";

    }

}



/* YES BUTTON */

function yesBeauty(){

    const result =
        document.getElementById("beautyResult");


    result.style.display =
        "block";


    result.innerHTML =

        "<div class='no-message'>" +

        "ALAM KO NAMAN TALAGA. <br><br>" +

        "I just wanted to hear you say it. HAHAHA.<br><br>" +

        "See? inamin mona talaga<br><br>" +

        "<b>Good boy. You chose correctly. ♡</b>" +

        "</div>";

}



/* ========================= */
/* QUESTION #2 */
/* ========================= */

function cuteMe(){

    document.getElementById("cuteResult").style.display="block";

    document.getElementById("cuteResult").innerHTML=

    "CORRECT ANSWER! 💜<br><br>" +

    "Sa true kasi mas cute talaga ako kisa sayo, " +

    "muka ka kasing unggoy pero love parin kita. 😭";

}



/* ========================= */
/* QUESTION #3 */
/* ========================= */

function loveAnswer(){

    document.getElementById("loveResult").style.display="block";

    document.getElementById("loveResult").innerHTML=

    "Yeheyy dahil dyan may kiss ka sakin 😭💜<br><br>" +

    "Ang harot mo talaga HAHAHA but thanks.";

}



/* ========================= */
/* QUESTION #4 */
/* ========================= */

function luckyAnswer(){

    document.getElementById("luckyResult").style.display="block";

    document.getElementById("luckyResult").innerHTML=

    "VERY GOOD. <br><br>" +

    "I really know talaga na miss mo 'ko " +

    "kasi inlove na inlove ka sakin eh. ";

}



/* ========================= */
/* SURPRISES */
/* ========================= */

function surprise1(){

    alert(
        "💌 Thank you for coming into my life, kiven. "
    );

}


function surprise2(){

    alert(
        "💜 Reminder: someone out there is always cheering for you and it's me."
    );

}


function surprise3(){

    alert(
        "😭 Congratulations! You found another random message."
    );

}


function surprise4(){

    alert(
        "👀 You really clicked everything HAHAHA. I knew you would."
    );

}



/* ========================= */
/* SECRET */
/* ========================= */

function showSecret(){

    document.getElementById("secretText").style.display="block";

}

</script>


</body>
</html>
