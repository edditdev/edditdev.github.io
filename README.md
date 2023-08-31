<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
  body {
    margin: 0;
    padding: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    overflow: hidden;
  }

  video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    animation: shake 0.5s infinite;
  }

  @keyframes shake {
    0%, 100% {
      transform: translateX(0);
    }
    10%, 30%, 50%, 70%, 90% {
      transform: translateX(-10px);
    }
    20%, 40%, 60%, 80% {
      transform: translateX(10px);
    }
  }
</style>
<title>Video z Animacją Shake</title>
</head>
<body>
  <video autoplay loop muted>
    <source src="yalla.mp4" type="video/mp4">
    Przeglądarka nie obsługuje odtwarzania wideo.
  </video>
</body>
</html>
