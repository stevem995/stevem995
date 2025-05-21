<div class="AutomationGallery"

<img src="images/DevOpsMLOpsWelders150by150.png" alt="Two welders
    welding metal together.">
<p>Automation Means: Work Smarter, Not Harder! (picture is AI generated)</p>
</div>

## Table of Contents

   - [WHO AM I](#who-am-i)
   - [Current Projects](#current-projects)
   - [Current state of affairs](#current-state-of-affairs)
   - [Automation Tips and Tricks](#automation-tips-and-tricks)
     - [Emacs Tips](#emacs-tips)
        - [Emacs Go Print Function](#emacs-go-print-function)
        - [Emacs Python3 Print Function](#emacs-python3-print-function)
        - [Emacs Powershell Print Function](#emacs-powershell-print-function)
     - [Automation Windows](#automation-windows)
       - [Automation Windows ShortPath](#automation-windows-shortpath)
   - [Workstation Tips and Tricks](#automation-tips-and-tricks)
     - [Windows Tips](#windows-tips)
        - [Git Bash Prompt and Title](#git-bash-prompt-and-title)


## WHO AM I

Automation enthusiast and DevOps engineer.


## Current Projects

    TBD

## Current state of affairs

Here are some ideas to get you started:

- 🔭 I’m currently working on ...

     My future, finding a new position, and engineering projects.

- 🕮 I’m currently learning ...

    MLOps and breaking into the AI scene using MLFlow and Hugging Face.

    Portfolio for employers.

    Riemann Hypothesis: I'm reading Prime Obsession by John
    Derbyshire. At this point, trying to grasp operators and their
    linked Hermitian matrixes.

    Non-conforming parcels of land and what you need to go through with a
    zoning board. 🤦


## Automation Tips and Tricks

###  Emacs Tips

### [Emacs Go Print Function](#emacs-go-print-function)

```
; Description: Creates an interactive Emacs GO function which which creates a
; GO styled print statement and places the cursor accordingly.
; Example: fmt.Println("")
; Usage: M-x goprin
; Installation: Place this in your .emacs file.

(defun goprin ()
  "defalias pyprin: Insert go print skeleton"
  (interactive)
  (insert "fmt.Println\(\"\"\)")
  (backward-char 2))
```

### [Emacs Python3 Print Function](#emacs-python3-print-function)

```
; Description: Creates an interactive Emacs Python print function which which creates a
; python3 styled print statement and places the cursor accordingly.
; Example: print("{}".format())
; Usage: M-x pyprin
; Installation: Place this in your .emacs file.

(defun pyprin ()
  "defalias pyprin: Insert python print skeleton"
  (interactive)
  (insert "print\(\"\{\}\".format\(\)\)")
  (backward-char 13))
```

### [Emacs Powershell Print Function](#emacs-powershell-print-function)

```
; Description: Creates an interactive Emacs Powershell print function which which creates a
; Powershell styled print statement and places the cursor accordingly.
; Example: Write-Host ("{0}" -f )
; Usage: M-x pyprin
; Installation: Place this in your .emacs file.

(defun psprin ()
  "defalias psprin: Insert powershell print skeleton"
  (interactive)
  (insert "Write-Host \(\"\{0\}\" -f \)")
  (backward-char 9))
```

### Automation Windows

Simple automation on windows is a bit tricky. This is especially true
if you use Linux like programs such as git bash where the difference
become stark. Paths to not interpret correctly, etc.

### [Automation Windows ShortPath](#automation-windows-shortpath)


In order to set up aliases in Git-Bash to work correctly, you must use
the windows shortpath which is the fully qualified or absolute path.
There are several way to do this. The easiest is to use a script that
can print out the current path as a short path.

shortpath.cmd
```
:: Display the short path of current directory.
@ECHO OFF
if '%1'=='' (%0 .) else echo %~s1
```

You can then use that path in an alias
```
OPEN_OFFICE_WRITER="C:/PROGRA~2/OPENOF~1/program/swriter.exe "

alias resume='${OPEN_OFFICE_WRITER} my-resume.odt &'
```

### Workstation Tips and Tricks

### Windows Tips

Windows Tips focus on windows desktop tool customizations. This
includes changing prompts or removing your username from view.

### [Git Bash Prompt and Title](#git-bash-prompt-and-title)

To customize the Git Bash prompt you must find and modify the
git-prompt\.sh file(NOTE: this file cannot be modified from within
git-bash while it is running. Use an outside editor).

```
1. To find where git-prompt is installed open the Git Bash app's
   properties. This is buried by Microsoft for some unknown reason.
   The easiest way to find it is to add the app to the task bar. From
   there, you can right click for the properties menu.
   1. Open the start menu and search for Git Bash.
   2. Right click the icon and pin it to the task bar.
   3. Right click the Git Bash icon on the task bar.
   4. Right click the Git Bash icon in the menu
   5. select properties.
   6. Note the path, this is where git-prompt.sh is installed.
   7. git-prompt.sh is usually found in etc/profile.d subdirectory
2. Edit the git-prompt.sh file's PS1 variable commenting and removing
   lines as needed e.g:

    PS1='\[\033]0;\h:$PWD\007\]' # set window title
    PS1="$PS1"'\[\033[32m\]'       # change to green
    PS1="$PS1"'\h [\D{%m/%d/%g:%I:%M:%S:%p]}'  # host<space>Time stamp
    PS1="$PS1"'\[\033[0m\]'        # change color
    PS1="$PS1"': '                 # prompt: always : at end.


```

<div align="center">
  <p>Visitor count</p>
  <img src="https://profile-counter.glitch.me/stevem995/count.svg" alt="Visitor's Count" />
</div
>
