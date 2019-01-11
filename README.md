
# Paperback

Software to assist in digital data backup to... dead tree paper.

# Dependencies

* node v8, npm, and `npm install` dependencies in `package.json`
* Ubuntu packages:  qrencode, zbar-tools

# Limitations

* Only small files may be encoded.   500 bytes per page.
* Only one PDF page at present, therefore 500 bytes maximum (limitation being removed soon).

# Usage

Backup binary file to PDF:
```
$ ./genpdf binary500.dat binary500.dat.pdf
```

Restore binary file from PDF backup:
```
$ ./qrpdf2bin binary500.dat.pdf > binary500.dat
```

