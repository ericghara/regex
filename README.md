# regex
This is just an handy place for me to archive regexes I <em>programmed</em>, that might be useful in the future.

<ul>
    <li>A single line consisting only of q, not case sensitive 😛<pre>^[Q|q]$<pre></li>
    <li>Single line hash comment, including leading whitespace<pre>(\b|^)\s*#.*$<pre></li>
    <li>Whitespace not between quotes<pre>\s+(?=([^"]*"[^"]*")*[^"]*$)<pre></li>
    <li>Text between quotes, which begin and end a line<pre>(?<=^").+(?="$)<pre></li>
    <li>Public java methods, w/o dockstrigns and annotations<pre>public.*\{[^}]*\}<pre></li>
    <li>Public java methods, w/ docstrings<pre>/[^/]*/(\n)*[^p]*public.*\{[^}]*\}<pre></li>
    <li>Catch blocks containing the throw keyword<pre>catch[^}]*\sthrow\s[^}]*}<pre></li>
    <li>Specific file extensions in a filepath<pre>(?<=^[^\.].*\.)(reg|exp|rss)$<pre></li>
    <li>SHA1 hash preceded by a file path, that is a child of /aParent/Path<pre>(?<=(/aParent/Path/)(.*\s))[0-9a-fA-F]{40}(?=\b)<pre></li>
</ul>
