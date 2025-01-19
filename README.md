# git-sup

Quick and not-so-dirty bash script to show the statuses of multiple Git 
repositories in a concise manner.

## Usage

~~~
Usage: $(basename ${BASH_SOURCE}) [OPTION] [GIT_REPOSITORY]...
Show statuses of Git repositories given in arguments or of all 
repositories found from the current working directory when no arguments 
are specified.

Options:
  -fF	Do not (f) or do run (F) git fetch.
	Git fetch is not done by default.

  -lL	Do not (l) or do show (L) git log for the commits behind/ahead.
	Git logs are not showed by default.

Git Config:
  gitsup.rungitfetch	true/false valued. Overriden by option -fF.
  gitsup.showgitlog	true/false valued. Overriden by option -lL.
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
