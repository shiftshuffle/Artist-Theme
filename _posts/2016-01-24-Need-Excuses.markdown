---
layout: post
title:  "Need Excuses? Try This"
date:   2016-01-24 09:11:03
description: Phasellus hendrerit. Pellent aliquet nibh nec urna. In nis aliquet vel, dapibus id,mattis.
thumbnail: food2.jpg
categories: category1

# Information for the author block
author: Nina Petropoulos
---
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

<div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[2]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-julia"><pre><span class="k">using</span> <span class="n">Requests</span>

<span class="k">function</span><span class="nf"> letmesee</span><span class="p">(</span><span class="n">guess</span><span class="p">::</span><span class="n">String</span><span class="p">)</span>
    <span class="k">if</span> <span class="n">get</span><span class="p">(</span><span class="n">target</span><span class="o">*</span><span class="n">guess</span><span class="p">)</span><span class="o">.</span><span class="n">status</span><span class="o">==</span><span class="mi">404</span>
        <span class="k">return</span> <span class="n">true</span>
        <span class="k">else</span>
            <span class="k">return</span> <span class="n">false</span>
    <span class="k">end</span>
<span class="k">end</span>


<span class="k">function</span><span class="nf"> hex2bin</span><span class="p">(</span><span class="n">s</span><span class="p">::</span><span class="n">ASCIIString</span><span class="p">)</span>
    <span class="n">len</span> <span class="o">=</span> <span class="n">length</span><span class="p">(</span><span class="n">s</span><span class="p">)</span>
    <span class="k">if</span> <span class="n">isodd</span><span class="p">(</span><span class="n">len</span><span class="p">)</span>
        <span class="nb">error</span><span class="p">(</span><span class="s">&quot;Input string length should be even&quot;</span><span class="p">)</span>
    <span class="k">end</span>
    <span class="n">arr</span> <span class="o">=</span> <span class="n">zeros</span><span class="p">(</span><span class="kt">Uint8</span><span class="p">,</span> <span class="n">div</span><span class="p">(</span><span class="n">len</span><span class="p">,</span><span class="mi">2</span><span class="p">))</span>
    <span class="n">i</span> <span class="o">=</span> <span class="n">j</span> <span class="o">=</span> <span class="mi">0</span>
    <span class="k">while</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="n">len</span>
        <span class="n">n</span> <span class="o">=</span> <span class="mi">0</span>
        <span class="n">c</span> <span class="o">=</span> <span class="n">s</span><span class="p">[</span><span class="n">i</span><span class="o">+=</span><span class="mi">1</span><span class="p">]</span>
        <span class="n">n</span> <span class="o">=</span> <span class="sc">&#39;0&#39;</span> <span class="o">&lt;=</span> <span class="n">c</span> <span class="o">&lt;=</span> <span class="sc">&#39;9&#39;</span> <span class="o">?</span> <span class="n">c</span> <span class="o">-</span> <span class="sc">&#39;0&#39;</span> <span class="p">:</span>
            <span class="sc">&#39;a&#39;</span> <span class="o">&lt;=</span> <span class="n">c</span> <span class="o">&lt;=</span> <span class="sc">&#39;f&#39;</span> <span class="o">?</span> <span class="n">c</span> <span class="o">-</span> <span class="sc">&#39;a&#39;</span> <span class="o">+</span> <span class="mi">10</span> <span class="p">:</span>
            <span class="sc">&#39;A&#39;</span> <span class="o">&lt;=</span> <span class="n">c</span> <span class="o">&lt;=</span> <span class="sc">&#39;F&#39;</span> <span class="o">?</span> <span class="n">c</span> <span class="o">-</span> <span class="sc">&#39;A&#39;</span> <span class="o">+</span> <span class="mi">10</span> <span class="p">:</span> <span class="nb">error</span><span class="p">(</span><span class="s">&quot;Input string isn&#39;t a hexadecimal string&quot;</span><span class="p">)</span>
        <span class="n">c</span> <span class="o">=</span> <span class="n">s</span><span class="p">[</span><span class="n">i</span><span class="o">+=</span><span class="mi">1</span><span class="p">]</span>
        <span class="n">n</span> <span class="o">=</span> <span class="sc">&#39;0&#39;</span> <span class="o">&lt;=</span> <span class="n">c</span> <span class="o">&lt;=</span> <span class="sc">&#39;9&#39;</span> <span class="o">?</span> <span class="n">n</span> <span class="o">&lt;&lt;</span> <span class="mi">4</span> <span class="o">+</span> <span class="n">c</span> <span class="o">-</span> <span class="sc">&#39;0&#39;</span> <span class="p">:</span>
            <span class="sc">&#39;a&#39;</span> <span class="o">&lt;=</span> <span class="n">c</span> <span class="o">&lt;=</span> <span class="sc">&#39;f&#39;</span> <span class="o">?</span> <span class="n">n</span> <span class="o">&lt;&lt;</span> <span class="mi">4</span> <span class="o">+</span> <span class="n">c</span> <span class="o">-</span> <span class="sc">&#39;a&#39;</span> <span class="o">+</span> <span class="mi">10</span> <span class="p">:</span>
            <span class="sc">&#39;A&#39;</span> <span class="o">&lt;=</span> <span class="n">c</span> <span class="o">&lt;=</span> <span class="sc">&#39;F&#39;</span> <span class="o">?</span> <span class="n">n</span> <span class="o">&lt;&lt;</span> <span class="mi">4</span> <span class="o">+</span> <span class="n">c</span> <span class="o">-</span> <span class="sc">&#39;A&#39;</span> <span class="o">+</span> <span class="mi">10</span> <span class="p">:</span> <span class="nb">error</span><span class="p">(</span><span class="s">&quot;Input string isn&#39;t a hexadecimal string&quot;</span><span class="p">)</span>
        <span class="n">arr</span><span class="p">[</span><span class="n">j</span><span class="o">+=</span><span class="mi">1</span><span class="p">]</span> <span class="o">=</span> <span class="n">n</span>
    <span class="k">end</span>
    <span class="k">return</span> <span class="n">arr</span>
