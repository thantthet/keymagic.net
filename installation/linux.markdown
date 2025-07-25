---
title: Installation on Linux
date: 2019-03-01 17:23:00 +06:30
---

<div class="glass-card">
  <h3>Ubuntu PPA</h3>
  <p>
    For Ubuntu and compatible Debian-based distributions, you can install KeyMagic using the kokoye2007 PPA:
  </p>
  <pre><code>sudo add-apt-repository -y ppa:kokoye2007/ppa
sudo apt-get update
sudo apt-get install ibus-keymagic
</code></pre>
</div>

<div class="glass-card">
  <h3>Manual Installation</h3>
  <p>
    Download the appropriate package for your Linux distribution from <a href="https://sourceforge.net/projects/ubuntumm/files/ibus-keymagic/">SourceForge</a>.
  </p>

  <h4>Debian Base</h4>
  <p>
    For Debian-based systems (Ubuntu, Mint, Kali, etc.), download the DEB file <a href="https://sourceforge.net/projects/ubuntumm/files/ibus-keymagic/DEBIAN_Ubuntu_Mint_Pinguy_Kali_Deb/">here</a>.
  </p>
  <pre><code>sudo dpkg -i ibus-keymagic*.deb
</code></pre>

  <h4>Redhat Base</h4>
  <p>
    For Redhat-based systems (Fedora, CentOS, etc.), download the appropriate RPM file:
    <ul>
      <li><a href="https://sourceforge.net/projects/ubuntumm/files/ibus-keymagic/Redhat_Fedora_CentOS_RPM/Fedora/">Fedora fc-x86-64</a></li>
      <li><a href="https://sourceforge.net/projects/ubuntumm/files/ibus-keymagic/Redhat_Fedora_CentOS_RPM/CentOS/">CentOS el7 x86-64</a></li>
    </ul>
  </p>
  <pre><code>sudo rpm -ivh ibus-keymagic*.rpm
</code></pre>

  <h4>Arch Linux</h4>
  <p>
    For Arch Linux, download the package <a href="https://sourceforge.net/projects/ubuntumm/files/ibus-keymagic/ARCH_Linux/ibus-keymagic-x86_64.pkg.tar.xz/download">ibus-keymagic-x86_64.pkg.tar.xz</a> and install with:
  </p>
  <pre><code>sudo pacman -U ibus-keymagic*.xz
</code></pre>
</div>

<div class="glass-card">
  <h3>Keyboard</h3>
  <ul>
    <li>Download KeyMagic keyboard layouts from <a href="https://github.com/thantthet/keymagic-keyboards">GitHub</a> (e.g., KhmerNiDA, Myanmar, Mon, Shan, Malay).</li>
  </ul>
  <p>To add and configure a keyboard layout:</p>
  <pre><code>mkdir -p ~/.keymagic
cp *.km2 ~/.keymagic
ibus-daemon -rdx
ibus-setup &
ibus-daemon -rdx
</code></pre>
  <pre><code># If using GNOME:
gnome-control-center keyboard || gnome-control-center region
</code></pre>
  <blockquote>
    KeyMagic will appear under the English group.<br>
    Add your additional keyboard layout as needed.
  </blockquote>
  <p>Logout and log back in to apply changes.</p>
  <p>Thanks to <a href="https://ubuntu-mm.net">Ko Ko Ye</a> and Ubuntu-MM for providing packages.</p>
</div>
