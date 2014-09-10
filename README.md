<h1>KPHP Debugger</h1>
 
<h2>Installation</h2>

<ol>
  <li>Download Eclipse Kepler: <a href="http://download.eclipse.org/eclipse/downloads/drops4/R-4.3.2-201402211700/"> 4.3.2 Release</a> </li>
  <li>Install PHP Development Tools <a href="http://www.eclipse.org/pdt/">PDT</a></li>
    <p>
      From Eclipse menu: <strong>Help</strong> > <strong>Install New Software</strong>
      Work with: http://download.eclipse.org/tools/pdt/updates/3.3
    </p>
  <li>Install <a href="http://www.graphviz.org"> Graphviz </a></li>
  <li>Put <code>org.phpsemantics.debug.core</code> ,<code>org.phpsemantics.debug.ui</code> and <code>tools</code> into <em>dropins</em> folder under the Eclipse directory.</li>

</ol>


<h2>Setup</h2>
<ol>
<li>set path of dot in <code>makeGraph</code>(only for Mac)</li>
<p>
You need to add the path of dot tool into <code>makeGraph</code> script as following:.<br />
Change <code>export PATH=$PATH</code> with <code>export PATH="/path/of/dot":$PATH</code><br />
You can get path of dot by:<code>which dot</code>
</p>
<li>kompile php.k</li>
<p>Under <code>kphp2</code> directory,  run this command: <code>./../k/bin/kompile/php.k</code><br />
This might take a few minutes. When it finishes, you get the <code>php-kompiled</code> folder in <code>kphp2</code>.
</p>
</ol>




<h2>TroubleShooting</h2>
<p>
<strong>Check if the interpreter is working:</strong><br />
run following commands under <code>tools/kphp2</code> directory:<br />
<code>scripts/kphp example-breakpoint.php</code><br />
Then you should get output in XML-like notationm (go to <a href="http://www.doc.ic.ac.uk/~maffeis/phpsemantics/documentation.html">KPHP website</a> to know more about output)

<p>
<strong>Check version of the k tool</strong><br />
run following commands under tools/k/bin:<br />
<code>./krun -version</code><br />
Then it should say:
<code>cd ./krun -version</code><br />
K-framework nightly build.<br />
Git Revision: eb0a7cb<br />
Build date: Fri May 23 10:49:48 CDT 2014
</p>

<p>
<strong>Check the dot tool</strong><br />
Under tools directory, run following command:<br />
<code>./makeGraph example.dot example.png</code><bt />
Then you should get a directed graph.

</p>



