---
layout: post
title:  "You Need Ten Posts"
date:   2017-03-03 09:11:03
description: Phasellus hendrerit. Pellent aliquet nibh nec urna. In nis aliquet vel, dapibus id,mattis.
thumbnail: food1.jpg
categories: crypto

# Information for the author block
author: shiftshuffle
---



Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut [enim ad minim][link1] veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.


<div tabindex="-1" id="notebook" class="border-box-sizing">
  <div class="container" id="notebook-container">

<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[2]:</div>
<div class="inner_cell">
  <div class="input_area">
<div class=" highlight hl-julia"><pre><span></span><span class="k">using</span> <span class="n">Graphs</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[3]:</div>
<div class="inner_cell">
  <div class="input_area">
<div class=" highlight hl-julia"><pre><span></span><span class="n">m2</span><span class="o">=</span><span class="p">[]</span>
<span class="k">for</span> <span class="n">i</span><span class="o">=</span><span class="mi">1</span><span class="p">:</span><span class="mi">125</span>
  <span class="n">push!</span><span class="p">(</span><span class="n">m2</span><span class="p">,(((</span><span class="n">i</span><span class="o">-</span><span class="mi">1</span><span class="p">)</span><span class="n">÷5</span><span class="p">)</span><span class="o">+</span><span class="mi">1</span><span class="p">,(</span><span class="n">i</span><span class="o">-</span><span class="mi">1</span><span class="p">)</span><span class="o">%</span><span class="mi">25</span><span class="o">+</span><span class="mi">1</span><span class="p">))</span>
<span class="k">end</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[4]:</div>
<div class="inner_cell">
  <div class="input_area">
<div class=" highlight hl-julia"><pre><span></span><span class="n">base5</span> <span class="o">=</span> <span class="p">[</span><span class="s">&quot;RR&quot;</span><span class="p">,</span>
       <span class="s">&quot;RV&quot;</span><span class="p">,</span>
       <span class="s">&quot;RB&quot;</span><span class="p">,</span>
       <span class="s">&quot;RJ&quot;</span><span class="p">,</span>
       <span class="s">&quot;RN&quot;</span><span class="p">,</span>
       <span class="s">&quot;VR&quot;</span><span class="p">,</span>
       <span class="s">&quot;VV&quot;</span><span class="p">,</span>
       <span class="s">&quot;VB&quot;</span><span class="p">,</span>
       <span class="s">&quot;VJ&quot;</span><span class="p">,</span>
       <span class="s">&quot;VN&quot;</span><span class="p">,</span>
       <span class="s">&quot;BR&quot;</span><span class="p">,</span>
       <span class="s">&quot;BV&quot;</span><span class="p">,</span>
       <span class="s">&quot;BB&quot;</span><span class="p">,</span>
       <span class="s">&quot;BJ&quot;</span><span class="p">,</span>
       <span class="s">&quot;BN&quot;</span><span class="p">,</span>
       <span class="s">&quot;JR&quot;</span><span class="p">,</span>
       <span class="s">&quot;JV&quot;</span><span class="p">,</span>
       <span class="s">&quot;JB&quot;</span><span class="p">,</span>
       <span class="s">&quot;JJ&quot;</span><span class="p">,</span>
       <span class="s">&quot;JN&quot;</span><span class="p">,</span>
       <span class="s">&quot;NR&quot;</span><span class="p">,</span>
       <span class="s">&quot;NV&quot;</span><span class="p">,</span>
       <span class="s">&quot;NB&quot;</span><span class="p">,</span>
       <span class="s">&quot;NJ&quot;</span><span class="p">,</span>
       <span class="s">&quot;NN&quot;</span><span class="p">];</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[5]:</div>
<div class="inner_cell">
  <div class="input_area">
<div class=" highlight hl-julia"><pre><span></span><span class="k">using</span> <span class="n">Graphs</span>

<span class="n">g</span> <span class="o">=</span> <span class="n">simple_graph</span><span class="p">(</span><span class="n">length</span><span class="p">(</span><span class="n">base5</span><span class="p">))</span>

