This module plays (by default) [https://www.youtube.com/watch?v=kxopViU98Xo]("Epic sax guy 10 hours") on a target Google Chromecast via YouTube.

Naturally, audio should be cranked to 11 before running this module.

## Verification Steps

1. Do: ```use auxiliary/scanner/http/chromecast_webserver ```
2. Do: ```set RHOST [IP]```
3. Do: ```run```

## Options

  **VID**

  The YouTube video to be played.  Defaults to [https://www.youtube.com/watch?v=kxopViU98Xo](kxopViU98Xo)

## Sample Output

Of note, this was played on a 1st generation Google Chromecast (USB stick looking, not circular)

```
msf > auxiliary/admin/chromecast/chromecast_youtube
msf auxiliary(chromecast_youtube) > set rhost 10.10.10.196
rhost => 10.10.10.196
msf auxiliary(chromecast_youtube) > run

[+] Playing https://www.youtube.com/watch?v=kxopViU98Xo
[*] Auxiliary module execution completed
```
