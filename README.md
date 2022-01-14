# regex
A collection of regular expressions that I may or may not have spent a few minutes <i>programming</i>.

<ul>
    <li>A single line consisting only of d, not case sensitive<pre>^[D|d]$<pre></li>
    <li>Single line hash comment, including leading whitespace<pre>(\b|^)\s*#.*$<pre></li>
    <li>Whitespace not between quotes<pre>\s+(?=([^"]*"[^"]*")*[^"]*$)<pre></li>
    <li>Text between quotes, which begin and end a line<pre>(?<=^").+(?="$)<pre></li>
    <li>Public java methods, w/o dockstrigns and annotations<pre>public.*\{[^}]*\}<pre></li>
    <li>Public java methods, w/ docstrings<pre>/[^/]*/(\n)*[^p]*public.*\{[^}]*\}<pre></li>
    <li>Specific file extensions in a filepath<pre>(?<=^[^\.].*\.)(reg|exp|rss)$<pre></li>
</ul>
