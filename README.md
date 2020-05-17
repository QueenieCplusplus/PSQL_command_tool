# PSQL command tool
below version 8 ~ 9.2 , if wanna above version 9.2 ~ 12 see document 

https://www.postgresql.org/docs/12/app-psql.html

    psql --help
    psql is the PostgreSQL interactive terminal. Usage:
    psql [OPTION]... [DBNAME [USERNAME]]

General options:

    -c, --command=COMMAND
    -d, --dbname=DBNAME
    -f, --file=FILENAME
    -l, --list
    -v, --set=, --variable=NAME=VALUE
    set psql variable NAME to VALUE


-X, --no-psqlrc do not read startup file (~/.psqlrc) -1 ("one"), --single-transaction
execute command file as a single transaction

      --help show this help, then exit
      --version output version information, then exit
      
Input and output options:

Connection options:

run only single command (SQL or internal) and exit database name to connect to
execute commands from file, then exit
list available databases, then exit

    -a, --echo-all. echo all input from script
    -e, --echo-queries. echo commands sent to server
    -E, --echo-hidden. display queries that internal commands generate
    -L, --log-file=FILENAME. send session log to file
    -n, --no-readline. disable enhanced command line editing (readline)
    -o, --output=FILENAME. send query results to file (or |pipe)
    -q, --quiet. run quietly (no messages, only query output) 
    -s, --single-step. single-step mode (confirm each query)
    -S, --single-line. single-line mode (end of line terminates SQL command)
    
Output format options:

    -A, --no-align. unaligned table output mode
    -F, --field-separator=STRING. set field separator (default: "|")
    -H, --html HTML table output mode. set HTML table tag attributes (e.g., width, border) 
    -P, --pset=VAR[=ARG] set printing option VAR to ARG (see \pset command) -R, --record-separator=STRING
    set record separator (default: newline)
    -t, --tuples-only. print rows only
    -T, --table-attr=TEXT
    -x, --expanded. turn on expanded table output
    -z, --field-separator-zero set field separator to zero byte 
    -0, --record-separator-zero. set record separator to zero byte
    

-h, --host=HOSTNAME database server host or socket directory
  144 | Appendix: Install, Hosting, and Command-Line Guides
-p, --port=PORT database server port (default: "5432")
-U, --username=USERNAME database user name
-w, --no-password never prompt for password
-W, --password force password prompt (should happen automatically)


For more information, type "\?" (for internal commands) or "\help" (for SQL commands) from within psql, or consult the psql section in the PostgreSQL documentation.
These items are new features introduced in PostgreSQL 9.2.
