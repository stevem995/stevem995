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

### Emacs Tips

### Emacs Go Print Function

```
Description: Creates an interactive Emacs GO function which which creates a
GO styled print statement and places the cursor accordingly.
Example: fmt.Println("")
Usage: M-x goprin
Installation: Place this in your .emacs file.


(defun goprin ()
  "defalias pyprin: Insert go print skeleton"
  (interactive)
  (insert "fmt.Println\(\"\"\)")
  (backward-char 2))
```

### Emacs Python3 Print Function

```
Description: Creates an interactive Emacs Python print function which which creates a
python3 styled print statement and places the cursor accordingly.
Example: print("{}".format())
Usage: M-x pyprin
Installation: Place this in your .emacs file.

(defun pyprin ()
  "defalias pyprin: Insert python print skeleton"
  (interactive)
  (insert "print\(\"\{\}\".format\(\)\)")
  (backward-char 13))
```

### Emacs Powershell Print Function

```
Description: Creates an interactive Emacs Powershell print function which which creates a
Powershell styled print statement and places the cursor accordingly.
Example: Write-Host ("{0}" -f )
Usage: M-x pyprin
Installation: Place this in your .emacs file.

(defun psprin ()
  "defalias psprin: Insert powershell print skeleton"
  (interactive)
  (insert "Write-Host \(\"\{0\}\" -f \)")
  (backward-char 9))
```


<div align="center">
  <p>Visitor count</p>
  <img src="https://profile-counter.glitch.me/stevem995/count.svg" alt="Visitor's Count" />
</div
>
