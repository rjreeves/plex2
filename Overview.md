---


---

<h1 id="overview">Overview</h1>
<h2 id="introduction">Introduction</h2>
<p>The motive of this task was the “old” plexserver running on an old Mini Mac, which has reached its end of line with recent MAC OS X updates/upgrades. The easy option would be to purchase or accquire a “newer” Mac.  Another option was to use my database server (move the data base to another machine or the cloud) which was an intel NUC with suitable hardware for running Plex Media Server.</p>
<h2 id="challenges">Challenges</h2>
<h3 id="initially">Initially</h3>
<ul>
<li>Install Linix on the NUC with PlexMedia Server.  Easy to install</li>
<li>Configure this server full connection with the NAS farm.  	Not so easy as the mount  		functionality could not automatically detect SAMBA versions. More on this later.</li>
<li>Working with “Transmission”. The objective here was to use more web interfaces, thus reduce dependancy on screen sharing/remote destop . So far - mixed success.</li>
<li>Automate the Plex Server to be as much Unattended as possible.
<ul>
<li>Automated updates of OS and Plex software - DONE</li>
<li>Auto “MOUNTS” of the NAS farm on startup. - DONE</li>
<li>Monitor and MOUNT NAS farm nodes on a periodical cycle (say 10 Minutes) WIP.</li>
</ul>
</li>
</ul>
<h3 id="currently">Currently</h3>
<ul>
<li>
<p>Introduced <strong>fcopy</strong> (dev in python). Two main features are to copy TV shows (and movies) from Transmission to the NAS farm. The functionality is still early days. The second main feature to is translate the file names (as downloaded vis the torrent client) to comply with Plex name protocol.</p>
</li>
<li>
<p>Installed COCKPIT admin tool on the server.  Well used.</p>
</li>
<li>
<p>Installed FileBrowser (web based) to use for file copying. MIxed success!</p>
</li>
<li>
<p>Believing the NUC would work with the HDMI on the TV set could be use to provide GUI access. Not really required so when OS is updated (currently Fedora 30) would consider server version and not workstation.</p>
</li>
</ul>
<h3 id="future">Future</h3>
<p>Improve the fcopy to auto copy to the correct NAS and subfolder.</p>

