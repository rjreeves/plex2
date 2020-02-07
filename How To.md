---


---

<h1 id="how-to">How To</h1>
<h3 id="manually-mount-nas-drives">Manually Mount NAS Drives</h3>
<p>using cockpit login as plex\Plexmedia.1<br>
go to the Terminal<br>
enter <em>sudo -i</em> using the above password<br>
enter <em>cd /root/Documents</em><br>
enter <em>./Mounts_Up.sh</em><br>
read the output to ensure each mount is ultimately successful.<br>
You can expect the MOUNTS to be available upon script completion.</p>
<h3 id="restart-the-plexmediaserver">Restart the plexmediaserver</h3>
<p>Two methods</p>
<ol>
<li>Re-boot the machine, not my preference as this puts stress on the database keeping its integrity (very low probabililty).</li>
<li>using the cockpit<br>
goto  <em>Services</em> , find plexmediaservice in the list and click.<br>
using the stop start  button to force the restart</li>
</ol>
<h3 id="plex-not-running-after-update-or-restart">Plex not running after update or restart</h3>
<p>Sometimes after plex has been updated the service is required to be restarted as per above.</p>
<h3 id="plex-client-reporting-server-has-outstanding-update.">Plex Client reporting Server has outstanding update.</h3>
<p>This message should disappear after 6am daily. As the auto update includes updating the plexmedaserver.<br>
If the problem continues (very rare in my experience), its most likley the fedora update service (dnf) needs is cache flushed.<br>
using cockpit, go to terminal<br>
enter <em>sudo -i</em>  (password Plex.1)<br>
enter <em>dnf clean all</em><br>
then goto the Software Updates and do an update.</p>

