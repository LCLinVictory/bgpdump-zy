This is a modified version of bgpdump based on another modification
[by dkhenry](https://bitbucket.org/dkhenry/bgpdump) 

Use the below command to see the modifications

```
$ grep -n "by yzhang" *.[ch]
bgpdump_attr.h:215:#define MAX_PREFIXES 2000  /* Change to 2000 from 1000 by yzhang */
util.c:76:/* disable tim2str() to save half time by yzhang */
util.c:77:void time2str(struct tm* date,char *time_str) /* by yzhang */
util.c:78:{                                   /* by yzhang */
util.c:79:    char tmp_str[10];               /* by yzhang */
util.c:80:    tmp_str[0] = '\0';              /* by yzhang */
util.c:81:    return;                         /* by yzhang */
``` 

== libBGPdump ==

A C library designed to help with analyzing dump
files produced by Zebra/Quagga or MRT. Documentation
is available at:

https://bitbucket.org/ripencc/bgpdump/wiki/Home

