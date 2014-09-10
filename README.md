<h1>KPHP Debugger</h1>
 
<h2>Installation</h2>

<ol>
  <li>Download Eclipse Kepler: <a href="http://download.eclipse.org/eclipse/downloads/drops4/R-4.3.2-201402211700/"> 4.3.2 Release </li>
  <li>Install PHP Development Tools <a href="http://www.eclipse.org/pdt/">PDT</li>
    <p>
      From Eclipse menu: <strong>Help</strong> > <strong>Install New Software</strong>
      Work with: http://download.eclipse.org/tools/pdt/updates/3.3
    </p>
  <li>Install <a href="http://www.graphviz.org"> Graphviz </li>
  <li>Put <code>org.phpsemantics.debug.core</code> ,<code>org.phpsemantics.debug.ui</code> and <code>tools</code> into <em>dropins</em> folder under the Eclipse directory.</li>

</ol>

<h2>TroubleShooting</h2>
<h2>Check Tools</h2>

 
<ul>
<li>kphp</li>
<p>
<strong>Check if the interpreter is working:</strong><br />
run following commands under tools directory:<br />
<code>cd kphp2</code><br />
<code>cd ./krun -version</code><br />
Then you will see following outputs:<br />
K-framework nightly build.<br />
Git Revision: eb0a7cb<br />
Build date: Fri May 23 10:49:48 CDT 2014
</p>

<p>
<strong>Check version of the k tool</strong><br />
run following commands under tools directory:<br />
<code>cd k/bin</code><br />
<code>cd scripts/kphp example-breakpoint.php --config</code><br />
Then you will output in xml annotation. If not, you need to re-kompile php.k<br />
</p>

<p>
<strong>kompile php.k</strong>
<code>cd k/bin</code><br />
<code>./kompile ./../../kphp2/php.k</code><br />


</p>



<li>dot</li>
</ul>

