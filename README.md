docker-tangle-nginx
===

* An example of using Org mode, babel, and tangle to set up, run, invoke, and stop an nginx server

Usage
===

* Edit the dtn.org file (in an emacs that supports orgmode, e.g, 24)
* Run the setup shell source blocks (using C-c C-c and respond yes to prompts))
* Generate the build/Dockerfile (using C-c C-v t in the dockerfile source block)
* Run the remaning shell source blocks

To regenerate the .html file
===

* Edit the dtn.org file
* Export to html (C-c C-e h o and then respond yes to prompts)

Sample exported .html
===
Browse [sample output](http://wrightmikea.github.io/docker-tangle-nginx.html "exported html")

Notes
===
* Mac OS X
* Docker Toolkit
* Emacs 24.5.1
* ~/.emacs/init.el customizations

>     (org-babel-do-load-languages
>       'org-babel-load-languages
>        '((sh . t)
>         ))

* I also had to workaround an orgmode/babel bug where the output of docker ps was not being displayed due to a greater-than symbol