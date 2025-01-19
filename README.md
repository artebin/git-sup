# git-sup

Quick and not-so-dirty bash script to show the statuses of multiple Git 
repositories in a concise manner.

## Usage

~~~
Usage: git-sup [OPTION] [GIT_REPOSITORY]...
Show statuses of Git repositories given in arguments or of all 
repositories found from the current working directory when no arguments 
are specified.

Options:
  -f, -F	Do not (f) or do (F) run git fetch.
		Git fetch is not done by default.

  -l, -L	Do not (l) or do (L) show git logs for the commits 
		behind/ahead. Git logs are not showed by default.

Git Config:
  gitsup.rungitfetch	true/false valued. Overridden by option -fF.
  gitsup.showgitlog	true/false valued. Overridden by option -lL.
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
