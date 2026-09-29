<script setup lang="ts">
const currentYear = new Date().getFullYear()
</script>

<template>
  <header class="site-header">
    <h1>I am Patrick (Santiago) Feeney</h1>
    <nav class="social-links" aria-label="Contact links">
      <a href="https://github.com/patrickfeeney03?tab=repositories" target="_blank" rel="noopener noreferrer">GitHub</a>
      <a href="mailto:patrickfeeneytamayo@gmail.com">patrickfeeneytamayo@gmail.com</a>
    </nav>
  </header>

  <main>
    <section>
      <ul>
        <li>Work at Genesys. My team and I recently won the 2026 company Hackathon;</li>
        <li>Got 1st place in my course and in the electronic and electrical eng department and best final year project. Studied Software and Electronic Engineering;</li>
        <li>Work on Angular frontends for WebRTC applications;</li>
        <li>Debug a bunch of race conditions related to event based frontends.</li>
        <li>Work with real time data. WebSockets, WebRTC, Kafka;</li>
        <li>Work with Java Spring microservice backends. WebRTC signaling (how to get people to talk to each other on a call);</li>
        <li>
          Work on our own client-side WebRTC libraries.
          <a href="https://github.com/purecloudlabs/genesys-cloud-streaming-client" target="_blank" rel="noopener noreferrer">streaming-client</a>,
          <a href="https://github.com/MyPureCloud/genesys-cloud-webrtc-sdk" target="_blank" rel="noopener noreferrer">webrtc-sdk</a>;
        </li>
      </ul>

      <hr />

      <ul>
        <li>I like hosting stuff on VPSs. Recently, I decided to ditch Docker and use systemd services and cron jobs.</li>
        <li>Even more recently I decided to give Cloudflare a try to use their fullstack solutions.
        I like how simple but capable it seems. Only 5 dol per month compared to recent VPS prices sounds great.</li>
        <li>I like Herdr/tmux + NVIM + codex/claude/opencode/pi/grok CLI + Lazygit. I like how I can
        have the same setup wherever I go.</li>
        <li>I only use VSCode to view JSON.</li>
        <li>I like lifting weights and riding my bike in the city.</li>
      </ul>
    </section>
  </main>

  <footer class="site-footer">
    <p>{{ currentYear }} Patrick Feeney</p>
  </footer>
</template>
