# git_sup

Quick and not-so-dirty bash script to show the status of multiple GIT projects in one command and a concise maneer.  
It is based only on git commands and in particular it parses the output of `git branch`.

## Usage

~~~
Usage: git_sup [OPTION]... [GIT_PROJECT_FOLDER...]
Show status of GIT projects given in arguments or of all projects found in the current directory when no argument are specified.

  -f PERFORM_GIT_FETCH
~~~

## Example

~~~
njames@rollin:MyProjects$ git_sup -f
🗀 felix !! 2 pending change(s)
   * master ↪ origin/master: behind 14

🗀 felix-archives
   * master ↪ origin/master

🗀 felix-themes
   * main ↪ origin/main

🗀 git_sup !! 1 pending change(s)
   * main ↪ origin/main

🗀 MyConfig
   * master ↪ origin/master

🗀 MyCurriculumVitae
   * master ↪ origin/master

🗀 MyDocumentation
   * master ↪ origin/master: behind 3

🗀 MyMurtaugh
   * master ↪ origin/master: behind 4

🗀 SpectralSorcery
   * main ↪ origin/main
~~~
