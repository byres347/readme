# remove all '  my = "";'
:%s/  my  = "";// 

# add at the end of line 67 to line 107
:67, 101norm A = "";
:67, 101s/$/ = "";

# Moving to matching braces
%

# search
https://www.cs.swarthmore.edu/oldhelp/vim/searching.html

# indenting to convert tab to space (adding in .vimrc)  
https://www.cs.swarthmore.edu/oldhelp/vim/indenting.html
set tabstop=4  
set expandtab  
set shiftwidth=4  
set shiftround  

# copy & paste
https://blog.csdn.net/dongdongnihao_/article/details/103624021
goto visual mode: ^v
begging of line: 0
end of line: $
copy: y
cut: d
exit visual mode: Esc
paste: p
selects entire lines: V  
selects range of text: v  

# binary view
%! xxd

# add xxx in each beginning of line
:%s/^/xxx

# add xxx in each end of line
:%s/$/xxx

# remove lines with xxx keywords in gvim
:g/xxx/d

# unknown command
:echo expand('%:p')
:echo @%

# add banner
1) type 30
2) press i
3) press =
4) press esc

insert mode  
I: begin of line  
A: end of line  

normal mode  
0: move cursor to begin of line  
$: move cursor to end of line
