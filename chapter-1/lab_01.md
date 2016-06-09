
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Geographic-Data-Science---Lab-01">Geographic Data Science - Lab 01<a class="anchor-link" href="#Geographic-Data-Science---Lab-01">&#182;</a></h1><p><a href="http://darribas.org">Dani Arribas-Bel</a></p>
<h1 id="Computational-tools-for-Geographic-Data-Science">Computational tools for Geographic Data Science<a class="anchor-link" href="#Computational-tools-for-Geographic-Data-Science">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>In this first tutorial we will introduce the main tools we will be working with throughout the rest of the course. Although very basic and seemingly abstract, everything showed here will become the basis on top of which we will build more sophisticated (and fun) tasks. But, before, let us get to know the tools that will give us data super-powers.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Open-Source">Open Source<a class="anchor-link" href="#Open-Source">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This course will introduce you to a series of computational tools that make the life of the Data Scientist possible, and much easier. All of them are <a href="https://en.wikipedia.org/wiki/Open_source">open-source</a>, which means the creators of these pieces of software have made available the source code for people to use it, study it, modify it, and re-distribute it. This has allowed a large eco-system that today represents the best option for scientific computing, and is used widely both in industry and academia. Thanks to this, this course can be taught with entirely freely available tools that you can install in any of your computers.</p>
<p>If you want to learn more about open-source and free software, here are a few links:</p>
<ul>
<li><strong>[Video]</strong>: brief <a href="https://www.youtube.com/watch?v=Tyd0FO0tko8">explanation</a> of open source.</li>
<li><strong>[Book]</strong> <a href="https://en.wikipedia.org/wiki/The_Cathedral_and_the_Bazaar">The Cathedral and the Bazaar</a>: classic book, freely available, that documents the benefits and history of open-source software.</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Jupyter-Notebook"><code>Jupyter</code> Notebook<a class="anchor-link" href="#Jupyter-Notebook">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The main computational tool you will be using during this course is the <a href="http://jupyter.org/">Jupyter notebook</a>. Notebooks are a convenient way to thread text, code and the output it produces in a simple file that you can then share, edit and modify. You can think of notebooks as the Word document of Data Scientists, just better.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Start-a-notebook">Start a notebook<a class="anchor-link" href="#Start-a-notebook">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>In order to begin a notebook session, you need to do it from what is called the <em>command line</em>, a terminal window that allows you to interact with your computer through written commands. This is how you can fire up a terminal:</p>
<ul>
<li>If you are on a <strong>Windows</strong> computer, you can start PowerShell from the Start menu (<code>cmd prompt</code>). </li>
<li>On a <strong>Mac</strong>, fire up the Terminal.app utility. </li>
<li>In <strong>Linux</strong>, use any of the terminals available.</li>
</ul>
<p>Then type the following command</p>

<pre><code>&gt; source activate gds</code></pre>
<p><strong>NOTE</strong>: ignore <code>source</code> if you are on Windows and simply type <code>activate gds</code>.</p>
<p>Then launch <code>Jupyter</code> by typing on the same terminal:</p>

<pre><code>&gt; jupyter notebook</code></pre>
<p>This should bring up a browser window with a home page that looks more or less like this (although with a different list of files probably):</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><img src="figs/lab01_jupyter_home.png" alt="Jupyter home"></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Navigate until the folder where you have placed the <code>lab_01.ipynb</code> file for this tutorial and click on it. This will open the notebook on a different tab. You are now on the interactive version of the notebook!</p>
<p>When you are finished with the session, you can save the notebook with <code>File -&gt; Save and Checkpoint</code>. Everything you do on the notebook (text, code and output) is saved into an <code>.ipynb</code> file that you can open later, share, etc.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Cells">Cells<a class="anchor-link" href="#Cells">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The main building block of notebooks are cells. These are chunks of the same time of content which can be cut, pasted, and moved around in a notebook. Cells can be of two types:</p>
<ul>
<li><strong>Text</strong>, like the one where this is written.</li>
<li><strong>Code</strong>, like the following one below:</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[1]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="c1"># This is a code cell</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>You can create a new cell by clicking <code>Insert</code> -&gt; <code>Cell Above</code>/<code>Below</code> in the top menu. By default, this will be a code cell, but you can change that on the <code>Cell</code> -&gt; <code>Cell Type</code> menu. Choose <code>Markdown</code> for a text cell. Once a new cell is created, you can edit it by clicking on it, which will create the cursor bar inside for you to start typing.</p>
<p><strong>Pro tip!</strong>: cells can also be created with shortcuts. If you press <code>&lt;escape&gt;</code> and then <code>b</code> (<code>a</code>), a new cell will be created below (above). There is a whole bunch of shortcuts you can explore by pressing <code>&lt;escape&gt;</code> and <code>h</code> (press <code>&lt;escape&gt;</code> again to leave the help).</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Code-and-its-output">Code and its output<a class="anchor-link" href="#Code-and-its-output">&#182;</a></h3><p>A particularly useful feature of notebooks is that you can save, in the same place, the code you use to generate any output (tables, figures, etc.). As an example, the cell below contains a snipet of Python that returns a printed statement. This statement is then printed below and recorded in the notebook as output:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[2]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">print</span><span class="p">(</span><span class="s2">&quot;Hello world!!!&quot;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>Hello world!!!
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Note also how the notebook has automatic syntax highlighting support for Python. This makes the code much more readable and understandable. More on Python below.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Markdown">Markdown<a class="anchor-link" href="#Markdown">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Text cells in a notebook use the <a href="https://help.github.com/articles/github-flavored-markdown/">Github Flavored Markdown</a> markup language. This means you can write plain text with some rules and the notebook renders a more visually appealing version of it. Let's see some examples:</p>
<ul>
<li><strong>BOLD</strong>:</li>
</ul>
<p><code>This is **bold**.</code></p>
<p>Is rendered:</p>
<p>This is <strong>bold</strong>.</p>
<ul>
<li><strong>ITALIC</strong>:</li>
</ul>
<p><code>This is *italic*.</code></p>
<p>Is rendered:</p>
<p>This is <em>italic</em>.</p>
<ul>
<li><strong>LISTS</strong>:</li>
</ul>
<p>You can create unnumbered lists:</p>