<span class="k">for</span> <span class="n">i</span> <span class="k">in</span> <span class="n">m2</span>
  <span class="n">add_edge!</span><span class="p">(</span><span class="n">g</span><span class="p">,</span> <span class="n">i</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">i</span><span class="p">[</span><span class="mi">2</span><span class="p">])</span>
<span class="k">end</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[6]:</div>
<div class="inner_cell">
  <div class="input_area">
<div class=" highlight hl-julia"><pre><span></span><span class="n">v</span><span class="o">=</span><span class="mi">1</span><span class="p">;</span>
<span class="n">queue</span><span class="o">=</span><span class="p">[];</span>
<span class="n">circuit</span><span class="o">=</span><span class="p">[];</span>
<span class="n">possible</span><span class="o">=</span><span class="p">[];</span>
<span class="n">edgecolormap</span> <span class="o">=</span> <span class="n">zeros</span><span class="p">(</span><span class="kt">Int</span><span class="p">,</span> <span class="n">num_edges</span><span class="p">(</span><span class="n">g</span><span class="p">));</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[7]:</div>
<div class="inner_cell">
  <div class="input_area">
<div class=" highlight hl-julia"><pre><span></span><span class="k">for</span> <span class="n">i</span> <span class="k">in</span> <span class="n">out_edges</span><span class="p">(</span><span class="n">v</span><span class="p">,</span> <span class="n">g</span><span class="p">)</span>
  <span class="k">if</span> <span class="n">edgecolormap</span><span class="p">[</span><span class="n">edge_index</span><span class="p">(</span><span class="n">i</span><span class="p">,</span> <span class="n">g</span><span class="p">)]</span><span class="o">==</span><span class="mi">0</span>
      <span class="n">push!</span><span class="p">(</span><span class="n">possible</span><span class="p">,</span><span class="n">i</span><span class="p">)</span>
  <span class="k">end</span>
<span class="k">end</span>

<span class="n">push!</span><span class="p">(</span><span class="n">queue</span><span class="p">,</span><span class="n">v</span><span class="p">)</span>
<span class="n">v_edge</span> <span class="o">=</span> <span class="n">possible</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
<span class="n">v</span> <span class="o">=</span> <span class="n">v_edge</span><span class="o">.</span><span class="n">target</span>
<span class="n">e_color</span> <span class="o">=</span> <span class="n">edgecolormap</span><span class="p">[</span><span class="n">edge_index</span><span class="p">(</span><span class="n">v_edge</span><span class="p">,</span> <span class="n">g</span><span class="p">)]</span>

<span class="k">if</span> <span class="n">e_color</span> <span class="o">==</span> <span class="mi">0</span>
  <span class="n">edgecolormap</span><span class="p">[</span><span class="n">edge_index</span><span class="p">(</span><span class="n">v_edge</span><span class="p">,</span> <span class="n">g</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">1</span>
<span class="k">end</span>




<span class="k">while</span> <span class="o">!</span><span class="n">isempty</span><span class="p">(</span><span class="n">queue</span><span class="p">)</span>

  <span class="n">possible</span><span class="o">=</span><span class="p">[]</span>
  <span class="k">for</span> <span class="n">i</span> <span class="k">in</span> <span class="n">out_edges</span><span class="p">(</span><span class="n">v</span><span class="p">,</span> <span class="n">g</span><span class="p">)</span>
      <span class="k">if</span> <span class="n">edgecolormap</span><span class="p">[</span><span class="n">edge_index</span><span class="p">(</span><span class="n">i</span><span class="p">,</span> <span class="n">g</span><span class="p">)]</span><span class="o">==</span><span class="mi">0</span>
          <span class="n">push!</span><span class="p">(</span><span class="n">possible</span><span class="p">,</span><span class="n">i</span><span class="p">)</span>
      <span class="k">end</span>
  <span class="k">end</span>

  <span class="k">if</span> <span class="o">!</span><span class="n">isempty</span><span class="p">(</span><span class="n">possible</span><span class="p">)</span>
      <span class="n">push!</span><span class="p">(</span><span class="n">queue</span><span class="p">,</span><span class="n">v</span><span class="p">)</span>
      <span class="n">v_edge</span> <span class="o">=</span> <span class="n">possible</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
      <span class="n">v</span> <span class="o">=</span> <span class="n">v_edge</span><span class="o">.</span><span class="n">target</span>
      <span class="n">e_color</span> <span class="o">=</span> <span class="n">edgecolormap</span><span class="p">[</span><span class="n">edge_index</span><span class="p">(</span><span class="n">v_edge</span><span class="p">,</span> <span class="n">g</span><span class="p">)]</span>

      <span class="k">if</span> <span class="n">e_color</span> <span class="o">==</span> <span class="mi">0</span>
          <span class="n">edgecolormap</span><span class="p">[</span><span class="n">edge_index</span><span class="p">(</span><span class="n">v_edge</span><span class="p">,</span> <span class="n">g</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">1</span>
      <span class="k">end</span>


  <span class="k">elseif</span> <span class="n">isempty</span><span class="p">(</span><span class="n">possible</span><span class="p">)</span>
          <span class="n">push!</span><span class="p">(</span><span class="n">circuit</span><span class="p">,</span><span class="n">v</span><span class="p">)</span>
          <span class="n">v</span><span class="o">=</span><span class="n">pop!</span><span class="p">(</span><span class="n">queue</span><span class="p">)</span>
  <span class="k">end</span>

<span class="k">end</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[8]:</div>
<div class="inner_cell">
  <div class="input_area">
<div class=" highlight hl-julia"><pre><span></span><span class="n">u</span><span class="o">=</span><span class="p">[</span><span class="n">base5</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="k">for</span> <span class="n">i</span> <span class="k">in</span> <span class="n">reverse</span><span class="p">(</span><span class="n">circuit</span><span class="p">)</span> <span class="p">]</span>
<span class="n">u2</span><span class="o">=</span><span class="p">[</span><span class="n">i</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="k">for</span> <span class="n">i</span> <span class="k">in</span> <span class="n">u</span><span class="p">]</span>


<span class="n">println</span><span class="p">(</span><span class="n">join</span><span class="p">(</span><span class="n">u</span><span class="p">,</span> <span class="s">&quot;-&gt;&quot;</span><span class="p">))</span>
<span class="n">println</span><span class="p">(</span><span class="s">&quot;</span><span class="se">\n</span><span class="s">&quot;</span><span class="p">)</span>
<span class="n">println</span><span class="p">(</span><span class="n">join</span><span class="p">(</span><span class="n">u2</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>RR-&gt;RV-&gt;VR-&gt;RR-&gt;RB-&gt;BR-&gt;RR-&gt;RJ-&gt;JR-&gt;RR-&gt;RN-&gt;NR-&gt;RV-&gt;VV-&gt;VR-&gt;RV-&gt;VB-&gt;BR-&gt;RV-&gt;VJ-&gt;JR-&gt;RV-&gt;VN-&gt;NR-&gt;RB-&gt;BV-&gt;VR-&gt;RB-&gt;BB-&gt;BR-&gt;RB-&gt;BJ-&gt;JR-&gt;RB-&gt;BN-&gt;NR-&gt;RJ-&gt;JV-&gt;VR-&gt;RJ-&gt;JB-&gt;BR-&gt;RJ-&gt;JJ-&gt;JR-&gt;RJ-&gt;JN-&gt;NR-&gt;RN-&gt;NV-&gt;VR-&gt;RN-&gt;NB-&gt;BR-&gt;RN-&gt;NJ-&gt;JR-&gt;RN-&gt;NN-&gt;NV-&gt;VV-&gt;VV-&gt;VB-&gt;BV-&gt;VV-&gt;VJ-&gt;JV-&gt;VV-&gt;VN-&gt;NV-&gt;VB-&gt;BB-&gt;BV-&gt;VB-&gt;BJ-&gt;JV-&gt;VB-&gt;BN-&gt;NV-&gt;VJ-&gt;JB-&gt;BV-&gt;VJ-&gt;JJ-&gt;JV-&gt;VJ-&gt;JN-&gt;NV-&gt;VN-&gt;NB-&gt;BV-&gt;VN-&gt;NJ-&gt;JV-&gt;VN-&gt;NN-&gt;NB-&gt;BB-&gt;BB-&gt;BJ-&gt;JB-&gt;BB-&gt;BN-&gt;NB-&gt;BJ-&gt;JJ-&gt;JB-&gt;BJ-&gt;JN-&gt;NB-&gt;BN-&gt;NJ-&gt;JB-&gt;BN-&gt;NN-&gt;NJ-&gt;JJ-&gt;JJ-&gt;JN-&gt;NJ-&gt;JN-&gt;NN-&gt;NN-&gt;NR-&gt;RR


RVRRBRRJRRNRVVRVBRVJRVNRBVRBBRBJRBNRJVRJBRJJRJNRNVRNBRNJRNNVVVBVVJVVNVBBVBJVBNVJBVJJVJNVNBVNJVNNBBBJBBNBJJBJNBNJBNNJJJNJNNNRR
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
<p><a href="http://graphsjl-docs.readthedocs.io/en/latest/algorithms.html#graph-traversal">graphs.jl</a></p>
<p><a href="http://www.geeksforgeeks.org/hierholzers-algorithm-directed-graph/">hierholzer</a></p>
<p><a href="http://www.graph-magics.com/articles/euler.php">euler cycle</a></p>
<p><a href="https://www.youtube.com/watch?v=_x4IVlsw_q4">video euler cycle</a></p>

</div>
</div>
</div>
  </div>
</div>
