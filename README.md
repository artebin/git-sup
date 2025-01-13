# git-sup

Quick and not-so-dirty bash script to show the status of multiple Git 
repositories concise manner.

## Usage

~~~
Usage: git-sup [OPTIONS] [GIT_PROJECT_FOLDER ...]
Show statuses of Git repositories given in arguments or of all 
repoitories found in the current directory when no argument specified.

Options:
  -f	Perform git fetch.

~~~

## Example

~~~
njames@rollin:MyProjects$ git-sup -f
⏺ boo
   * main ➜ origin/main

⏺ felix !! 2 pending change(s)
   * master [behind 1] ➜ origin/master

⏺ felix-themes
   * main ➜ origin/main

⏺ git-sup
   * main ➜ origin/main

⏺ MyCurriculumVitae
   * master ➜ origin/master

⏺ MyDocumentation
   * master ➜ origin/master

⏺ MyMurtaugh !! 1 pending change(s)
   * master ➜ origin/master

⏺ MyWorkshop !! 53 pending change(s)
   * main ➜ origin/main

⏺ rififi
   * main [behind 1] ➜ origin/main
~~~
