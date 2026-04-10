var video;

window.addEventListener("load", function() {
	console.log("Good job opening the window");


    video = document.querySelector("#player1");

    video.autoplay = false;
    video.loop = false;
});

document.querySelector("#play").addEventListener("click", function() {
    console.log("Play Video");
    video.play();

    document.querySelector("#volume").innerHTML = (video.volume * 100) + "%";
});

document.querySelector("#pause").addEventListener("click", function() {
    console.log("Pause Video");
    video.pause();
});

document.querySelector("#slower").addEventListener("click", function() {

    video.playbackRate *= 0.90;
    console.log("Speed is " + video.playbackRate);
});

document.querySelector("#faster").addEventListener("click", function() {

    video.playbackRate /= 0.90;
    console.log("Speed is " + video.playbackRate);
});

document.querySelector("#skip").addEventListener("click", function() {

    if (video.currentTime < video.duration - 10) {
        video.currentTime += 10;
    } else {
        video.currentTime = 0;
    }
    console.log("Video current time is " + video.currentTime);
});

document.querySelector("#mute").addEventListener("click", function() {
    if (video.muted) {
        video.muted = false;
        this.innerHTML = "Mute";
    } else {
        video.muted = true;
        this.innerHTML = "Unmute";
    }
});

document.querySelector("#slider").addEventListener("change", function() {

    video.volume = this.value / 100;

    document.querySelector("#volume").innerHTML = this.value + "%";
    console.log("The current volume is " + video.volume);
});

document.querySelector("#vintage").addEventListener("click", function() {
    video.classList.add("oldSchool");
});

document.querySelector("#orig").addEventListener("click", function() {
    video.classList.remove("oldSchool");
});

// document.querySelector("#play").addEventListener("click", function() {
// 	console.log("Play Video");
// });

