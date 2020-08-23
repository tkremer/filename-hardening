This is just a set of files with weird names that may throw off your shell scripts and/or various utilities. Run your backup scripts against this and see if they break.

Things considered include:
- shell metacharacters and spaces in filenames
- UTF-8 and corresponding non-UTF-8 filenames
- escape sequences and control characters in filenames
- line feeds in filenames
- SQL injection in filenames
- a literal "-" filename
- colons in filenames (for tools like rsync)
- circular symlinks
- a named pipe (for grep -R)
- filenames that are historically reserved in Windows

