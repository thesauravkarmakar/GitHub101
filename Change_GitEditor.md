For many people, the default text editor when using Git from the terminal is VIM. If you ever find yourself with a merge conflict ,
you’ll get kicked out to VIM to fix the conflict and then you’ll need to know the specific VIM commands to edit the doc such commands like i (to edit) 
and :wq (to save and quit). To avoid the inconveniences , you could just change the default text editor which can be done as follows :-

1) Install your desired text editor(such as Microsoft VisualStudio , Atom ,etc) . 
2) Open Terminal.
3)Type this command: $ git config --global core.editor "(editor name , ex : for atom : "atom" , for VisualStudioCode : "code" , etc)  -n -w"


Hope this helps , Happy coding .
