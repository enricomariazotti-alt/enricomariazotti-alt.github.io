---
title: MS-My Style
layout: default
---

<!-- Bottone per switchare il tema -->
<button id="theme-toggle" style="margin-bottom:1em;">Toggle Theme</button>

<!-- CSS per Light e Dark Mode -->
<style>
:root {
  --bg-color: #ffffff;
  --text-color: #000000;
  --link-color: #1e90ff;
}

body.dark {
  --bg-color: #121212;
  --text-color: #eee;
  --link-color: #80cbc4;
}

body {
  background-color: var(--bg-color);
  color: var(--text-color);
  transition: background-color 0.3s, color 0.3s;
  font-family: sans-serif;
  padding: 2em;
}

a {
  color: var(--link-color);
}
button {
  padding: 0.5em 1em;
  cursor: pointer;
}
</style>

<!-- JavaScript per il toggle -->
<script>
const btn = document.getElementById('theme-toggle');

// Imposta il tema salvato in locale
if(localStorage.getItem('theme') === 'dark') {
  document.body.classList.add('dark');
}

btn.onclick = () => {
  document.body.classList.toggle('dark');
  localStorage.setItem('theme', document.body.classList.contains('dark') ? 'dark' : 'light');
};
</script>

# Hi! I’m Enrico ☕🌍

A coffee-loving, adventure-chasing, sometimes-chaotic soul with a soft spot for cozy moments and big laughs 😄. I’m a proud parent of two amazing kids 👨‍👧‍👦, always curious, and love finding beauty in the unexpected ✨. I enjoy long walks 🚶‍♂️, spontaneous adventures 🏕️, binge-watching shows 📺, and good conversations that can go anywhere 🗣️. Life’s messy, fun, and full of surprises—and I’m here to try to enjoy it all while sharing my journey with you 💫.  

---

**MS (Multiple Sclerosis)**, for me, is not just a challenge—it’s *My Style* 💪. It’s part of how I live, think, and grow 🌱. My journey so far has been full of difficulties, challenges, victories 🏆, and losses 💔, and every day brings its own mix of small wins, reflections 🤔, and moments of joy 😊. I embrace life fully, navigating the ups and downs with my own pace and perspective, turning what some see as limits into a unique way of experiencing the world 🌈.  

---

The idea behind this blog is to share a mix of the journey I’ve made so far 🛤️ and the everyday situations, thoughts 💭, and reflections I experience—a honest intersection of past and present, challenges and small joys 🌟.

👉 Learn more about me on the [About Me](about.md) page.
