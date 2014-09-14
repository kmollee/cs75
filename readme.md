# this is cs75 learning note

change file or directory permission

```shell
find . -type d | xargs chmod 711
find . -type f | xargs chmod 644
find . -name ".php" | xargs chmod 600
```

refer

[在Linux底下，wget參數使用參考](http://itgroup.blueshop.com.tw/pendm/blog?n=convew&i=9401)

[Using wget to recursively fetch a directory with arbitrary files in it](http://stackoverflow.com/questions/273743/using-wget-to-recursively-fetch-a-directory-with-arbitrary-files-in-it)

[How to download with wget without following links with parameters](http://serverfault.com/questions/156045/how-to-download-with-wget-without-following-links-with-parameters)


download from cdn(except mp3 mp4)

```shell
wget -r -R mp3,mp4,torrent --reject-regex '.*download|.*torrent' --no-parent http://cdn.cs75.net/2012/summer/
```
