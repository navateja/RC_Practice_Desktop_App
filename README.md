RC_Practice_Desktop_App
=======================

This is a desktop application for practicing reading comprehensions. Unlike its <a href='https://github.com/lagnajeet/RC_Practice_Utility'>predecessor</a> which was just an HTML file with the logic implemented in JavaScript this is a true desktop application. It accepts data files as XML documents. The data format of the XML document is as shown below.

<pre>
<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>passages</span><span style='color:#7f0055; '>></span>	
	<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>passage_data</span> pid=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>[passage_index]</span><span style='color:#0000ff; '>"</span><span style='color:#7f0055; '>></span>
		<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>data</span> txt=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>[passage_data]</span><span style='color:#0000ff; '>"</span><span style='color:#7f0055; '>></span><span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>data</span><span style='color:#7f0055; '>></span>
		<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>questions</span><span style='color:#7f0055; '>></span>
			<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>question_data</span> qid=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>[question_index]</span><span style='color:#0000ff; '>"</span><span style='color:#7f0055; '>></span>
				<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>data</span> txt=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>[question]</span><span style='color:#0000ff; '>"</span> index=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>0</span><span style='color:#0000ff; '>"</span><span style='color:#7f0055; '>></span><span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>data</span><span style='color:#7f0055; '>></span>
				<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>data</span> txt=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>[answer]</span><span style='color:#0000ff; '>"</span> index=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>1</span><span style='color:#0000ff; '>"</span><span style='color:#7f0055; '>></span><span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>data</span><span style='color:#7f0055; '>></span>
				<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>data</span> txt=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>[option1]</span><span style='color:#0000ff; '>"</span> index=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>2</span><span style='color:#0000ff; '>"</span><span style='color:#7f0055; '>></span><span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>data</span><span style='color:#7f0055; '>></span>
				<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>data</span> txt=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>[option2]</span><span style='color:#0000ff; '>"</span> index=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>3</span><span style='color:#0000ff; '>"</span><span style='color:#7f0055; '>></span><span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>data</span><span style='color:#7f0055; '>></span>
				<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>data</span> txt=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>[option3]</span><span style='color:#0000ff; '>"</span> index=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>4</span><span style='color:#0000ff; '>"</span><span style='color:#7f0055; '>></span><span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>data</span><span style='color:#7f0055; '>></span>
				<span style='color:#7f0055; '>&lt;</span><span style='color:#7f0055; '>data</span> txt=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>[option4]</span><span style='color:#0000ff; '>"</span> index=<span style='color:#0000ff; '>"</span><span style='color:#0000ff; '>5</span><span style='color:#0000ff; '>"</span><span style='color:#7f0055; '>></span><span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>data</span><span style='color:#7f0055; '>></span>
			<span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>question_data</span><span style='color:#7f0055; '>></span>
		<span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>questions</span><span style='color:#7f0055; '>></span>
	<span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>passage_data</span><span style='color:#7f0055; '>></span>
<span style='color:#7f0055; '>&lt;/</span><span style='color:#7f0055; '>passages</span><span style='color:#7f0055; '>></span>
</pre>

The executables can be downloaded from <a href="https://github.com/lagnajeet/RC_Practice_Desktop_App/blob/master/RC_Practice_Utility_32bit_Windows_Linux.zip?raw=true">RC_Practice_Utility_32bit_Windows_Linux</a>. It contains an example <a href="https://github.com/lagnajeet/RC_Practice_Desktop_App/blob/master/data.xml">data.xml</a> file and the program compiled for both Windows and Linux. It can also be compiled for Mac.
<br><br>
It uses <a href="www.fltk.org">FLTK</a> for the GUI and <a href="rapidxml.sourceforge.net">RapidXML</a> for XML parsing.
