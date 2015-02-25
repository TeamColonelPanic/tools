Steghide
========

[Steghide](http://steghide.sourceforge.net/) can be used to hide and extract data in various kinds of image- and audio-files..

```
To hide or embed:
        steghide embed -cf picture.jpg -ef secret.txt
        This command will embed the file secret.txt in the cover file picture.jpg.

To extract:
        steghide extract -sf picture.jpg
        If the supplied passphrase is correct, the contents of the original file secret.txt will be extracted from the stego file picture.jpg and saved in the current directory.

To get some information about a file that contains embedded data before extracting it:
        steghide info received_file.wav
```

Reference usage
---------------

[TODO / QName](writeupurl)