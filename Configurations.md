---


---

<h1 id="configuration">Configuration</h1>
<h2 id="backup">BACKUP</h2>
<p>On Das/Media  (192.168.0.183)<br>
In the Plexbackup folder…<br>
<em><strong>/mnt/Das/Media/plexbackup/config/</strong></em> contains the backup of the config files.<br>
<em><strong>Mounts_Up.sh</strong></em><br>
<em><strong>plexmounts.timer</strong></em><br>
<em><strong>plexmounts.service</strong></em></p>
<h2 id="mounting-nas-drives">Mounting NAS Drives</h2>
<p>After some research the <em><strong>Mounts_Up.sh</strong></em> script (as of 7-Feb-20) is the best so far for mounting the NAS drives. This script can be found and is expected in the <em><strong>/root/Documents/</strong></em> folder.</p>
<p>The script checks to see if each drive is connected, if not then mount!<br>
To allow the script to be executed on boot-up, the CIFS version and password (for root) are included.</p>
<p>Note:-  NAS-Content-45 required CIFS version=1.0.</p>
<h2 id="auto-mount-nas-drives">Auto Mount NAS Drives</h2>
<p>This is achieved using the systemd service to execute the above script on boot.<br>
So in the folder <em><strong>/etc/systemd/system</strong></em> two files to make this work<br>
<strong><strong>plexmounts.timer</strong></strong> and <strong><strong>plexmounts.service</strong></strong></p>
<p>Note if changes to either file the systemd service needs to reload<br>
<em><strong>systemctl daemon-reload</strong></em><br>
and maybe<br>
<em><strong>systemctl restart systemd</strong></em></p>

