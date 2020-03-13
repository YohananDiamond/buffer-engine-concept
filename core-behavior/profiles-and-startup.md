# Profiles and Startup

Note: there are some files specified with .ext: it's a temporary
extension name for the script files, which is something yet to be
decided.

1. The basic core (& interpreter) starts up;

2. It stores the contents of the CLI argument --profile (or -p), or
   --file (or -f); these arguments are mutually exclusive.

3. If -f is specified, it tries to load -f as the start file.

4. Else, if -p is specified (or not, where -p
   defaults to "main"), it tries all of the cases below (stopping on the
   when there is a successful one, stopping the program altogether if
   all of them fail):

   * It looks for `${XDG_CONFIG_HOME:-~/.config}/bfe/profiles/${X}.ext`
   and tries to run it.

   * It looks for `${XDG_CONFIG_HOME:-~/.config}/bfe/${X}.ext` and tries
   to run it.

   * It looks for `/usr/share/bfe/profiles/${X}.ext` and tries to run
   it.

   Where `${X}` is the option given by -p.

`/usr/share/bfe/profiles/main.ext` should be the starting point of a
default example profile.

<!-- TODO: where to locate standard library? -->
