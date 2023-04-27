---
title: Theme Changer
layout: base
---
# Theme Changer
You guys can copy this file and change/improve it here is the [link](https://github.com/AniCricKet/tmv4/blob/master/_pages/theme-changer.md)

<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="../assets/css/fastpages-styles.css">
    <link rel="stylesheet" href="../assets/css/dark-mode1.css" id="theme-link">
</head>
<body>
    <button id="theme-toggle">Toggle Theme</button>
    <script>
        const toggleButton = document.querySelector('#theme-toggle');
        const themeLink = document.querySelector('#theme-link');
        toggleButton.addEventListener('click', () => {
            if (themeLink.getAttribute('href') === '../assets/css/fastpages-styles.css') {
                themeLink.setAttribute('href', '../assets/css/dark-mode1.css');
            } else {
                themeLink.setAttribute('href', '../assets/css/fastpages-styles.css');
            }
        });
    </script>
</body>
</html>

<!--
<html>
<body>
    <?php
        include("../_includes/theme-changer.php")
    ?>
</body>
</html>

<html>
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="../assets/css/fastpages-styles.css" id="default-theme-link">
    <link rel="stylesheet" href="../assets/css/dark-mode1.css" id="dark-theme-link" disabled>
    <link rel="stylesheet" href="../assets/css/other-style.css" id="mort-theme-link" disabled>
</head>
<body>
    <button id="default-theme-toggle">Default Theme</button>
    <button id="dark-theme-toggle">Dark Theme</button>
    <button id="mort-theme-toggle">Mort Theme</button>
    <script>
        const defaultToggleButton = document.querySelector('#default-theme-toggle');
        const darkToggleButton = document.querySelector('#dark-theme-toggle');
        const mortToggleButton = document.querySelector('#mort-theme-toggle');
        const defaultThemeLink = document.querySelector('#default-theme-link');
        const darkThemeLink = document.querySelector('#dark-theme-link');
        const mortThemeLink = document.querySelector('#mort-theme-link');
        defaultToggleButton.addEventListener('click', () => {
            defaultThemeLink.disabled = false;
            darkThemeLink.disabled = true;
            mortThemeLink.disabled = true;
        });
        darkToggleButton.addEventListener('click', () => {
            defaultThemeLink.disabled = true;
            darkThemeLink.disabled = false;
            mortThemeLink.disabled = true;
        });
        mortToggleButton.addEventListener('click', () => {
            defaultThemeLink.disabled = true;
            darkThemeLink.disabled = true;
            mortThemeLink.disabled = false;
        });
    </script>
</body>
</html>
-->