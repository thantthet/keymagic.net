---
title: FAQ
date:  2019-09-23 17:27:59 +06:30
---

<div class="glass-card" style="padding: 1.5rem; margin-bottom: 1.2rem;">
  <strong style="font-size: 1.2em;"><i class="fab fa-apple"></i> Mac OS X</strong>
  <ul style="margin-top: 1em; color: #333; font-size: 1em;">
    <li>
      <strong>I cannot turn off KeyMagic at login window <span style="font-weight: normal;">(Note: <b>Issue solved in macOS Sierra</b>)</span></strong>
      <div style="margin-top: 0.3em;">
        KeyMagic cannot control input method switching at the macOS login window. This is likely a macOS bug.
        <ul style="margin-top: 0.5em;">
          <li><b>Prevention:</b> Try enabling <code>System Preferences &gt; Users &amp; Groups &gt; Login Options &gt; Show Input menu in login window</code>. (May not always work 🤷‍♂️)</li>
          <li><b>Workaround:</b> If stuck at the login screen, perform a hard shutdown or restart your Mac.</li>
        </ul>
      </div>
    </li>
    <li style="margin-top: 1em;">
      <strong>How to install keyboard layouts?</strong>
      <div style="margin-top: 0.3em;">
        Copy the <code>km2</code> file into your <code>~/.keymagic</code> directory. (Create the directory if it does not exist.)
      </div>
    </li>
    <li style="margin-top: 1em;">
      <strong>KeyMagic keyboard menu is empty and KeyMagic won't work</strong>
      <div style="margin-top: 0.3em;">
        This is a known bug. As a temporary fix, kill the KeyMagic process from Activity Monitor and try typing again.
      </div>
    </li>
    <li style="margin-top: 1em;">
      <strong>I don't like notifications when switching keyboards</strong>
      <div style="margin-top: 0.3em;">
        You can disable notifications:
        <ol style="margin-top: 0.3em;">
          <li>Go to <code>System Preferences &gt; Notifications &gt; KeyMagic</code>.</li>
          <li>Set alert style to <b>None</b>.</li>
        </ol>
      </div>
    </li>
  </ul>
</div>

<div class="glass-card" style="padding: 1.5rem;">
  <strong style="font-size: 1.2em;"><i class="fab fa-windows"></i> Windows</strong>
  <ul style="margin-top: 1em; color: #333; font-size: 1em;">
    <li>
      <strong>I get runtime error when starting KeyMagic</strong>
      <div style="margin-top: 0.3em;">
        This may be due to missing dependencies. Please refer to the notes on the <a href="/downloads">downloads page</a>.
      </div>
    </li>
  </ul>
</div>