<span class="k">end</span>

<span class="n">bin2hex</span><span class="p">(</span><span class="n">arr</span><span class="p">::</span><span class="n">Array</span><span class="p">{</span><span class="kt">Uint8</span><span class="p">,</span><span class="mi">1</span><span class="p">})</span> <span class="o">=</span> <span class="n">join</span><span class="p">([</span><span class="n">hex</span><span class="p">(</span><span class="n">i</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span> <span class="k">for</span> <span class="n">i</span> <span class="k">in</span> <span class="n">arr</span><span class="p">])</span>
</pre></div>



<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt output_prompt">Out[2]:</div>

<div class="output_text output_subarea output_execute_result">
<pre>bin2hex (generic function with 1 method)</pre>
</div>


<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[3]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-julia"><pre><span class="n">target</span> <span class="o">=</span> <span class="s">&quot;<a href="http://crypto-class.appspot.com/po?er=&quot;">http://crypto-class.appspot.com/po?er=&quot;</a></span>
<span class="n">crypted</span><span class="o">=</span> <span class="s">&quot;f20bdba6ff29eed7b046d1df9fb7000058b1ffb4210a580f748b4ac714c001bd4a61044426fb515dad3f21f18aa577c0bdf302936266926ff37dbf7035d5eeb4&quot;</span>
<span class="n">data</span><span class="o">=</span><span class="n">hex2bin</span><span class="p">(</span><span class="n">crypted</span><span class="p">)</span>
<span class="n">blocks</span><span class="o">=</span><span class="n">Array</span><span class="p">[]</span>
<span class="n">clair</span><span class="o">=</span><span class="p">[</span><span class="kt">Uint8</span><span class="p">[]</span> <span class="k">for</span> <span class="n">i</span><span class="o">=</span><span class="mi">1</span><span class="p">:</span><span class="mi">3</span><span class="p">]</span></p>

<p><span class="k">for</span> <span class="n">i</span><span class="o">=</span><span class="mi">1</span><span class="p">:</span><span class="n">int</span><span class="p">(</span><span class="n">length</span><span class="p">(</span><span class="n">data</span><span class="p">)</span><span class="o">/</span><span class="mi">16</span><span class="p">)</span>
    <span class="n">push</span><span class="o">!</span><span class="p">(</span><span class="n">blocks</span><span class="p">,</span><span class="n">data</span><span class="p">[(</span><span class="n">i</span><span class="o">-</span><span class="mi">1</span><span class="p">)</span><span class="o"><em></span><span class="mi">16</span><span class="o">+</span><span class="mi">1</span><span class="p">:(</span><span class="n">i</span><span class="o">-</span><span class="mi">1</span><span class="p">)</span><span class="o"></em></span><span class="mi">16</span><span class="o">+</span><span class="mi">16</span><span class="p">])</span>
<span class="k">end</span></p>

<p><span class="k">for</span> <span class="n">h</span><span class="o">=</span><span class="mi">1</span><span class="p">:</span><span class="mi">3</span>
    <span class="n">pad</span><span class="o">=</span><span class="nb">convert</span><span class="p">(</span><span class="kt">Uint8</span><span class="p">,</span><span class="mi">1</span><span class="p">)</span>
    <span class="n">block</span><span class="o">=</span><span class="kt">Uint8</span><span class="p">[</span><span class="n">i</span> <span class="k">for</span> <span class="n">i</span> <span class="k">in</span> <span class="n">blocks</span><span class="p">[</span><span class="n">h</span><span class="p">]]</span>
    <span class="n">block</span><span class="p">[</span><span class="k">end</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">=</span><span class="n">block</span><span class="p">[</span><span class="k">end</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">$</span><span class="mi">1</span></p>

<p><span class="k">for</span> <span class="n">i</span><span class="o">=</span><span class="mi">0</span><span class="p">:</span><span class="mi">255</span>
<span class="n">g</span><span class="o">=</span><span class="nb">convert</span><span class="p">(</span><span class="kt">Uint8</span><span class="p">,</span><span class="n">i</span><span class="p">)</span>
<span class="n">block</span><span class="p">[</span><span class="k">end</span><span class="p">]</span><span class="o">=</span><span class="n">blocks</span><span class="p">[</span><span class="n">h</span><span class="p">][</span><span class="k">end</span><span class="p">]</span><span class="o">$</span><span class="n">g</span><span class="o">$</span><span class="n">pad</span>
<span class="n">guess</span><span class="o">=</span><span class="n">bin2hex</span><span class="p">(</span><span class="n">block</span><span class="p">)</span><span class="o">*</span><span class="n">bin2hex</span><span class="p">(</span><span class="n">blocks</span><span class="p">[</span><span class="n">h</span><span class="o">+</span><span class="mi">1</span><span class="p">])</span>
<span class="k">if</span> <span class="n">letmesee</span><span class="p">(</span><span class="n">guess</span><span class="p">)</span>
     <span class="n">println</span><span class="p">(</span><span class="n">char</span><span class="p">(</span><span class="n">g</span><span class="p">))</span>
    <span class="n">push</span><span class="o">!</span><span class="p">(</span><span class="n">clair</span><span class="p">[</span><span class="n">h</span><span class="p">],</span><span class="n">g</span><span class="p">)</span>
    <span class="k">break</span>
<span class="k">end</span>
<span class="k">end</span></p>

<p><span class="k">for</span> <span class="n">k</span><span class="o">=</span><span class="mi">2</span><span class="p">:</span><span class="mi">16</span>
<span class="n">pad</span><span class="o">=</span><span class="nb">convert</span><span class="p">(</span><span class="kt">Uint8</span><span class="p">,</span><span class="n">k</span><span class="p">)</span>
<span class="n">block</span><span class="o">=</span><span class="kt">Uint8</span><span class="p">[</span><span class="n">i</span> <span class="k">for</span> <span class="n">i</span> <span class="k">in</span> <span class="n">blocks</span><span class="p">[</span><span class="n">h</span><span class="p">]]</span></p>

<p><span class="k">for</span> <span class="n">j</span><span class="o">=</span><span class="mi">1</span><span class="p">:</span><span class="n">k</span><span class="o">-</span><span class="mi">1</span>
    <span class="n">block</span><span class="p">[</span><span class="k">end</span><span class="o">-</span><span class="n">j</span><span class="o">+</span><span class="mi">1</span><span class="p">]</span><span class="o">=</span><span class="n">block</span><span class="p">[</span><span class="k">end</span><span class="o">-</span><span class="n">j</span><span class="o">+</span><span class="mi">1</span><span class="p">]</span><span class="o">$</span><span class="n">clair</span><span class="p">[</span><span class="n">h</span><span class="p">][</span><span class="n">j</span><span class="p">]</span><span class="o">$</span><span class="n">pad</span>
<span class="k">end</span></p>

<p><span class="k">for</span> <span class="n">i</span><span class="o">=</span><span class="mi">0</span><span class="p">:</span><span class="mi">255</span>
    <span class="n">g</span><span class="o">=</span><span class="nb">convert</span><span class="p">(</span><span class="kt">Uint8</span><span class="p">,</span><span class="n">i</span><span class="p">)</span>
    <span class="n">block</span><span class="p">[</span><span class="k">end</span><span class="o">-</span><span class="n">k</span><span class="o">+</span><span class="mi">1</span><span class="p">]</span><span class="o">=</span><span class="n">blocks</span><span class="p">[</span><span class="n">h</span><span class="p">][</span><span class="k">end</span><span class="o">-</span><span class="n">k</span><span class="o">+</span><span class="mi">1</span><span class="p">]</span><span class="o">$</span><span class="n">g</span><span class="o">$</span><span class="n">pad</span>
    <span class="n">guess</span><span class="o">=</span><span class="n">bin2hex</span><span class="p">(</span><span class="n">block</span><span class="p">)</span><span class="o">*</span><span class="n">bin2hex</span><span class="p">(</span><span class="n">blocks</span><span class="p">[</span><span class="n">h</span><span class="o">+</span><span class="mi">1</span><span class="p">])</span>
    <span class="k">if</span> <span class="n">letmesee</span><span class="p">(</span><span class="n">guess</span><span class="p">)</span>
         <span class="c">#println(char(g))</span>
        <span class="n">push</span><span class="o">!</span><span class="p">(</span><span class="n">clair</span><span class="p">[</span><span class="n">h</span><span class="p">],</span><span class="n">g</span><span class="p">)</span>
        <span class="k">break</span>
    <span class="k">end</span>
<span class="k">end</span>
<span class="k">end</span>
<span class="k">end</span></p>

<p><span class="n">println</span><span class="p">(</span><span class="n">clair</span><span class="p">)</span></p>

<p><span class="n">reverse</span><span class="p">(</span><span class="n">join</span><span class="p">(</span><span class="n">map</span><span class="p">(</span><span class="n">char</span><span class="p">,</span><span class="n">clair</span><span class="p">[</span><span class="mi">1</span><span class="p">])))</span><span class="o"><em></span><span class="n">reverse</span><span class="p">(</span><span class="n">join</span><span class="p">(</span><span class="n">map</span><span class="p">(</span><span class="n">char</span><span class="p">,</span><span class="n">clair</span><span class="p">[</span><span class="mi">2</span><span class="p">])))</span><span class="o"></em></span><span class="n">reverse</span><span class="p">(</span><span class="n">join</span><span class="p">(</span><span class="n">map</span><span class="p">(</span><span class="n">char</span><span class="p">,</span><span class="n">clair</span><span class="p">[</span><span class="mi">3</span><span class="p">])))</span>
</pre></div></p>



<div class="output_wrapper">
<div class="output">


<div class="output_area"><div class="prompt"></div>
<div class="output_subarea output_stream output_stdout output_text">
<pre>
s

[Uint8[32,115,100,114,111,87,32,99,105,103,97,77,32,101,104,84],Uint8[115,79,32,104,115,105,109,97,101,117,113,83,32,101,114,97],Uint8[9,9,9,9,9,9,9,9,9,101,103,97,114,102,105,115]]
</pre>
</div>
</div>

<div class="output_area"><div class="prompt output_prompt">Out[3]:</div>

<div class="output_text output_subarea output_execute_result">
<pre>&quot;The Magic Words are Squeamish Ossifrage\t\t\t\t\t\t\t\t\t&quot;</pre>
</div>
