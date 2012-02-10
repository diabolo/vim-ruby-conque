# vim-ruby-conque.vim

## fork details

forked from skwp/vim-ruby-conque. This supports my way of using Cucumber
(using @wip)

## blurb
 
 * Colorized ruby, rake, and rspec output in vim using ConqueTerm
 * Dead simple -  ~20 lines of code
 * Sensible keybindings (feel free to change):
    * <code>nmap <silent> <Leader>rr :call RunRubyCurrentFileConque()<CR> </code>
    * <code>nmap <silent> <Leader>ss :call RunRspecCurrentFileConque()<CR></code>
    * <code>nmap <silent> <Leader>ll :call RunRspecCurrentLineConque()<CR></code>
    * <code>nmap <silent> <Leader>RR :call RunRakeConque()<CR></code>

 * Requires: http://code.google.com/p/conque/

 * Install: copy plugin/* to ~/.vim/plugin or if using pathogen, 
   copy the whole directroy to ~/.vim/bundle

## configuration

This plugin tries to detect whether you use 'rspec' (rspec2) or 'spec'
(rspec1) and set the default executable correctly. To override in your
~/.vimrc:

    let g:ruby_conque_rspec_command='spec'

