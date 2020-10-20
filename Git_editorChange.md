<h3><BOLD>GUIDE : TO CHANGE YOUR GIT EDITOR</h3></BOLD>

<h5>For many people, the default text editor when using Git from the terminal is VIM.
If you ever find yourself with a merge conflict , you’ll get kicked out to VIM to fix the conflict and then you’ll need to know the specific VIM commands 
to edit the doc such commands like i (to edit) and :wq (to save and quit). 

To avoid the inconveniences , you could just change the default text editor which can be done as follows :-</h5>

<h4>1)Install your desired text editor(such as Microsoft VisualStudio , Atom ,etc).

2)Open Terminal.

3)To check your current default editor type :</h4>

<h5>git config --global core.editor </h5>

<p align="center">
<img width="483" alt="Screenshot 2020-10-20 at 10 23 32 AM" src="https://user-images.githubusercontent.com/58665834/96541764-50959a80-12be-11eb-8121-31850b789c2f.png">
</p>

<h4>5) Type this command to use your desired editor for git:</h4>

<h5>$ git config --global core.editor "(editor name , ex : for atom : "atom" , for VisualStudioCode : "code" , etc) -n -w" </h5>

<h4>Type the following to check you new git editor:** git config --global core.editor </h4>

<h5>For example :-</h5>

<p align="center">
<img width="518" alt="Screenshot 2020-10-20 at 10 33 39 AM" src="https://user-images.githubusercontent.com/58665834/96542460-bc2c3780-12bf-11eb-86d7-47ee2899fc00.png">
</p>

<h5>If your desired texteditor appears , you have successfully made it your default Git editor , Congratulations

Hope this helps , Happy coding .</h5>
