---
layout: post
title:  "the making of bloom"
date:   2023-01-24 21:00:00 +0000
tags: audio lunetta
---

if you haven’t listened already, go check out my bands debut single, bloom! in this post, i’m going to be showcasing all the different versions of the song i could find, to show how we went from the original idea to the final master

here’s one of the first recordings i could find of bloom, the classic voice notes demo!

../assets/posts/making-of-bloom/1.wav
<p class="text-muted text-center"><i><small>there's some parts of this that we didn't end up using in the final track, but are still super cool. maybe in a future song we can dig those bits up again</small></i></p>

we then worked on some drums and structure bits to try and work out where we wanted verses and choruses, and recorded some scratch tracks

../../assets/posts/making-of-bloom/2.mp3
<p class="text-muted text-center"><i><small>insanely overcompressed, but i've always found i make demoes sound worse on purpose so i don't get too attached to them</small></i></p>

after that we decided we wanted harmonies, so i made a reallyyyy stupid midi version of the song so i could play around till we had something sounding good

../assets/posts/making-of-bloom/3.wav
<p class="text-muted text-center"><i><small>banger.....</small></i></p>

once we'd recorded the harmonies we thought we were pretty much done with bloom. the plan was to write a couple more songs until we had an EPs worth of material, then we were going to get into the studio to record everything. coming back to the song after some time off, i really felt that it was too "chuggy", 1/8th notes for a whole 3 minute song were really repetitive! i decided that i was going to try something different, so i brought the whole track into ableton, and laid it over some triplet drums i had written, and hit quantise...

../assets/posts/making-of-bloom/4.wav
<p class="text-muted text-center"><i><small>emma, the amazing drummer who plays on the track, wasn't happy recording that intro...</small></i></p>

now it's starting to sound like bloom! this was the version we ended up finalising and bringing into the studio. here's a super rough monitor bounce of the raw drum and guitar tracks

../assets/posts/making-of-bloom/5.wav
<p class="text-muted text-center"><i><small>listening back to this really shows how much shaping recorded drums need to sound release ready</small></i></p>


after recording some extra guitar parts and getting a friend to record bass, it was onto mixing! i mixed the track whilst on holiday in italy, and i really struggled to get something i was happy with, here's a screenshot of the session folder, showing all the different versions i did:

<div class="pt-5">
<img alt="mix session" src="../assets/posts/making-of-bloom/mixsession.jpeg" class="d-block mx-auto rounded" width="60%">
</div>
<p class="text-muted text-center"><i><small>if it wasn't for alex putting her foot down, i'd probably still be mixing the track</small></i></p>

<div class="pt-5">
<img alt="mix session" src="../assets/posts/making-of-bloom/goodview.jpeg" class="d-block mx-auto rounded" width="60%">
</div>
<p class="text-muted text-center"><i><small>remote working is always fun</small></i></p>

here's a javascript thing that lets you compare some mixes of bloom!

<script src="../assets/posts/making-of-bloom/howler.core.js"></script>

<center>
    <button onclick="playAudio()">play</button>

    <button onclick="solo1()">mix 1</button>
    <button onclick="solo2()">mix 2</button>
    <button onclick="solo3()">mix 3</button>
    <button onclick="solo4()">mix 4</button>

    <button onclick="stopAudio()">stop</button>
</center>


<script>
    var audio1 = new Howl({
        src: ["../assets/posts/making-of-bloom/mixes/bloomMix1.wav"]
    });

    var audio2 = new Howl({
        src: ["../assets/posts/making-of-bloom/mixes/bloomMix2.wav"]
    });

    var audio3 = new Howl({
        src: ["../assets/posts/making-of-bloom/mixes/bloomMix3.wav"]
    });

    var audio4 = new Howl({
        src: ["../assets/posts/making-of-bloom/mixes/bloomMix4.wav"]
    });


    function playAudio(){
        audio1.play();
        audio2.play();
        audio3.play();
        audio4.play();

        audio1.mute(false);
        audio2.mute(true);
        audio3.mute(true);
        audio4.mute(true);
    };

    function stopAudio(){
        audio1.stop();
        audio2.stop();
        audio3.stop();
        audio4.stop();

        audio1.mute(false);
        audio2.mute(true);
        audio3.mute(true);
        audio4.mute(true);
    };

    function solo1(){
        audio1.mute(false);
        audio2.mute(true);
        audio3.mute(true);
        audio4.mute(true);
    };

    function solo2(){
        audio1.mute(true);
        audio2.mute(false);
        audio3.mute(true);
        audio4.mute(true);
    };

    function solo3(){
        audio1.mute(true);
        audio2.mute(true);
        audio3.mute(false);
        audio4.mute(true);
    };

    function solo4(){
        audio1.mute(true);
        audio2.mute(true);
        audio3.mute(true);
        audio4.mute(false);
    };
</script>