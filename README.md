# git_sup

## Usage

~~~
Usage: git_sup [OPTION]... [GIT_PROJECT_FOLDER...]
Show statuses of GIT projects given in arguments or all projects found in the current directory when no argument specified.

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
