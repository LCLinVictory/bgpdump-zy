This is a modified version of bgpdump.

Use the below commond to see the modifications

```
$ grep 'by yzhang' *.[ch]
bgpdump_attr.h:#define MAX_PREFIXES 2000  /* Change to 2000 from 1000 by yzhang */
util.c:/* disable tim2str() to save half time by yzhang */
util.c:void time2str(struct tm* date,char *time_str) /* by yzhang */
util.c:{                                   /* by yzhang */
util.c:    char tmp_str[10];               /* by yzhang */
util.c:    tmp_str[0] = '\0';              /* by yzhang */
util.c:    return;                         /* by yzhang */
``` 

== libBGPdump ==

A C library designed to help with analyzing dump
files produced by Zebra/Quagga or MRT. Documenation
is available at:

https://bitbucket.org/ripencc/bgpdump/wiki/Home

