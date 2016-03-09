# ifmicro-configs


Writed in 2015-11-11 by MwumLi

----

Share my some softwares configurations


## shell

1. `.myshelrc` -- my shell configurations  
    For bash :  

        cp .myshelrc ~/ && echo 'source ~/.myshellrc' >> ~/.bashrc 

    For zsh :  

        cp .myshelrc ~/ && echo 'source ~/.myshellrc' >> ~/.zshrc

## tmux

1. `.tmux.conf` -- my tmux configurations  
   

        cp .tmux.conf ~/

    enable tmux 256 color : `alias tmux='tmux -2'`  

## oh-my-zsh

### Installation

zsh is very strong, but it's hard to configure it  
Fortunately, we have the oh-my-zsh  

[oh-my-zsh][] is a customized solution of zsh configuration, which is modular  
Only few steps, your will own a beautiful teriminal

[oh-my-zsh][] project: <https://github.com/robbyrussell/oh-my-zsh>  

After installation, oh-my-zsh will generate a new `.zshrc` instead of old `~/.zshrc`

### Change Theme `trapd00r`

There is a default theme `robbyrussell` in `~/.zshrc`  
But it's so simple that you could not like it(At least I don't like)

There are many themes in `~/.oh-my-zsh/themes/` , so you can take your pick  

I prefer `~/.oh-my-zsh/themes/trapd00r.zsh-theme` , do below :  

1. in `~/.zshrc` :  

        ZSH_THEME="trapd00r"

2. move `zsh_path` to bin PATH :  

        mv zsh_path /bin/

3. 下载、编译和安装[Term-ExtendedColor-0.224.tar.gz][] :  

        wget http://search.cpan.org/CPAN/authors/id/W/WO/WOLDRICH/Term-ExtendedColor-0.224.tar.gz
        tar xvzf Term-ExtendedColor-0.224.tar.gz
        cd Term-ExtendedColor-0.224  && perl Makefile.PL && sudo make install


The source address of `zsh_path` : <https://raw.githubusercontent.com/trapd00r/utils/master/zsh_path>  
Notice :  
> Here's `zsh_path` has been modify by me, because the ugly color  not match my teriminal color scheme  
> `zsh_path` is a perl script, which used to show a split path for current path  
> So, you can replace it by your own program  

[oh-my-zsh]: https://github.com/robbyrussell/oh-my-zsh "oh-my-zsh Github 地址"  
[Term-ExtendedColor-0.224.tar.gz]: http://search.cpan.org/CPAN/authors/id/W/WO/WOLDRICH/Term-ExtendedColor-0.224.tar.gz

## SSH

add my ssh keys and encrypt it

## man page

### Highlight

Two method to highlight man page  :

1. `man [command]` : change colorscheme to highlight man page  
2. `vman [comman]` : open man page by vim's readonly mode

### Installation

Man manual has been installed in Ubuntu by default  
If not installed in your os or update your man page, you can :  

    $ git clone http://git.kernel.org/pub/scm/docs/man-pages/man-pages
    $ cd man-pages && sudo make

### Reference

1. [man page](http://www.dreamxu.com/books/osg/linux/man-page.html)
2. [Download Page](https://www.kernel.org/doc/man-pages/download.html)  
3. [Github Project](https://github.com/mkerrisk/man-pages)  

