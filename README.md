<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>happy 2 years babee</title>

<style>
body {
    margin: 0;
    background-color: #141414;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    color: white;
    overflow-x: hidden;
}

/* Navbar */
.navbar {
    position: fixed;
    width: 100%;
    top: 0;
    background: linear-gradient(to bottom, rgba(0,0,0,0.8), transparent);
    padding: 20px 50px;
    z-index: 1000;
    box-sizing: border-box;
    display: flex;
    align-items: center;
}

.logo {
    color: #E50914;
    font-size: 28px;
    font-weight: bold;
    letter-spacing: 1px;
}

/* Hero section with blurred background effect */
.hero-container {
    position: relative;
    height: 85vh;
    width: 100%;
    overflow: hidden;
}

.hero-bg {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-size: cover;
    background-position: center;
    transition: background-image 1s ease-in-out;
    filter: brightness(0.6);
}

/* Netflix-style vignette/fade */
.hero-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(to top, #141414 5%, transparent 40%),
                linear-gradient(to right, rgba(0,0,0,0.7) 10%, transparent 60%);
}

.hero-content {
    position: absolute;
    bottom: 15%;
    left: 50px;
    z-index: 10;
    max-width: 600px;
}

.hero-content h1 {
    font-size: 55px;
    margin-bottom: 10px;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
    font-weight: bold;
}

.hero-content p {
    font-size: 18px;
    text-shadow: 1px 1px 3px rgba(0,0,0,0.8);
    margin-bottom: 20px;
}

/* Play & Info Buttons */
.btn-container {
    display: flex;
    gap: 10px;
}

.btn {
    padding: 10px 24px;
    border-radius: 4px;
    font-size: 16px;
    font-weight: bold;
    border: none;
    cursor: pointer;
    display: flex;
    align-items: center;
    gap: 8px;
    transition: opacity 0.2s;
}

.btn-play {
    background-color: white;
    color: black;
}

.btn-info {
    background-color: rgba(109, 109, 110, 0.7);
    color: white;
}

.btn:hover {
    opacity: 0.8;
}

/* Rows */
.row {
    padding: 0 50px;
    margin-top: 30px;
    position: relative;
    z-index: 20;
}

.row h2 {
    font-size: 20px;
    margin-bottom: 10px;
    font-weight: 500;
}

.row-posters {
    display: flex;
    gap: 10px;
    overflow-x: auto;
    padding: 15px 0;
}

/* Hide scrollbar */
.row-posters::-webkit-scrollbar {
    display: none;
}

/* Poster Card with Play Overlay & Hover Preview */
.poster-container {
    position: relative;
    min-width: 240px;
    height: 135px;
    border-radius: 4px;
    overflow: hidden;
    cursor: pointer;
    transition: transform 0.4s ease, box-shadow 0.4s ease;
}

.poster-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

/* Play Button Overlay */
.poster-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.4);
    display: flex;
    justify-content: center;
    align-items: center;
    opacity: 0;
    transition: opacity 0.3s ease;
}

.play-icon {
    width: 45px;
    height: 45px;
    background: rgba(255, 255, 255, 0.9);
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    color: black;
    font-size: 18px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.5);
    transform: scale(0.8);
    transition: transform 0.3s ease;
}

/* Hover Zoom & Preview Animation */
.poster-container:hover {
    transform: scale(1.15);
    z-index: 100;
    box-shadow: 0px 10px 20px rgba(0,0,0,0.8);
}

.poster-container:hover .poster-overlay {
    opacity: 1;
}

.poster-container:hover .play-icon {
    transform: scale(1);
}
</style>
</head>

<body>

<!-- Navbar -->
<div class="navbar">
    <div class="logo">NETFLIX</div>
</div>

<!-- Hero Section with Auto Slideshow -->
<div class="hero-container">
    <div class="hero-bg" id="heroBg"></div>
    <div class="hero-overlay"></div>
    <div class="hero-content">
        <h1>happy 2 years babee</h1>
        <p>Our story is my absolute favorite show to binge-watch. Here's to every season, every episode, and a lifetime of renewals. ❤️</p>
        <div class="btn-container">
            <button class="btn btn-play">▶ Play</button>
            <button class="btn btn-info">ⓘ More Info</button>
        </div>
    </div>
</div>

<!-- Row 1 -->
<div class="row">
    <h2>Trending Now</h2>
    <div class="row-posters">
        <div class="poster-container">
            <img src="photo1.jpg" alt="Memory 1">
            <div class="poster-overlay"><div class="play-icon">▶</div></div>
        </div>
        <div class="poster-container">
            <img src="photo2.jpg" alt="Memory 2">
            <div class="poster-overlay"><div class="play-icon">▶</div></div>
        </div>
        <div class="poster-container">
            <img src="photo3.jpg" alt="Memory 3">
            <div class="poster-overlay"><div class="play-icon">▶</div></div>
        </div>
    </div>
</div>

<!-- Row 2 -->
<div class="row">
    <h2>Watch It Again</h2>
    <div class="row-posters">
        <div class="poster-container">
            <img src="photo4.jpg" alt="Memory 4">
            <div class="poster-overlay"><div class="play-icon">▶</div></div>
        </div>
        <div class="poster-container">
            <img src="photo5.jpg" alt="Memory 5">
            <div class="poster-overlay"><div class="play-icon">▶</div></div>
        </div>
        <div class="poster-container">
            <img src="photo6.jpg" alt="Memory 6">
            <div class="poster-overlay"><div class="play-icon">▶</div></div>
        </div>
    </div>
</div>

<!-- Slideshow Logic -->
<script>
    const images = ['photo1.jpg', 'photo2.jpg', 'photo3.jpg', 'photo4.jpg', 'photo5.jpg', 'photo6.jpg'];
    let currentIndex = 0;
    const heroBg = document.getElementById('heroBg');

    function changeBackground() {
        heroBg.style.backgroundImage = `url('${images[currentIndex]}')`;
        currentIndex = (currentIndex + 1) % images.length;
    }

    // Initialize and set interval to change every 3 seconds
    changeBackground();
    setInterval(changeBackground, 3000);
</script>

</body>
</html># my-gallery
