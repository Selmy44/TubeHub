# TubeHub
This is a video platform
<!DOCTYPE html>
<html>
<head>
    <title>Video Platform</title>
    <style>
        /* Inline CSS */
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }
        #video-container {
            width: 80%;
            margin: 0 auto;
        }
    </style>
</head>
<body>
    <div id="video-container">
        <h1>Welcome to My Video Platform</h1>
        <video id="myVideo" controls width="640" height="360">
            <source src="example_video.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
    <script>
        // JavaScript for video control
        const video = document.getElementById('myVideo');

        video.addEventListener('play', () => {
            console.log('Video is playing');
        });

        video.addEventListener('pause', () => {
            console.log('Video is paused');
        });

        video.addEventListener('ended', () => {
            console.log('Video has ended');
        });

        video.addEventListener('timeupdate', () => {
            console.log('Current time: ' + video.currentTime);
        });
    </script>
</body>
</html>
