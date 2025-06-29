
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Redirect by Device</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <script>
    window.onload = function () {
      const ua = navigator.userAgent || navigator.vendor || window.opera;

      const iosLink = "https://cerulean-unicorn-64e5f2.netlify.app";       // ← вставь сюда iOS ссылку
      const androidLink = "https://artemsaas.github.io/06.06.24"; // ← и сюда Android

      if (/iPhone|iPad|iPod/i.test(ua)) {
        window.location.href = iosLink;
      } else if (/Android/i.test(ua)) {
        window.location.href = androidLink;
      }
      // если десктоп — ничего не делаем
    };
  </script>
</head>
<body>
  <p style="text-align: center; margin-top: 40vh; font-family: sans-serif;">
    Redirecting...
  </p>
</body>
</html>
