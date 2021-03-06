We must make sure that `&apos;` is always written as `&#39;`.

*** Parameters: ***
{} # params 
*** Markdown input: ***
`<p>here's an apostrophe & a quote "</p>`

	<p>here's an apostrophe & a quote "</p>
{:}

	<p>here's an apostrophe & a quote "</p>
{:lang=xml}

	<p>here's an apostrophe & a quote "</p>
{:html_use_syntax=true lang=not_supported}

	<p>here's an apostrophe & a quote "</p>
{:html_use_syntax=true lang=xml}


*** Output of inspect ***
md_el(:document,[
	md_par([md_code("<p>here's an apostrophe & a quote \"</p>")]),
	md_el(:code,[],{:raw_code=>"<p>here's an apostrophe & a quote \"</p>"},[]),
	md_el(:code,[],{:raw_code=>"<p>here's an apostrophe & a quote \"</p>"},[["lang", "xml"]]),
	md_el(:code,[],{:raw_code=>"<p>here's an apostrophe & a quote \"</p>"},[["html_use_syntax", "true"], ["lang", "not_supported"]]),
	md_el(:code,[],{:raw_code=>"<p>here's an apostrophe & a quote \"</p>"},[["html_use_syntax", "true"], ["lang", "xml"]])
],{},[])
*** Output of to_html ***
<p><code>&lt;p&gt;here's an apostrophe &amp; a quote "&lt;/p&gt;</code></p>

<pre><code>&lt;p&gt;here's an apostrophe &amp; a quote "&lt;/p&gt;</code></pre>

<pre class="xml"><code lang="xml" xml:lang="xml"><span class="punct">&lt;</span><span class="tag">p</span><span class="punct">&gt;</span>here's an apostrophe &amp; a quote "<span class="punct">&lt;/</span><span class="tag">p</span><span class="punct">&gt;</span></code></pre>

<pre class="not_supported"><code lang="not_supported" xml:lang="not_supported">&lt;p&gt;here's an apostrophe &amp; a quote "&lt;/p&gt;</code></pre>

<pre class="xml"><code lang="xml" xml:lang="xml"><span class="punct">&lt;</span><span class="tag">p</span><span class="punct">&gt;</span>here's an apostrophe &amp; a quote "<span class="punct">&lt;/</span><span class="tag">p</span><span class="punct">&gt;</span></code></pre>
*** Output of to_latex ***
{\colorbox[rgb]{1.00,0.93,1.00}{\tt \char60p\char62here\char39s~an~apostrophe~\char38~a~quote~\char34\char60\char47p\char62}}

\begin{verbatim}<p>here's an apostrophe & a quote "</p>\end{verbatim}
\begin{verbatim}<p>here's an apostrophe & a quote "</p>\end{verbatim}
\begin{verbatim}<p>here's an apostrophe & a quote "</p>\end{verbatim}
\begin{verbatim}<p>here's an apostrophe & a quote "</p>\end{verbatim}
*** Output of to_md ***

`<p>here's an apostrophe & a quote "</p>`

     <p>here's an apostrophe & a quote "</p>
{:}

     <p>here's an apostrophe & a quote "</p>
{:lang=xml}

     <p>here's an apostrophe & a quote "</p>
{:html_use_syntax=true lang=not_supported}

     <p>here's an apostrophe & a quote "</p>
{:html_use_syntax=true lang=xml}
*** Output of to_s ***

