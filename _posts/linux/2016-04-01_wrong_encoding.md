
#诡异的shell乱码： 文件encoding 正确(utf-8), export LANG="utf-8" 正确， xshell 的 encoding 设置正确 "utf-8" ，但直接往控制台输入中文仍然会乱码

<pre><code>
[awen@localhost data]$ php -r 'echo "????";'
????[awen@localhost data]$ 
[awen@localhost data]$ 
[awen@localhost data]$ php -r 'echo "使用说明";'
使用说明[awen@localhost data]$ 
[awen@localhost data]$ 
[awen@localhost data]$ vim abc.txt
[awen@localhost data]$ cat abc.txt 
echo "使用说明";'
[awen@localhost data]$ 
</code></pre>
