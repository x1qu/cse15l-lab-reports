#Week 5 Lab Report


1. Less command-line options:
```-E or --QUIT-AT-EOF ```

Causes less to automatically exit.

Examples:

Command I put in:
```(base) apple@dagedademacbook docsearch % less README.md -e ```

Result I got:

```The technical/ directory is a subdirectory of
https://anc.org/data/oanc/download/

~

```

Command I put in:
```(base) apple@dagedademacbook docsearch % less find-results.txt -e ```

Result I got:

```
...
technical/plos/pmed.0010034.txt
technical/plos/pmed.0010008.txt
technical/plos/pmed.0020120.txt
technical/plos/journal.pbio.0020172.txt
technical/plos/pmed.0020040.txt
technical/plos/pmed.0020068.txt
technical/plos/journal.pbio.0020012.txt
technical/plos/pmed.0020281.txt
technical/plos/pmed.0020242.txt
(END) - Next: -e

```

Command I put in:
```(base) apple@dagedademacbook docsearch % less Server.java -e ```

Result I got:

```
...
public class Server {
    public static void start(int port, URLHandler handler) throws IOException {
        HttpServer server = HttpServer.create(new InetSocketAddress(port), 0);

        //create request entrypoint
        server.createContext("/", new ServerHttpHandler(handler));

        //start the server
        server.start();
        System.out.println("Server Started! Visit http://localhost:" + port + " to visit.");
    }
}
(END) - Next: -e

```

This is important because it quits automatically so it could save time.

2. Less command-line options: 
```-f or --force ```

Forces non-regular(a directory or a device special file) files to be opened.   

Examples:

Command I put in:
```(base) apple@dagedademacbook docsearch % less README.md -f ```

Result I got:
```

The technical/ directory is a subdirectory of
https://anc.org/data/oanc/download/

(END) - Next: -f

```

Command I put in:
```(base) apple@dagedademacbook docsearch % less find-results.txt -f ```

Result I got:

```

...
technical/plos/pmed.0020082.txt
technical/plos/pmed.0010021.txt
technical/plos/pmed.0010034.txt
technical/plos/pmed.0010008.txt
technical/plos/pmed.0020120.txt
technical/plos/journal.pbio.0020172.txt
technical/plos/pmed.0020040.txt
technical/plos/pmed.0020068.txt
technical/plos/journal.pbio.0020012.txt
technical/plos/pmed.0020281.txt
technical/plos/pmed.0020242.txt
(END) - Next: -f

```

Command I put in:
```(base) apple@dagedademacbook docsearch % less Server.java -f ```

Result I got:

```

public static void start(int port, URLHandler handler) throws IOException {
        HttpServer server = HttpServer.create(new InetSocketAddress(port), 0);

        //create request entrypoint
        server.createContext("/", new ServerHttpHandler(handler));

        //start the server
        server.start();
        System.out.println("Server Started! Visit http://localhost:" + port + " to visit.");
    }
}
(END) - Next: -f

```

This is important because you get to force to open certain files that could be unprocessable by less.

3. Less command-line options: 
```--N or --LINE-NUMBERS ```

Display a line number at the beginning of each line.

Examples:

Command I put in:
```(base) apple@dagedademacbook docsearch % less -N README.md ```

Result I got:

```

1 The technical/ directory is a subdirectory of
      2 https://anc.org/data/oanc/download/
      3 
~
~
~
~
~
~
~
~
~
(END)

``` 

Command I put in:
```(base) apple@dagedademacbook docsearch % less -N find-results.txt ```

Result I got:

```

...
242 technical/plos/pmed.0020055.txt
    243 technical/plos/pmed.0020082.txt
    244 technical/plos/pmed.0010021.txt
    245 technical/plos/pmed.0010034.txt
    246 technical/plos/pmed.0010008.txt
    247 technical/plos/pmed.0020120.txt
    248 technical/plos/journal.pbio.0020172.txt
    249 technical/plos/pmed.0020040.txt
    250 technical/plos/pmed.0020068.txt
    251 technical/plos/journal.pbio.0020012.txt
    252 technical/plos/pmed.0020281.txt
    253 technical/plos/pmed.0020242.txt
(END)

```

Command I put in:
```(base) apple@dagedademacbook docsearch % less -N Server.java ```

Result I got:

```

...
42 public class Server {
     43     public static void start(int port, URLHandler handler) throws IOException {
     44         HttpServer server = HttpServer.create(new InetSocketAddress(port), 0);
     45 
     46         //create request entrypoint
     47         server.createContext("/", new ServerHttpHandler(handler));
     48 
     49         //start the server
     50         server.start();
     51         System.out.println("Server Started! Visit http://localhost:" + port + " to visit.");
     52     }
     53 }
(END)

```


This is important because by displaying each line number, it helps users find a specific line more easily. It saves a lot of time by not
counting lines. 
