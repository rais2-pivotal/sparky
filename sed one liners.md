# Useful Unix sed one-liners (or more)

#### Search and replace content between two strings, including the search strings

```
echo "this is really awesome 2312312 test" | sed -e "s:awesome[^*test]*test:BLAH:g"
this is really BLAH
```

#### Perl script to get rid of 'c' style comments '/* and */'
```
perl -0777 -pe 's,/\*.*?\*/,,gs' oia_2_cdm_loading.txt
```
