# Setting Up Your Git Workspace

This repo is inspired by a free online course from [Udacity](https://www.udacity.com/), How to Use Git and Github by Caroline Buckey and Sarah Spikes.
Check out the course here: [https://www.udacity.com/course/ud775](https://www.udacity.com/course/ud775).
This course was designed as part of a program to help me and others become Front-End Developers. You can check out the full details of the program here:
[https://www.udacity.com/course/nd001](https://www.udacity.com/course/nd001).

If you take your time to configure a few things about Git, it can be much easier and more pleasant to work with. This includes having a colourful custom
prompt that shows the commit that is currently checked out, and if there are any changes in the repo, having tab completion for git commands and
setting your prefered editor for editing commit messages.

### Watch this video from the course

<a href="http://www.youtube.com/watch?feature=player_embedded&v=XPOzPrahXgw" target="_blank">
<img src="http://img.youtube.com/vi/XPOzPrahXgw/0.jpg" alt="Git Workspace" width="320" height="240" border="1" />
</a>

**Disclaimer:** I have made a few personal modifications to these instructions, for the original instructions, please refer to the course on the Udacity website.
(Plus, I included the [videos](./videos) from the course in the repo, just incase they are pulled down in the future)


## Setting Up Your Workspace on Windows

### Download the necessary files

* Download the three files `git-completion.bash`, `git-prompt.sh` and `bash_profile` from the [windows](./windows) folder in this repo, and save
them in your home directory with the same names.
* If you already have a file in your home directory named `.bash_profile`, copy the content from the `bash_profile` file that you
downloaded and paste it at the bottom of your existing `.bash_profile` file. 
Otherwise, rename the `bash_profile` file that you downloaded to `.bash_profile` (with a dot at the beginning) and save it in
your home directory.

(If you're curious to learn more about how bash prompts work, see [this page](https://www.cyberciti.biz/tips/howto-linux-unix-bash-shell-setup-prompt.html).)

### Making Git configurations

Run the following Git configuration commands. The first one will need to be modified if you are using a text editor other than Sublime,
or if Sublime is installed in another location for you.
See [this page](https://help.github.com/articles/associating-text-editors-with-git/) for the correct command for a couple of other popular
text editors.
For any other editor, you'll need to enter the command you use to launch that editor from Git Bash.

```bash
git config --global core.editor "'C:/Program Files/Sublime Text 2/sublime_text.exe' -n -w"
git config --global push.default upstream
git config --global merge.conflictstyle diff3
```

### Make sure you can start your editor from Git Bash

If you use Sublime, you can do this by adding the following line to your `.bash_profile`:

```bash
alias subl="C:/Program\ Files/Sublime\ Text\ 2/sublime_text.exe"
```

### Restart Git Bash

You'll need to close and re-open Git Bash before all your changes take effect.

### Watch this video from the course

<a href="http://www.youtube.com/watch?feature=player_embedded&v=IfLhXM4RnB4" target="_blank">
<img src="http://img.youtube.com/vi/IfLhXM4RnB4/0.jpg" alt="Setting Up Your Workspace on Windows" width="320" height="240" border="1" />
</a>


## Setting Up Your Workspace on Mac and Linux

### Download the necessary files

* Download the three files `git-completion.bash`, `git-prompt.sh` and `bash_profile` from the [mac-or-linux](./mac-or-linux) folder in this repo, and save
them in your home directory with the same names.
* If you already have a file in your home directory named `.bash_profile` on mac (or `.bashrc` on linux), copy the content from the
`bash_profile` file that you downloaded and paste it at the bottom of your existing `.bash_profile` file on mac (or `.bashrc` on linux). 
Otherwise, rename the `bash_profile` file that you downloaded to `.bash_profile` on mac (or `.bashrc` on linux) (with a dot at the beginning)
and save it in your home directory.

(If you're curious to learn more about how bash prompts work, see [this page](https://www.cyberciti.biz/tips/howto-linux-unix-bash-shell-setup-prompt.html).)

### Make sure you can start your editor from the terminal

If you use Sublime, you can do this by adding the following line to your `.bash_profile` on mac (or `.bashrc` on linux)
(you may need to change the path if Sublime is installed in a different location for you):

```bash
alias subl="/Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl"
```

### Making Git configurations

Run the following Git configuration commands. The first one will need to be modified if you are using a text editor other than Sublime,
or if Sublime is installed in another location for you.
See [this page](https://help.github.com/articles/associating-text-editors-with-git/) for the correct command for a couple of other popular
text editors.
For any other editor, you'll need to enter the command you use to launch that editor from Git Bash.

```bash
git config --global core.editor "'/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl' -n -w"
git config --global push.default upstream
git config --global merge.conflictstyle diff3
```

(Instead of the first command, you may be able to use the simpler `git config --global core.editor "subl -n -w"` as shown in the video,
but many students have found this does not work for them.)

### Restart the terminal

You'll need to close and re-open the terminal before all your changes take effect.

### Watch this video from the course

<a href="http://www.youtube.com/watch?feature=player_embedded&v=s_eFuGauy6k" target="_blank">
<img src="http://img.youtube.com/vi/s_eFuGauy6k/0.jpg" alt="Setting Up Your Workspace on Mac" width="320" height="240" border="1" />
</a>


## Acknowledgments

* [Udacity](https://www.udacity.com/)
* Caroline Buckey - [cbuckey-uda](https://github.com/cbuckey-uda)
* Sarah Spikes - [salogel42](https://github.com/salogel42)