<pre><code>* Item 1
* Item 2
* ...</code></pre>
<p>Which will produce:</p>
<ul>
<li>Item 1</li>
<li>Item 2</li>
<li>...</li>
</ul>
<p>Or you can create numbered lists:</p>

<pre><code>1. First element
1. Second element
1. ...</code></pre>
<p>And get:</p>
<ol>
<li>First element</li>
<li>Second element</li>
<li>...</li>
</ol>
<p>Note that you don't have to write the actual number of the element, just using <code>1.</code> always produces a numbered list.</p>
<p>You can also nest lists:</p>

<pre><code>* First unnumbered element, which can be split into:

    1. One numbered element
    2. Another numbered element

* Second element.
* ...</code></pre>
<ul>
<li><p>First unnumbered element, which can be split into:</p>
<ol>
<li>One numbered element</li>
<li>Another numbered element</li>
</ol>
</li>
<li><p>Second element.</p>
</li>
<li>...</li>
</ul>
<p>This creates many oportunities to combine things nicely.</p>
<ul>
<li><strong>LINKS</strong></li>
</ul>
<p><code>You can easily create hyperlinks, for example to [WikiPedia](https://www.wikipedia.org/).</code></p>
<p>You can easily create hyperlinks, for example to <a href="https://www.wikipedia.org/">WikiPedia</a>.</p>
<ul>
<li><strong>HEADINGS</strong>: including <code>#</code> before a line causes it to render a heading.</li>
</ul>
<hr>
<p><code># This is Header 1</code></p>
<p>Turns into:</p>
<h1 id="This-is-Header-1">This is Header 1<a class="anchor-link" href="#This-is-Header-1">&#182;</a></h1><hr>
<p><code>## This is Header 2</code></p>
<p>Turns into:</p>
<h2 id="This-is-Header-2">This is Header 2<a class="anchor-link" href="#This-is-Header-2">&#182;</a></h2><hr>
<p><code>### This is Header 3</code></p>
<p>Turns into:</p>
<h3 id="This-is-Header-3">This is Header 3<a class="anchor-link" href="#This-is-Header-3">&#182;</a></h3><p>And so on...</p>
<hr>
<p>You can see a more in detail introduction in the following links:</p>
<blockquote><p><a href="https://help.github.com/articles/markdown-basics/">https://help.github.com/articles/markdown-basics/</a></p>
<p><a href="https://help.github.com/articles/github-flavored-markdown/">https://help.github.com/articles/github-flavored-markdown/</a></p>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Rich-content-in-a-notebook">Rich content in a notebook<a class="anchor-link" href="#Rich-content-in-a-notebook">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Notebooks can also include rich content from the web. For that, we need to import the <code>display</code> module:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[3]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="kn">import</span> <span class="nn">IPython.display</span> <span class="kn">as</span> <span class="nn">display</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This makes available additional functionality that allows us to embed rich content. For example, we can include a YouTube clip easily by passing it's ID:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[4]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">display</span><span class="o">.</span><span class="n">YouTubeVideo</span><span class="p">(</span><span class="s1">&#39;iinQDhsdE9s&#39;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[4]:</div>

<div class="output_html rendered_html output_subarea output_execute_result">

        <iframe
            width="400"
            height="300"
            src="https://www.youtube.com/embed/iinQDhsdE9s"
            frameborder="0"
            allowfullscreen
        ></iframe>
        
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Or we can pass standard HTML code:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[5]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">display</span><span class="o">.</span><span class="n">HTML</span><span class="p">(</span><span class="s2">&quot;&quot;&quot;&lt;table&gt;</span>
<span class="s2">&lt;tr&gt;</span>
<span class="s2">&lt;th&gt;Header 1&lt;/th&gt;</span>
<span class="s2">&lt;th&gt;Header 2&lt;/th&gt;</span>
<span class="s2">&lt;/tr&gt;</span>
<span class="s2">&lt;tr&gt;</span>
<span class="s2">&lt;td&gt;row 1, cell 1&lt;/td&gt;</span>
<span class="s2">&lt;td&gt;row 1, cell 2&lt;/td&gt;</span>
<span class="s2">&lt;/tr&gt;</span>
<span class="s2">&lt;tr&gt;</span>
<span class="s2">&lt;td&gt;row 2, cell 1&lt;/td&gt;</span>
<span class="s2">&lt;td&gt;row 2, cell 2&lt;/td&gt;</span>
<span class="s2">&lt;/tr&gt;</span>
<span class="s2">&lt;/table&gt;&quot;&quot;&quot;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[5]:</div>

<div class="output_html rendered_html output_subarea output_execute_result">
<table>
<tr>
<th>Header 1</th>
<th>Header 2</th>
</tr>
<tr>
<td>row 1, cell 1</td>
<td>row 1, cell 2</td>
</tr>
<tr>
<td>row 2, cell 1</td>
<td>row 2, cell 2</td>
</tr>
</table>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Note that this opens the door for including a large number of elements from the web, as an <code>iframe</code> is also allowed. For example, interactive maps can be included:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[6]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">osm</span> <span class="o">=</span> <span class="s2">&quot;&quot;&quot;</span>
<span class="s2">&lt;iframe width=&quot;425&quot; height=&quot;350&quot; frameborder=&quot;0&quot; scrolling=&quot;no&quot; marginheight=&quot;0&quot; marginwidth=&quot;0&quot; src=&quot;http://www.openstreetmap.org/export/embed.html?bbox=-2.9662737250328064%2C53.400500637844594%2C-2.964626848697662%2C53.402550738394034&amp;amp;layer=mapnik&quot; style=&quot;border: 1px solid black&quot;&gt;&lt;/iframe&gt;&lt;br/&gt;&lt;small&gt;&lt;a href=&quot;http://www.openstreetmap.org/#map=19/53.40153/-2.96545&quot;&gt;View Larger Map&lt;/a&gt;&lt;/small&gt;</span>
<span class="s2">&quot;&quot;&quot;</span>
<span class="n">display</span><span class="o">.</span><span class="n">HTML</span><span class="p">(</span><span class="n">osm</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[6]:</div>

<div class="output_html rendered_html output_subarea output_execute_result">

<iframe width="425" height="350" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="http://www.openstreetmap.org/export/embed.html?bbox=-2.9662737250328064%2C53.400500637844594%2C-2.964626848697662%2C53.402550738394034&amp;layer=mapnik" style="border: 1px solid black"></iframe><br/><small><a href="http://www.openstreetmap.org/#map=19/53.40153/-2.96545">View Larger Map</a></small>

</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Or sound content:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[7]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">sound</span> <span class="o">=</span> <span class="s1">&#39;&#39;&#39;</span>
<span class="s1">&lt;iframe width=&quot;100%&quot; height=&quot;450&quot; scrolling=&quot;no&quot; frameborder=&quot;no&quot; src=&quot;https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/178720725&amp;amp;auto_play=false&amp;amp;hide_related=false&amp;amp;show_comments=true&amp;amp;show_user=true&amp;amp;show_reposts=false&amp;amp;visual=true&quot;&gt;&lt;/iframe&gt;</span>
<span class="s1">&#39;&#39;&#39;</span>
<span class="n">display</span><span class="o">.</span><span class="n">HTML</span><span class="p">(</span><span class="n">sound</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[7]:</div>

<div class="output_html rendered_html output_subarea output_execute_result">

<iframe width="100%" height="450" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/178720725&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;visual=true"></iframe>

</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>A more thorough exploration of them is available in <a href="http://jeffskinnerbox.me/notebooks/ipython's-rich-display-system.html">this</a> notebook.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Exercise-to-work-on-your-own">Exercise to work on your own<a class="anchor-link" href="#Exercise-to-work-on-your-own">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Try to reproduce, using markdown and the different tools the notebook affords you, the following WikiPedia entry:</p>
<blockquote><p><a href="https://en.wikipedia.org/wiki/Chocolate_chip_cookie_dough_ice_cream">https://en.wikipedia.org/wiki/Chocolate_chip_cookie_dough_ice_cream</a></p>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[8]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">display</span><span class="o">.</span><span class="n">IFrame</span><span class="p">(</span><span class="s1">&#39;https://en.wikipedia.org/wiki/Chocolate_chip_cookie_dough_ice_cream&#39;</span><span class="p">,</span> 
              <span class="mi">700</span><span class="p">,</span> <span class="mi">500</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[8]:</div>

<div class="output_html rendered_html output_subarea output_execute_result">

        <iframe
            width="700"
            height="500"
            src="https://en.wikipedia.org/wiki/Chocolate_chip_cookie_dough_ice_cream"
            frameborder="0"
            allowfullscreen
        ></iframe>
        
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Pay special attention in getting the bold, italics, links, headlines and lists correctly formated. Bonus if you manage to insert the image as well!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Python">Python<a class="anchor-link" href="#Python">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Although we will have a look at other programs, the main bulk of the course relies on the <a href="https://www.python.org/">Python</a> programming language. Python is a <a href="https://en.wikipedia.org/wiki/High-level_programming_language">high-level</a> programming language widely used today. To give a couple of examples of its relevance, it is underlying <a href="https://www.quora.com/How-does-dropbox-use-python-What-features-are-implemented-in-it-any-tangentially-related-material?share=1">most of the Dropbox</a> systems, but also heavily <a href="https://www.python.org/about/success/usa/">used</a> to control satellites at NASA. A great deal of Science is also done in Python, from <a href="https://www.youtube.com/watch?v=mLuIB8aW2KA">research in astronomy</a> at UC Berkley, to <a href="http://www.quant-econ.net/">courses in economics</a> by Nobel Prize Professors.</p>
<p>This course uses Python because it has emerged as one of the main and most solid options for Data Science, together with other free alternatives such as R. Python is widely used for data processing and analysis both in academia and in industry. There is a vibrant and growing scientific community (<a href="http://scipy.org/">example</a> and <a href="http://pydata.org/">example</a>), working at both universities and companies, that supports and enhances its capabilities for data analysis by providing new and refining existing extensions (a.ka.a. libraries, see below). In the geospatial world, Python is also very widely adopted, being the selected language for scripting in both <a href="http://www.esri.com/software/arcgis">ArcGIS</a> and <a href="http://qgis.org">QGIS</a>. All of this means that, whether you are thinking of continuing in Higher Education or trying to find a job in industry, Python will be an importan asset that employers will significantly value.</p>
<p>Being a high-level language means that the code can be "dynamically interpreted", which means it is run on-the-fly without the need to be compiled. This is in contrast to "low-level" programming languages, which first need to be converted into machine code (i.e. compiled) before they can be run. With Python, one does not need to worry about compilation and can just write code, evaluate, fix it, re-evaluate it, etc. in a quick cycle, making it a very productive tool. The rest of this tutorial covers some of the basic elements of the language, from conventions like how to comment your code, to the basic data structures available.</p>
<p>The rest of the tutorial is partly inspired by the introductory lesson in <a href="https://github.com/barbagroup/CFDPython">this course</a> by Lorena Barba's group.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Python-libraries">Python libraries<a class="anchor-link" href="#Python-libraries">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The standard Python language includes some data structures (e.g. lists, dictionaries, etc. See below) and allows many basic operations (e.g. sum, product, etc.). For example, right out of the box, and without any further action needed, you can use Python as a calculator:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[9]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="mi">3</span> <span class="o">+</span> <span class="mi">5</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[9]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>8</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[10]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="mf">2.</span> <span class="o">/</span> <span class="mi">3</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[10]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>0.6666666666666666</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[11]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="p">(</span><span class="mi">3</span> <span class="o">+</span> <span class="mi">5</span><span class="p">)</span> <span class="o">*</span> <span class="mf">2.</span> <span class="o">/</span> <span class="mi">3</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[11]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>5.333333333333333</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>However, the strength of Python as a data analysis tool comes from the extensions provided separately that add functionality and provide access to much more sophisticated data structures and functions. These come in the form of packages, or libraries, that once installed need to be imported into a session.</p>
<p>In this course, we will be using many of the core libraries of what has been called the "PyData stack", the set of libraries that make Python a full-fledge system for Data Science. We will introduce them gradually as we need them for particular tasks but, for now, let us have a look at the foundational library, <a href="http://www.numpy.org/">numpy</a> (short for numerical Python). Importing it is simple:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[12]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="kn">import</span> <span class="nn">numpy</span> <span class="kn">as</span> <span class="nn">np</span> <span class="c1"># we rename it in the session as `np` by convention</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Note how we import it <em>and</em> rename it in the session, from <code>numpy</code> to <code>np</code>, which is shorter and more convenient.</p>
<p>Note also how comments work in Python: everything in a line <em>after</em> the <code>#</code> sign is ignored by Python when it evaluates the code. This allows you to insert comments that Python will ignore but that can help you and others better understand the code.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Once imports are out of the way, let us start exploring what we can do with <code>numpy</code>. One of the easiest tasks is to create a sequence of numbers:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[13]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">seq</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">)</span>
<span class="n">seq</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[13]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The first thing to note is that, in line 1, we create the sequence by calling the function <code>arange</code> and assign it to an object called <code>seq</code> (it could have been called anything else, pick your favorite) and, in line 2, we have it printed as the output of the cell.</p>
<p>Another interesting feature is how, since we are calling a <code>numpy</code> function called <code>arange</code> by adding <code>np.</code> in front. This is to note that the function comes explicitly from <code>numpy</code>. To find out how necessary this is, you can try generating the sequence without <code>np</code>:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[14]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">seq</span> <span class="o">=</span> <span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">)</span>
<span class="n">seq</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_text output_error">
<pre>
<span class="ansired">---------------------------------------------------------------------------</span>
<span class="ansired">NameError</span>                                 Traceback (most recent call last)
<span class="ansigreen">&lt;ipython-input-14-8381d1c402c4&gt;</span> in <span class="ansicyan">&lt;module&gt;</span><span class="ansiblue">()</span>
<span class="ansigreen">----&gt; 1</span><span class="ansiyellow"> </span>seq <span class="ansiyellow">=</span> arange<span class="ansiyellow">(</span><span class="ansicyan">10</span><span class="ansiyellow">)</span><span class="ansiyellow"></span>
<span class="ansigreen">      2</span> seq<span class="ansiyellow"></span>

<span class="ansired">NameError</span>: name &apos;arange&apos; is not defined</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>What you get instead is an error, also called a "traceback". In particular, Python is telling that it cannot find a function named <code>arange</code> in the core library. This is because that particular function is only available in <code>numpy</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Variables">Variables<a class="anchor-link" href="#Variables">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>A basic feature of Python is the ability to assign a name to different "things", or objects. These can also be called sometimes "variables". We have already seen that in the example above but, to make it more explicit, let us make it even simpler. For example, an object can be a single number:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[15]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">a</span> <span class="o">=</span> <span class="mi">3</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Or a name, also called "string":</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[16]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">b</span> <span class="o">=</span> <span class="s1">&#39;Hello World&#39;</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>You can check what type an object is also easily:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[17]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="nb">type</span><span class="p">(</span><span class="n">a</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[17]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>int</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><code>int</code> is short for "integer" which, roughly speaking, means an whole number. If you want to save a number with decimals, you will be using floats:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[18]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">c</span> <span class="o">=</span> <span class="mf">1.5</span>
<span class="nb">type</span><span class="p">(</span><span class="n">c</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[18]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>float</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>As mentioned, what we understand as letters in a wide sense (spaces and other signs count too) is called "strings" (<code>str</code> in short):</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[19]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="nb">type</span><span class="p">(</span><span class="n">b</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[19]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>str</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Help">Help<a class="anchor-link" href="#Help">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>A very handy feature of Python is the ability to access on-the-spot help for its different functions. This means that you can check what a function is supposed to do, or how to access it, right inside your Python session. Of course, this also works handsomely inside a notebook. There are a couple of ways to access the help.</p>
<p>Take the <code>numpy</code> function <code>arange</code> that we have used above. The easiest way to check interactively how to use it is by:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[20]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre>np.arange<span class="o">?</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>As you can see, this brings up a sub-window in the browser with all the information you need.</p>
<p>If, for whatever reason, you needed to print that info into the notebook itself, you can do the following:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[21]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">help</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>Help on built-in function arange in module numpy.core.multiarray:

arange(...)
    arange([start,] stop[, step,], dtype=None)
    
    Return evenly spaced values within a given interval.
    
    Values are generated within the half-open interval &#96;&#96;[start, stop)&#96;&#96;
    (in other words, the interval including &#96;start&#96; but excluding &#96;stop&#96;).
    For integer arguments the function is equivalent to the Python built-in
    &#96;range &lt;http://docs.python.org/lib/built-in-funcs.html&gt;&#96;_ function,
    but returns an ndarray rather than a list.
    
    When using a non-integer step, such as 0.1, the results will often not
    be consistent.  It is better to use &#96;&#96;linspace&#96;&#96; for these cases.
    
    Parameters
    ----------
    start : number, optional
        Start of interval.  The interval includes this value.  The default
        start value is 0.
    stop : number
        End of interval.  The interval does not include this value, except
        in some cases where &#96;step&#96; is not an integer and floating point
        round-off affects the length of &#96;out&#96;.
    step : number, optional
        Spacing between values.  For any output &#96;out&#96;, this is the distance
        between two adjacent values, &#96;&#96;out[i+1] - out[i]&#96;&#96;.  The default
        step size is 1.  If &#96;step&#96; is specified, &#96;start&#96; must also be given.
    dtype : dtype
        The type of the output array.  If &#96;dtype&#96; is not given, infer the data
        type from the other input arguments.
    
    Returns
    -------
    arange : ndarray
        Array of evenly spaced values.
    
        For floating point arguments, the length of the result is
        &#96;&#96;ceil((stop - start)/step)&#96;&#96;.  Because of floating point overflow,
        this rule may result in the last element of &#96;out&#96; being greater
        than &#96;stop&#96;.
    
    See Also
    --------
    linspace : Evenly spaced numbers with careful handling of endpoints.
    ogrid: Arrays of evenly spaced numbers in N-dimensions.
    mgrid: Grid-shaped arrays of evenly spaced numbers in N-dimensions.
    
    Examples
    --------
    &gt;&gt;&gt; np.arange(3)
    array([0, 1, 2])
    &gt;&gt;&gt; np.arange(3.0)
    array([ 0.,  1.,  2.])
    &gt;&gt;&gt; np.arange(3,7)
    array([3, 4, 5, 6])
    &gt;&gt;&gt; np.arange(3,7,2)
    array([3, 5])

</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Control-flow-(a.k.a.-for-loops-and-if-statements)">Control flow (a.k.a. <code>for</code> loops and <code>if</code> statements)<a class="anchor-link" href="#Control-flow-(a.k.a.-for-loops-and-if-statements)">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Although this does not intend to be a comprehensive introduction to computer programming or general purpose Python (check the references for that, in particular Allen Downey's <a href="http://www.greenteapress.com/thinkpython/thinkpython.html">book</a>), it is important to be aware of two building blocks of almost any computer program: <code>for</code> loops and <code>if</code> statements. It is possible that you will never require them for this course, as all that is used here is based on existing methods and functions, but it is always useful to know they exist and to be able to recognize them. They can also come in very handy in cases where you some extra functionality out of standard methods. Without further ado, let us have a look and the two single most relevant tools of computer programming.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<ul>
<li><code>for</code> loops</li>
</ul>
<p>These allow  you to repeat a particular action or task over a sequence. As an example, you can print your name ten times without having to type it yourself every single time:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[22]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">):</span>
    <span class="k">print</span> <span class="s1">&#39;my name&#39;</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>my name
my name
my name
my name
my name
my name
my name
my name
my name
my name
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Note a couple of features in the loop:</p>
<ol>
<li>You loop <em>over</em> a sequence, in this particular case the sequence of ten numbers created by <code>np.arange(10)</code>.</li>
<li>In every step, for every element of the sequence in this case, you repeat an action. Here we are printing the same text, <code>my name</code>.</li>
<li>Although not used in this simple loop, each of the elements you loop over can be accessed inside the loop. This can be irrelevant, as in the loop above, or extremely useful, it depends on the context. For example, see a case where you use the value of the sequence in each step:</li>
</ol>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[23]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">):</span>
    <span class="k">print</span> <span class="s2">&quot;I am at step &quot;</span><span class="p">,</span> <span class="n">i</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>I am at step  0
I am at step  1
I am at step  2
I am at step  3
I am at step  4
I am at step  5
I am at step  6
I am at step  7
I am at step  8
I am at step  9
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>One more note: for convention, we are calling the element of the sequence <code>i</code>, but this could be named anything. In fact, in many cases, more meaningful names make code much more readable. For example, you could think of a re-write of the loop above as:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[24]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">for</span> <span class="n">step</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">):</span>
    <span class="k">print</span> <span class="s2">&quot;I am at step &quot;</span><span class="p">,</span> <span class="n">step</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>I am at step  0
I am at step  1
I am at step  2
I am at step  3
I am at step  4
I am at step  5
I am at step  6
I am at step  7
I am at step  8
I am at step  9
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<ul>
<li><code>if</code> statements</li>
</ul>
<p>We have just seen how <code>for</code> loops allow you to repeat an action over a sequence. In the case of <code>if</code> statements, these allow you to select or restrict such actions to only those cases that meet a condition(s) you specify in the statement.</p>
<p>For example, if you think of the loops written above, you might want to only print those that are odd, skipping those that are even:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[25]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">):</span>
    <span class="k">if</span> <span class="n">i</span><span class="o">%</span><span class="k">2</span>:
        <span class="k">print</span> <span class="n">i</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>1
3
5
7
9
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Ignore for the moment the part <code>i%2</code>, just remember this is one way Python has to check if a number is odd. The important bit in this loop, as compared to the simpler one above, is that we are using an <code>if</code> statement to select only those candidates that meet the condition. In other words, what we are doing it looping over every number in the sequence from zero to nine (<code>for i in np.arange(10)</code>) and checking if they are even or odd (<code>if i%2</code>). If they meet the condition, they are odd, then we proceed and print them on the screen.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>A full <code>if</code> statement also allows for an action to be taken if the original condition is not satisfied. This is called an "ifelse" statement. For example, you can think of a loop that prints the type of each number in a sequence:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[26]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">):</span>
    <span class="c1"># Check if it is odd</span>
    <span class="k">if</span> <span class="n">i</span><span class="o">%</span><span class="k">2</span>:
        <span class="k">print</span> <span class="n">i</span><span class="p">,</span> <span class="s1">&#39; is odd&#39;</span>
    <span class="c1"># If not odd (even), then do the following</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="k">print</span> <span class="n">i</span><span class="p">,</span> <span class="s1">&#39; is even&#39;</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>0  is even
1  is odd
2  is even
3  is odd
4  is even
5  is odd
6  is even
7  is odd
8  is even
9  is odd
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Data-structures">Data structures<a class="anchor-link" href="#Data-structures">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The standard python you can access without importing any additional libraries contains a few core data structures that is very handy to know. Most of data analysis is done on top of other structures specifically designed for the purpose (numpy arrays and pandas dataframes, mostly. See the following sessions for more details), but some understanding of these core Python structures is very useful. In this context, we will look at three: values, lists, and dictionaries.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<ul>
<li><strong>Values</strong>: these are the most basic elements to organize data and information in Python. You can think of them as numbers (integers or floats) or words (strings). Typically, these are the elements that will be stored in lists and dictionaries.</li>
</ul>
<p>An integer is a whole number:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[27]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">i</span> <span class="o">=</span> <span class="mi">5</span>
<span class="nb">type</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[27]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>int</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>A float is a number that allows for decimals:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[28]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">f</span> <span class="o">=</span> <span class="mf">5.2</span>
<span class="nb">type</span><span class="p">(</span><span class="n">f</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[28]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>float</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Note that a float can also not have decimals and still be stored as such:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[29]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">fw</span> <span class="o">=</span> <span class="mf">5.</span>
<span class="nb">type</span><span class="p">(</span><span class="n">fw</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[29]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>float</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>However, they are different representations:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[30]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">f</span> <span class="o">==</span> <span class="n">fw</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[30]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>False</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<ul>
<li><strong>Lists</strong>: a list is an ordered sequence of values that can be of mixed types. They are represented between squared brackets (<code>[]</code>) and, although not very efficient in memory terms, are very flexible and useful to "put things together".</li>
</ul>
<p>For example, the following list of integers:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[31]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">l</span> <span class="o">=</span> <span class="p">[</span><span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">5</span><span class="p">]</span>
<span class="n">l</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[31]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>[1, 2, 3, 4, 5]</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[32]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="nb">type</span><span class="p">(</span><span class="n">l</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[32]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>list</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Or the following mixed one:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[33]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">m</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;a&#39;</span><span class="p">,</span> <span class="s1">&#39;b&#39;</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="s1">&#39;c&#39;</span><span class="p">,</span> <span class="mi">6</span><span class="p">,</span> <span class="mi">7</span><span class="p">]</span>
<span class="n">m</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[33]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>[&apos;a&apos;, &apos;b&apos;, 5, &apos;c&apos;, 6, 7]</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Lists can be queried and sliced. For example, the first element can be retrieved by:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[34]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">l</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[34]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>1</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Or the second to the fourth:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[35]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">:</span><span class="mi">4</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[35]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>[&apos;b&apos;, 5, &apos;c&apos;]</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Lists can be added:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[36]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">l</span> <span class="o">+</span> <span class="n">m</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[36]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>[1, 2, 3, 4, 5, &apos;a&apos;, &apos;b&apos;, 5, &apos;c&apos;, 6, 7]</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>New elements added:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[37]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">l</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="mi">4</span><span class="p">)</span>
<span class="n">l</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[37]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>[1, 2, 3, 4, 5, 4]</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Or modified:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[38]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">l</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[38]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>2</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[39]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">l</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">=</span> <span class="s1">&#39;two&#39;</span>
<span class="n">l</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[39]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>&apos;two&apos;</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[40]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">l</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[40]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>[1, &apos;two&apos;, 3, 4, 5, 4]</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<ul>
<li><strong>Dictionaries</strong>: dictionaries are unordered collections of "keys" and "values". A key, which can be of any kind, is the element associated with a "value", which can also be of any kind. Dictionaries are used when order is not important but you need fast and easy lookup. They are expressed in curly brackets, with keys and values being linked through columns.</li>
</ul>
<p>For example, we can think of a dictionary to store a series of names and the ages of the people they represent:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[41]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">ages</span> <span class="o">=</span> <span class="p">{</span><span class="s1">&#39;Ana&#39;</span><span class="p">:</span> <span class="mi">24</span><span class="p">,</span> <span class="s1">&#39;John&#39;</span><span class="p">:</span> <span class="mi">20</span><span class="p">,</span> <span class="s1">&#39;Li&#39;</span><span class="p">:</span> <span class="mi">27</span><span class="p">,</span> <span class="s1">&#39;Ivan&#39;</span><span class="p">:</span> <span class="mi">40</span><span class="p">,</span> <span class="s1">&#39;Tali&#39;</span><span class="p">:</span><span class="mi">33</span><span class="p">}</span>
<span class="n">ages</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[41]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>{&apos;Ana&apos;: 24, &apos;Ivan&apos;: 40, &apos;John&apos;: 20, &apos;Li&apos;: 27, &apos;Tali&apos;: 33}</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[42]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="nb">type</span><span class="p">(</span><span class="n">ages</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[42]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>dict</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Dictionaries can then be queried and values retrieved easily by using their keys. For example, if we quickly want to know Li's age:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[43]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">ages</span><span class="p">[</span><span class="s1">&#39;Li&#39;</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[43]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>27</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Similarly to lists, you can modify and assign new values:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[44]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">ages</span><span class="p">[</span><span class="s1">&#39;Juan&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="mi">73</span>
<span class="n">ages</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[44]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>{&apos;Ana&apos;: 24, &apos;Ivan&apos;: 40, &apos;John&apos;: 20, &apos;Juan&apos;: 73, &apos;Li&apos;: 27, &apos;Tali&apos;: 33}</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Using this property, you can create entirely empty dictionaries and populate them later on:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[45]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">newdict</span> <span class="o">=</span> <span class="p">{}</span>
<span class="n">newdict</span><span class="p">[</span><span class="s1">&#39;key1&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="mi">1</span>
<span class="n">newdict</span><span class="p">[</span><span class="s1">&#39;key2&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="mi">2</span>
<span class="n">newdict</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[45]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>{&apos;key1&apos;: 1, &apos;key2&apos;: 2}</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Functions">Functions<a class="anchor-link" href="#Functions">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The last part of this whirlwind tour on Python relates to functions, or more properly termed, methods. The motivation is that, so far, we have only seen how you can create Python code that, if you want to run again somewhere else, you need to copy and paste entirely. However, as we will see in more detail later in the course, one of the main reasons why you want to use Python for data analysis, instead of a point-and-click graphical interface like SPSS, for instance, is that you can easily reuse code and re-run analyses easily. Methods help us accomplish this by encapsulating snippets of code that perform a particular task and making them available to be called.</p>
<p>We have already <em>used</em> methods here. When we call <code>np.arange</code>, we are using one of them. Now, we will see how to <em>create</em> a method of our own that performs the specific task we want it to do. For example, let us create a very simple method to reproduce the first loop we created above:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[46]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">def</span> <span class="nf">run_simple_loop</span><span class="p">():</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">):</span>
        <span class="k">print</span> <span class="n">i</span>
    <span class="k">return</span> <span class="bp">None</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Already with this simple method, there is a bunch of interesting things going on:</p>
<ul>
<li>First, note how we define a bit of code is a method, as oposed to plain Python: we use <code>def</code> followed by the name of our function (we have chosen <code>run_simple_loop</code>, but we anything could have done).</li>
<li>Second, we append <code>()</code> after the name, and finish the line with a colon (<code>:</code>). This is necessary and will allow us to specify requirements for the function (see below).</li>
<li>Third, realize that everything inside a function needs to be indented. This is a core property of Python and, although some people find it odd, it enhances readibility greatly.</li>
<li>Fourth, the piece of code to do the task we want, printing the sequence of numbers, is inside the function in the same way it was outside, only properly indented.</li>
<li>Fifth, we finish the method with a line starting by <code>return</code>. In this case, we follow it with <code>None</code>, but this will change as methods become more sophisticated. Essentially, this is the part of the method where you specify which elements you want it to return and save for later use.</li>
</ul>
<p>Once we have paid attention to these elements, we can see how the method can be <em>called</em> and hence the code inside it executed:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[47]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">run_simple_loop</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>0
1
2
3
4
5
6
7
8
9
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This is the same way that we called <code>np.arange</code> before. Note how we do not include the colon (<code>:</code>) but simply use the name of the method followed by the parenthesis.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This is the simplest possile method you can write: you do not require anything, just executing it, and the code produces and output (the printout) but it is not saved anywhere. The rest of this section relaxes these two aspects to allow us to build more complex, but also more useful, methods.</p>
<p>First, you can specify "arguments" to be passed that modify the behaviour of the method. Remember how we called <code>np.arange</code> with a number that implied the length of the sequence we wanted returned. We can do the same thing in our own function. The main aspect to pay attention to in this context is that the arguments need to be variables, not particular values. Let us see a modified example of our method:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[48]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">def</span> <span class="nf">run_simple_loopX</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
        <span class="k">print</span> <span class="n">i</span>
    <span class="k">return</span> <span class="bp">None</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>We have replaced the fixed length of the sequence (10) by a variable named <code>x</code> that allows us to specify <em>any value we want</em> when we call the method:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[49]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">run_simple_loopX</span><span class="p">(</span><span class="mi">3</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>0
1
2
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[50]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">run_simple_loopX</span><span class="p">(</span><span class="mi">2</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>0
1
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Another way you can build more flexibility into a method is by allowing it to return an output of the computation. In the previous examples, the function performs a computation (i.e. printing values on the screen), but it does not return any value. This is in contrast with, for example, <code>np.arange</code> which does return an output, the sequence of values:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[51]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">a</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[52]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">a</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[52]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Our function does not save anything:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[53]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">b</span> <span class="o">=</span> <span class="n">run_simple_loopX</span><span class="p">(</span><span class="mi">3</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>0
1
2
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[54]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">b</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>We can modify this using the last line of a method. For example, let us assume we want to return a sequence as long as the series of numbers we print on the screen. The method should be:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[55]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">def</span> <span class="nf">run_simple_loopXout</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
        <span class="k">print</span> <span class="n">i</span>
    <span class="k">return</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">x</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Note the main difference: instead of returning <code>None</code>, we are telling Python to return a sequence, which has the same length as the one used to specify the loop. Now, there is an alternative way of being more efficient in this method, and that is assigning the sequence to a new object and using it when necessary later on. The results are exactly the same, but there are less computations performed and, more critically, we minimize the chances of making mistakes.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[56]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">def</span> <span class="nf">run_simple_loopXout</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
    <span class="n">seq</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">x</span><span class="p">)</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">seq</span><span class="p">:</span>
        <span class="k">print</span> <span class="n">i</span>
    <span class="k">return</span> <span class="n">seq</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Either of these two new versions of the method return an output:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[57]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">a</span> <span class="o">=</span> <span class="n">run_simple_loopX</span><span class="p">(</span><span class="mi">3</span><span class="p">)</span>
<span class="n">b</span> <span class="o">=</span> <span class="n">run_simple_loopXout</span><span class="p">(</span><span class="mi">3</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>0
1
2
0
1
2
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[58]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">a</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[59]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">b</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[59]:</div>


<div class="output_text output_subarea output_execute_result">
<pre>array([0, 1, 2])</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The advantage of methods, as oposed to straight code, is that they force us to think in a modular way, helping us identify exactly what it needs to be done, in what order, and what it is required. Encapsulating these atomic bits of functionality in methods allows us to write things once and flexibly use them everywhere, saving us time (and headaches) in the long run.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>A final note on functions. It is important that, whenever you create a function, you include some documentation about what it expects, what it does, and what it returns. Although there are many ways of doing this, the typical convention is as follows:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[60]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="k">def</span> <span class="nf">run_simple_loopXout</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
    <span class="sd">&quot;&quot;&quot;</span>
<span class="sd">    Print out the values of a sequence of certain length</span>
<span class="sd">    ...</span>
<span class="sd">    </span>
<span class="sd">    Arguments</span>
<span class="sd">    ---------</span>
<span class="sd">    x     : int</span>
<span class="sd">            Length of the sequence to be printed out</span>
<span class="sd">    </span>
<span class="sd">    Returns</span>
<span class="sd">    -------</span>
<span class="sd">    seq   : np.array</span>
<span class="sd">            Sequence of values printed out</span>
<span class="sd">    &quot;&quot;&quot;</span>
    <span class="n">seq</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">x</span><span class="p">)</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">seq</span><span class="p">:</span>
        <span class="k">print</span> <span class="n">i</span>
    <span class="k">return</span> <span class="n">seq</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Documentation, as any string, are highlighted in red on a notebook. Let us have a look at the structure and components of a well-made documentation (also called "docstring"):</p>
<ul>
<li>It is encapsulated between triple commas (<code>"""</code>).</li>
<li>Begins with a short description of what the method does. The shorter the better, the more concise, the even better.</li>
<li>There is a section called "Arguments" that lists the elements that the function expects. </li>
<li>Each argument is then listed, followed by its type. In this case it is an object <code>x</code> that, as we are told, needs to be an integer.</li>
<li>The arguments are followed by another section that specifies what the function returns, and of what type the output is.</li>
</ul>
<p>Documentation in this way is very useful to remember what a function does, but also to force yourself to write clearer code. A bonus is that, if you include documentation in this way, it can be checked with the standard <code>help</code> or <code>?</code> systems reviewed above:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[61]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre>run_simple_loopXout<span class="o">?</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[62]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span class="n">help</span><span class="p">(</span><span class="n">run_simple_loopXout</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>Help on function run_simple_loopXout in module __main__:

run_simple_loopXout(x)
    Print out the values of a sequence of certain length
    ...
    
    Arguments
    ---------
    x     : int
            Length of the sequence to be printed out
    
    Returns
    -------
    seq   : np.array
            Sequence of values printed out

</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Exercise-to-work-on-your-own">Exercise to work on your own<a class="anchor-link" href="#Exercise-to-work-on-your-own">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Write a properly documented function with the following behaviour:</p>
<ul>
<li>It has a meaningful name (i.e. it is related to its behaviour).</li>
<li>It takes an integer that represents the length of a sequence that will be created.</li>
<li>It creates a dictionary that is empty.</li>
<li>It loops over the sequence and stores each number as the key of an entry in the dictionary, assigning either "odd" or "even" to the value, depending on the type of number.</li>
<li>Returns the dictionary.</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered">
<div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<p><a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Geographic Data Science'15 - Lab 1</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://darribas.org" property="cc:attributionName" rel="cc:attributionURL">Dani Arribas-Bel</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.</p>

</div>
</div>
</div>