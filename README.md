# agnoster-bash-color
This configuration of agnoster theme is used to have history line, time and username in different colors. There is two available configurations: **random colors** and **fixed colors**. Choose the one you prefer. :cupid:

### Prerequisites

[Oh-My-Bash](https://ohmybash.nntoan.com/) and [Agnoster theme](https://github.com/ohmybash/oh-my-bash/wiki/Themes) installed


## Script 1 ~ random colors

This configuration is aimed to have changing colors every time the user enters a command in the terminal.

<img src="https://github.com/manialinux/agnoster-bash-color/blob/main/agnoster-bash-random-color.png" alt="drawing" width="500"/>

All you have to do is replace your configuration file of agnoster theme (which should be located at `~.oh-my-bash/themes/agnoster/agnoster.theme.sh` ) by the content of [theme1.sh](https://github.com/manialinux/agnoster-bash-color/blob/main/theme-random-color.sh).


## Script 2 ~ fixed colors 

This configuration enables to have fixed colors in terminal.

<img src="https://github.com/manialinux/agnoster-bash-color/blob/main/agnoster-bash-fixed-color.png" alt="drawing" width="500"/>

In your configuration file of agnoster theme (which should be located at `~.oh-my-bash/themes/agnoster/agnoster.theme.sh`):

<ul>
  <li>Add the two news functions `prompt_historyline()` and `prompt_time()` from [theme-fixed-color](https://github.com/manialinux/agnoster-bash-color/blob/main/theme-fixed-color.sh) to your config file.</li>
  <li>Use the two others functions `prompt_context()` and `build_prompt()` to replace already existing functions in your configuration file.</li>
</ul>


#### Optional

You can change colors in the configuration file as you wish, as following: `prompt_segment colorBackground colorForeground`

### In any case, don't forget to update config file with the command 
`source .bashrc`
