# rpi_tracked
记录一次树莓派被攻击

```
└─[0] cat  /var/log/auth.log.1|  grep 221.231.139
Mar 31 20:40:14 raspberrypi sshd[17467]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:14 raspberrypi sshd[17470]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:15 raspberrypi sshd[17470]: Failed password for root from 221.231.139.150 port 3671 ssh2
Mar 31 20:40:15 raspberrypi sshd[17467]: Failed password for root from 221.231.139.150 port 3439 ssh2
Mar 31 20:40:17 raspberrypi sshd[17470]: Failed password for root from 221.231.139.150 port 3671 ssh2
Mar 31 20:40:17 raspberrypi sshd[17467]: Failed password for root from 221.231.139.150 port 3439 ssh2
Mar 31 20:40:19 raspberrypi sshd[17470]: Failed password for root from 221.231.139.150 port 3671 ssh2
Mar 31 20:40:21 raspberrypi sshd[17467]: Failed password for root from 221.231.139.150 port 3439 ssh2
Mar 31 20:40:22 raspberrypi sshd[17470]: Failed password for root from 221.231.139.150 port 3671 ssh2
Mar 31 20:40:23 raspberrypi sshd[17467]: Failed password for root from 221.231.139.150 port 3439 ssh2
Mar 31 20:40:25 raspberrypi sshd[17470]: Failed password for root from 221.231.139.150 port 3671 ssh2
Mar 31 20:40:25 raspberrypi sshd[17467]: Failed password for root from 221.231.139.150 port 3439 ssh2
Mar 31 20:40:27 raspberrypi sshd[17470]: Failed password for root from 221.231.139.150 port 3671 ssh2
Mar 31 20:40:27 raspberrypi sshd[17470]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3671 ssh2 [preauth]
Mar 31 20:40:27 raspberrypi sshd[17470]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:27 raspberrypi sshd[17467]: Failed password for root from 221.231.139.150 port 3439 ssh2
Mar 31 20:40:27 raspberrypi sshd[17467]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3439 ssh2 [preauth]
Mar 31 20:40:27 raspberrypi sshd[17467]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:29 raspberrypi sshd[17511]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:29 raspberrypi sshd[17513]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:31 raspberrypi sshd[17511]: Failed password for root from 221.231.139.150 port 1425 ssh2
Mar 31 20:40:32 raspberrypi sshd[17513]: Failed password for root from 221.231.139.150 port 1436 ssh2
Mar 31 20:40:34 raspberrypi sshd[17511]: Failed password for root from 221.231.139.150 port 1425 ssh2
Mar 31 20:40:34 raspberrypi sshd[17513]: Failed password for root from 221.231.139.150 port 1436 ssh2
Mar 31 20:40:36 raspberrypi sshd[17511]: Failed password for root from 221.231.139.150 port 1425 ssh2
Mar 31 20:40:37 raspberrypi sshd[17513]: Failed password for root from 221.231.139.150 port 1436 ssh2
Mar 31 20:40:39 raspberrypi sshd[17511]: Failed password for root from 221.231.139.150 port 1425 ssh2
Mar 31 20:40:39 raspberrypi sshd[17513]: Failed password for root from 221.231.139.150 port 1436 ssh2
Mar 31 20:40:41 raspberrypi sshd[17513]: Failed password for root from 221.231.139.150 port 1436 ssh2
Mar 31 20:40:41 raspberrypi sshd[17511]: Failed password for root from 221.231.139.150 port 1425 ssh2
Mar 31 20:40:44 raspberrypi sshd[17513]: Failed password for root from 221.231.139.150 port 1436 ssh2
Mar 31 20:40:44 raspberrypi sshd[17513]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1436 ssh2 [preauth]
Mar 31 20:40:44 raspberrypi sshd[17513]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:44 raspberrypi sshd[17511]: Failed password for root from 221.231.139.150 port 1425 ssh2
Mar 31 20:40:44 raspberrypi sshd[17511]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1425 ssh2 [preauth]
Mar 31 20:40:44 raspberrypi sshd[17511]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:45 raspberrypi sshd[17546]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:47 raspberrypi sshd[17546]: Failed password for root from 221.231.139.150 port 2587 ssh2
Mar 31 20:40:50 raspberrypi sshd[17546]: Failed password for root from 221.231.139.150 port 2587 ssh2
Mar 31 20:40:51 raspberrypi sshd[17546]: Failed password for root from 221.231.139.150 port 2587 ssh2
Mar 31 20:40:53 raspberrypi sshd[17546]: Failed password for root from 221.231.139.150 port 2587 ssh2
Mar 31 20:40:56 raspberrypi sshd[17554]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:56 raspberrypi sshd[17546]: Failed password for root from 221.231.139.150 port 2587 ssh2
Mar 31 20:40:58 raspberrypi sshd[17554]: Failed password for root from 221.231.139.150 port 2657 ssh2
Mar 31 20:40:58 raspberrypi sshd[17546]: Failed password for root from 221.231.139.150 port 2587 ssh2
Mar 31 20:40:58 raspberrypi sshd[17546]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2587 ssh2 [preauth]
Mar 31 20:40:58 raspberrypi sshd[17546]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:40:59 raspberrypi sshd[17577]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:00 raspberrypi sshd[17554]: Failed password for root from 221.231.139.150 port 2657 ssh2
Mar 31 20:41:01 raspberrypi sshd[17577]: Failed password for root from 221.231.139.150 port 4201 ssh2
Mar 31 20:41:02 raspberrypi sshd[17554]: Failed password for root from 221.231.139.150 port 2657 ssh2
Mar 31 20:41:03 raspberrypi sshd[17577]: Failed password for root from 221.231.139.150 port 4201 ssh2
Mar 31 20:41:05 raspberrypi sshd[17577]: Failed password for root from 221.231.139.150 port 4201 ssh2
Mar 31 20:41:05 raspberrypi sshd[17554]: Failed password for root from 221.231.139.150 port 2657 ssh2
Mar 31 20:41:07 raspberrypi sshd[17577]: Failed password for root from 221.231.139.150 port 4201 ssh2
Mar 31 20:41:09 raspberrypi sshd[17554]: Failed password for root from 221.231.139.150 port 2657 ssh2
Mar 31 20:41:10 raspberrypi sshd[17577]: Failed password for root from 221.231.139.150 port 4201 ssh2
Mar 31 20:41:12 raspberrypi sshd[17554]: Failed password for root from 221.231.139.150 port 2657 ssh2
Mar 31 20:41:12 raspberrypi sshd[17554]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2657 ssh2 [preauth]
Mar 31 20:41:12 raspberrypi sshd[17554]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:12 raspberrypi sshd[17577]: Failed password for root from 221.231.139.150 port 4201 ssh2
Mar 31 20:41:12 raspberrypi sshd[17577]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4201 ssh2 [preauth]
Mar 31 20:41:12 raspberrypi sshd[17577]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:13 raspberrypi sshd[17623]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:14 raspberrypi sshd[17632]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:15 raspberrypi sshd[17623]: Failed password for root from 221.231.139.150 port 1394 ssh2
Mar 31 20:41:16 raspberrypi sshd[17632]: Failed password for root from 221.231.139.150 port 1423 ssh2
Mar 31 20:41:19 raspberrypi sshd[17632]: Failed password for root from 221.231.139.150 port 1423 ssh2
Mar 31 20:41:19 raspberrypi sshd[17623]: Failed password for root from 221.231.139.150 port 1394 ssh2
Mar 31 20:41:22 raspberrypi sshd[17632]: Failed password for root from 221.231.139.150 port 1423 ssh2
Mar 31 20:41:22 raspberrypi sshd[17623]: Failed password for root from 221.231.139.150 port 1394 ssh2
Mar 31 20:41:24 raspberrypi sshd[17632]: Failed password for root from 221.231.139.150 port 1423 ssh2
Mar 31 20:41:24 raspberrypi sshd[17623]: Failed password for root from 221.231.139.150 port 1394 ssh2
Mar 31 20:41:26 raspberrypi sshd[17632]: Failed password for root from 221.231.139.150 port 1423 ssh2
Mar 31 20:41:26 raspberrypi sshd[17623]: Failed password for root from 221.231.139.150 port 1394 ssh2
Mar 31 20:41:28 raspberrypi sshd[17632]: Failed password for root from 221.231.139.150 port 1423 ssh2
Mar 31 20:41:28 raspberrypi sshd[17632]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1423 ssh2 [preauth]
Mar 31 20:41:28 raspberrypi sshd[17632]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:28 raspberrypi sshd[17623]: Failed password for root from 221.231.139.150 port 1394 ssh2
Mar 31 20:41:28 raspberrypi sshd[17623]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1394 ssh2 [preauth]
Mar 31 20:41:28 raspberrypi sshd[17623]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:29 raspberrypi sshd[17672]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:32 raspberrypi sshd[17672]: Failed password for root from 221.231.139.150 port 2229 ssh2
Mar 31 20:41:34 raspberrypi sshd[17674]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:35 raspberrypi sshd[17672]: Failed password for root from 221.231.139.150 port 2229 ssh2
Mar 31 20:41:35 raspberrypi sshd[17674]: Failed password for root from 221.231.139.150 port 2238 ssh2
Mar 31 20:41:37 raspberrypi sshd[17672]: Failed password for root from 221.231.139.150 port 2229 ssh2
Mar 31 20:41:38 raspberrypi sshd[17674]: Failed password for root from 221.231.139.150 port 2238 ssh2
Mar 31 20:41:39 raspberrypi sshd[17672]: Failed password for root from 221.231.139.150 port 2229 ssh2
Mar 31 20:41:39 raspberrypi sshd[17674]: Failed password for root from 221.231.139.150 port 2238 ssh2
Mar 31 20:41:42 raspberrypi sshd[17672]: Failed password for root from 221.231.139.150 port 2229 ssh2
Mar 31 20:41:43 raspberrypi sshd[17674]: Failed password for root from 221.231.139.150 port 2238 ssh2
Mar 31 20:41:44 raspberrypi sshd[17672]: Failed password for root from 221.231.139.150 port 2229 ssh2
Mar 31 20:41:44 raspberrypi sshd[17672]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2229 ssh2 [preauth]
Mar 31 20:41:44 raspberrypi sshd[17672]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:46 raspberrypi sshd[17674]: Failed password for root from 221.231.139.150 port 2238 ssh2
Mar 31 20:41:46 raspberrypi sshd[17703]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:48 raspberrypi sshd[17703]: Failed password for root from 221.231.139.150 port 2953 ssh2
Mar 31 20:41:48 raspberrypi sshd[17674]: Failed password for root from 221.231.139.150 port 2238 ssh2
Mar 31 20:41:48 raspberrypi sshd[17674]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2238 ssh2 [preauth]
Mar 31 20:41:48 raspberrypi sshd[17674]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:50 raspberrypi sshd[17703]: Failed password for root from 221.231.139.150 port 2953 ssh2
Mar 31 20:41:51 raspberrypi sshd[17703]: Failed password for root from 221.231.139.150 port 2953 ssh2
Mar 31 20:41:53 raspberrypi sshd[17716]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:41:54 raspberrypi sshd[17703]: Failed password for root from 221.231.139.150 port 2953 ssh2
Mar 31 20:41:55 raspberrypi sshd[17716]: Failed password for root from 221.231.139.150 port 3109 ssh2
Mar 31 20:41:57 raspberrypi sshd[17703]: Failed password for root from 221.231.139.150 port 2953 ssh2
Mar 31 20:41:58 raspberrypi sshd[17716]: Failed password for root from 221.231.139.150 port 3109 ssh2
Mar 31 20:41:58 raspberrypi sshd[17703]: Failed password for root from 221.231.139.150 port 2953 ssh2
Mar 31 20:41:58 raspberrypi sshd[17703]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2953 ssh2 [preauth]
Mar 31 20:41:58 raspberrypi sshd[17703]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:00 raspberrypi sshd[17716]: Failed password for root from 221.231.139.150 port 3109 ssh2
Mar 31 20:42:00 raspberrypi sshd[17738]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:02 raspberrypi sshd[17716]: Failed password for root from 221.231.139.150 port 3109 ssh2
Mar 31 20:42:02 raspberrypi sshd[17738]: Failed password for root from 221.231.139.150 port 3555 ssh2
Mar 31 20:42:04 raspberrypi sshd[17716]: Failed password for root from 221.231.139.150 port 3109 ssh2
Mar 31 20:42:04 raspberrypi sshd[17738]: Failed password for root from 221.231.139.150 port 3555 ssh2
Mar 31 20:42:06 raspberrypi sshd[17716]: Failed password for root from 221.231.139.150 port 3109 ssh2
Mar 31 20:42:06 raspberrypi sshd[17716]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3109 ssh2 [preauth]
Mar 31 20:42:06 raspberrypi sshd[17716]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:06 raspberrypi sshd[17738]: Failed password for root from 221.231.139.150 port 3555 ssh2
Mar 31 20:42:07 raspberrypi sshd[17776]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:08 raspberrypi sshd[17738]: Failed password for root from 221.231.139.150 port 3555 ssh2
Mar 31 20:42:09 raspberrypi sshd[17776]: Failed password for root from 221.231.139.150 port 3849 ssh2
Mar 31 20:42:10 raspberrypi sshd[17738]: Failed password for root from 221.231.139.150 port 3555 ssh2
Mar 31 20:42:11 raspberrypi sshd[17776]: Failed password for root from 221.231.139.150 port 3849 ssh2
Mar 31 20:42:12 raspberrypi sshd[17738]: Failed password for root from 221.231.139.150 port 3555 ssh2
Mar 31 20:42:12 raspberrypi sshd[17738]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3555 ssh2 [preauth]
Mar 31 20:42:12 raspberrypi sshd[17738]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:13 raspberrypi sshd[17776]: Failed password for root from 221.231.139.150 port 3849 ssh2
Mar 31 20:42:14 raspberrypi sshd[17793]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:16 raspberrypi sshd[17776]: Failed password for root from 221.231.139.150 port 3849 ssh2
Mar 31 20:42:16 raspberrypi sshd[17793]: Failed password for root from 221.231.139.150 port 4152 ssh2
Mar 31 20:42:18 raspberrypi sshd[17776]: Failed password for root from 221.231.139.150 port 3849 ssh2
Mar 31 20:42:18 raspberrypi sshd[17793]: Failed password for root from 221.231.139.150 port 4152 ssh2
Mar 31 20:42:20 raspberrypi sshd[17776]: Failed password for root from 221.231.139.150 port 3849 ssh2
Mar 31 20:42:20 raspberrypi sshd[17776]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3849 ssh2 [preauth]
Mar 31 20:42:20 raspberrypi sshd[17776]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:20 raspberrypi sshd[17793]: Failed password for root from 221.231.139.150 port 4152 ssh2
Mar 31 20:42:22 raspberrypi sshd[17793]: Failed password for root from 221.231.139.150 port 4152 ssh2
Mar 31 20:42:23 raspberrypi sshd[17815]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:24 raspberrypi sshd[17793]: Failed password for root from 221.231.139.150 port 4152 ssh2
Mar 31 20:42:25 raspberrypi sshd[17815]: Failed password for root from 221.231.139.150 port 4511 ssh2
Mar 31 20:42:26 raspberrypi sshd[17793]: Failed password for root from 221.231.139.150 port 4152 ssh2
Mar 31 20:42:26 raspberrypi sshd[17793]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4152 ssh2 [preauth]
Mar 31 20:42:26 raspberrypi sshd[17793]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:28 raspberrypi sshd[17830]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:28 raspberrypi sshd[17815]: Failed password for root from 221.231.139.150 port 4511 ssh2
Mar 31 20:42:29 raspberrypi sshd[17830]: Failed password for root from 221.231.139.150 port 4782 ssh2
Mar 31 20:42:30 raspberrypi sshd[17815]: Failed password for root from 221.231.139.150 port 4511 ssh2
Mar 31 20:42:32 raspberrypi sshd[17830]: Failed password for root from 221.231.139.150 port 4782 ssh2
Mar 31 20:42:32 raspberrypi sshd[17815]: Failed password for root from 221.231.139.150 port 4511 ssh2
Mar 31 20:42:34 raspberrypi sshd[17830]: Failed password for root from 221.231.139.150 port 4782 ssh2
Mar 31 20:42:34 raspberrypi sshd[17815]: Failed password for root from 221.231.139.150 port 4511 ssh2
Mar 31 20:42:36 raspberrypi sshd[17830]: Failed password for root from 221.231.139.150 port 4782 ssh2
Mar 31 20:42:36 raspberrypi sshd[17815]: Failed password for root from 221.231.139.150 port 4511 ssh2
Mar 31 20:42:36 raspberrypi sshd[17815]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4511 ssh2 [preauth]
Mar 31 20:42:36 raspberrypi sshd[17815]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:39 raspberrypi sshd[17830]: Failed password for root from 221.231.139.150 port 4782 ssh2
Mar 31 20:42:39 raspberrypi sshd[17856]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:41 raspberrypi sshd[17830]: Failed password for root from 221.231.139.150 port 4782 ssh2
Mar 31 20:42:41 raspberrypi sshd[17830]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4782 ssh2 [preauth]
Mar 31 20:42:41 raspberrypi sshd[17830]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:41 raspberrypi sshd[17856]: Failed password for root from 221.231.139.150 port 1197 ssh2
Mar 31 20:42:42 raspberrypi sshd[17869]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:43 raspberrypi sshd[17856]: Failed password for root from 221.231.139.150 port 1197 ssh2
Mar 31 20:42:44 raspberrypi sshd[17869]: Failed password for root from 221.231.139.150 port 1355 ssh2
Mar 31 20:42:46 raspberrypi sshd[17856]: Failed password for root from 221.231.139.150 port 1197 ssh2
Mar 31 20:42:46 raspberrypi sshd[17869]: Failed password for root from 221.231.139.150 port 1355 ssh2
Mar 31 20:42:49 raspberrypi sshd[17869]: Failed password for root from 221.231.139.150 port 1355 ssh2
Mar 31 20:42:49 raspberrypi sshd[17856]: Failed password for root from 221.231.139.150 port 1197 ssh2
Mar 31 20:42:51 raspberrypi sshd[17869]: Failed password for root from 221.231.139.150 port 1355 ssh2
Mar 31 20:42:52 raspberrypi sshd[17856]: Failed password for root from 221.231.139.150 port 1197 ssh2
Mar 31 20:42:53 raspberrypi sshd[17869]: Failed password for root from 221.231.139.150 port 1355 ssh2
Mar 31 20:42:54 raspberrypi sshd[17856]: Failed password for root from 221.231.139.150 port 1197 ssh2
Mar 31 20:42:54 raspberrypi sshd[17856]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1197 ssh2 [preauth]
Mar 31 20:42:54 raspberrypi sshd[17856]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:55 raspberrypi sshd[17869]: Failed password for root from 221.231.139.150 port 1355 ssh2
Mar 31 20:42:55 raspberrypi sshd[17869]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1355 ssh2 [preauth]
Mar 31 20:42:55 raspberrypi sshd[17869]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:56 raspberrypi sshd[17906]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:57 raspberrypi sshd[17898]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:42:58 raspberrypi sshd[17906]: Failed password for root from 221.231.139.150 port 1873 ssh2
Mar 31 20:42:59 raspberrypi sshd[17898]: Failed password for root from 221.231.139.150 port 1802 ssh2
Mar 31 20:43:00 raspberrypi sshd[17906]: Failed password for root from 221.231.139.150 port 1873 ssh2
Mar 31 20:43:01 raspberrypi sshd[17898]: Failed password for root from 221.231.139.150 port 1802 ssh2
Mar 31 20:43:03 raspberrypi sshd[17906]: Failed password for root from 221.231.139.150 port 1873 ssh2
Mar 31 20:43:03 raspberrypi sshd[17898]: Failed password for root from 221.231.139.150 port 1802 ssh2
Mar 31 20:43:05 raspberrypi sshd[17906]: Failed password for root from 221.231.139.150 port 1873 ssh2
Mar 31 20:43:05 raspberrypi sshd[17898]: Failed password for root from 221.231.139.150 port 1802 ssh2
Mar 31 20:43:07 raspberrypi sshd[17906]: Failed password for root from 221.231.139.150 port 1873 ssh2
Mar 31 20:43:08 raspberrypi sshd[17898]: Failed password for root from 221.231.139.150 port 1802 ssh2
Mar 31 20:43:09 raspberrypi sshd[17898]: Failed password for root from 221.231.139.150 port 1802 ssh2
Mar 31 20:43:09 raspberrypi sshd[17898]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1802 ssh2 [preauth]
Mar 31 20:43:09 raspberrypi sshd[17898]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:10 raspberrypi sshd[17906]: Failed password for root from 221.231.139.150 port 1873 ssh2
Mar 31 20:43:10 raspberrypi sshd[17906]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1873 ssh2 [preauth]
Mar 31 20:43:10 raspberrypi sshd[17906]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:11 raspberrypi sshd[17962]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:12 raspberrypi sshd[17954]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:13 raspberrypi sshd[17962]: Failed password for root from 221.231.139.150 port 2323 ssh2
Mar 31 20:43:15 raspberrypi sshd[17954]: Failed password for root from 221.231.139.150 port 2308 ssh2
Mar 31 20:43:16 raspberrypi sshd[17962]: Failed password for root from 221.231.139.150 port 2323 ssh2
Mar 31 20:43:16 raspberrypi sshd[17954]: Failed password for root from 221.231.139.150 port 2308 ssh2
Mar 31 20:43:18 raspberrypi sshd[17962]: Failed password for root from 221.231.139.150 port 2323 ssh2
Mar 31 20:43:19 raspberrypi sshd[17954]: Failed password for root from 221.231.139.150 port 2308 ssh2
Mar 31 20:43:20 raspberrypi sshd[17962]: Failed password for root from 221.231.139.150 port 2323 ssh2
Mar 31 20:43:21 raspberrypi sshd[17954]: Failed password for root from 221.231.139.150 port 2308 ssh2
Mar 31 20:43:22 raspberrypi sshd[17962]: Failed password for root from 221.231.139.150 port 2323 ssh2
Mar 31 20:43:23 raspberrypi sshd[17954]: Failed password for root from 221.231.139.150 port 2308 ssh2
Mar 31 20:43:24 raspberrypi sshd[17962]: Failed password for root from 221.231.139.150 port 2323 ssh2
Mar 31 20:43:24 raspberrypi sshd[17962]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2323 ssh2 [preauth]
Mar 31 20:43:24 raspberrypi sshd[17962]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:25 raspberrypi sshd[17993]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:26 raspberrypi sshd[17954]: Failed password for root from 221.231.139.150 port 2308 ssh2
Mar 31 20:43:26 raspberrypi sshd[17954]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2308 ssh2 [preauth]
Mar 31 20:43:26 raspberrypi sshd[17954]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:27 raspberrypi sshd[17993]: Failed password for root from 221.231.139.150 port 2752 ssh2
Mar 31 20:43:28 raspberrypi sshd[18001]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:29 raspberrypi sshd[17993]: Failed password for root from 221.231.139.150 port 2752 ssh2
Mar 31 20:43:30 raspberrypi sshd[18001]: Failed password for root from 221.231.139.150 port 2807 ssh2
Mar 31 20:43:31 raspberrypi sshd[17993]: Failed password for root from 221.231.139.150 port 2752 ssh2
Mar 31 20:43:33 raspberrypi sshd[18001]: Failed password for root from 221.231.139.150 port 2807 ssh2
Mar 31 20:43:34 raspberrypi sshd[17993]: Failed password for root from 221.231.139.150 port 2752 ssh2
Mar 31 20:43:34 raspberrypi sshd[18001]: Failed password for root from 221.231.139.150 port 2807 ssh2
Mar 31 20:43:36 raspberrypi sshd[17993]: Failed password for root from 221.231.139.150 port 2752 ssh2
Mar 31 20:43:36 raspberrypi sshd[18001]: Failed password for root from 221.231.139.150 port 2807 ssh2
Mar 31 20:43:38 raspberrypi sshd[17993]: Failed password for root from 221.231.139.150 port 2752 ssh2
Mar 31 20:43:38 raspberrypi sshd[17993]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2752 ssh2 [preauth]
Mar 31 20:43:38 raspberrypi sshd[17993]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:39 raspberrypi sshd[18001]: Failed password for root from 221.231.139.150 port 2807 ssh2
Mar 31 20:43:39 raspberrypi sshd[18030]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:41 raspberrypi sshd[18001]: Failed password for root from 221.231.139.150 port 2807 ssh2
Mar 31 20:43:41 raspberrypi sshd[18001]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2807 ssh2 [preauth]
Mar 31 20:43:41 raspberrypi sshd[18001]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:41 raspberrypi sshd[18030]: Failed password for root from 221.231.139.150 port 3185 ssh2
Mar 31 20:43:41 raspberrypi sshd[18042]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:43 raspberrypi sshd[18030]: Failed password for root from 221.231.139.150 port 3185 ssh2
Mar 31 20:43:43 raspberrypi sshd[18042]: Failed password for root from 221.231.139.150 port 3238 ssh2
Mar 31 20:43:46 raspberrypi sshd[18030]: Failed password for root from 221.231.139.150 port 3185 ssh2
Mar 31 20:43:46 raspberrypi sshd[18042]: Failed password for root from 221.231.139.150 port 3238 ssh2
Mar 31 20:43:48 raspberrypi sshd[18030]: Failed password for root from 221.231.139.150 port 3185 ssh2
Mar 31 20:43:48 raspberrypi sshd[18042]: Failed password for root from 221.231.139.150 port 3238 ssh2
Mar 31 20:43:50 raspberrypi sshd[18030]: Failed password for root from 221.231.139.150 port 3185 ssh2
Mar 31 20:43:51 raspberrypi sshd[18042]: Failed password for root from 221.231.139.150 port 3238 ssh2
Mar 31 20:43:53 raspberrypi sshd[18042]: Failed password for root from 221.231.139.150 port 3238 ssh2
Mar 31 20:43:53 raspberrypi sshd[18030]: Failed password for root from 221.231.139.150 port 3185 ssh2
Mar 31 20:43:53 raspberrypi sshd[18030]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3185 ssh2 [preauth]
Mar 31 20:43:53 raspberrypi sshd[18030]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:54 raspberrypi sshd[18071]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:55 raspberrypi sshd[18042]: Failed password for root from 221.231.139.150 port 3238 ssh2
Mar 31 20:43:55 raspberrypi sshd[18042]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3238 ssh2 [preauth]
Mar 31 20:43:55 raspberrypi sshd[18042]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:57 raspberrypi sshd[18071]: Failed password for root from 221.231.139.150 port 3582 ssh2
Mar 31 20:43:57 raspberrypi sshd[18079]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:43:59 raspberrypi sshd[18071]: Failed password for root from 221.231.139.150 port 3582 ssh2
Mar 31 20:44:00 raspberrypi sshd[18079]: Failed password for root from 221.231.139.150 port 3649 ssh2
Mar 31 20:44:02 raspberrypi sshd[18071]: Failed password for root from 221.231.139.150 port 3582 ssh2
Mar 31 20:44:02 raspberrypi sshd[18079]: Failed password for root from 221.231.139.150 port 3649 ssh2
Mar 31 20:44:04 raspberrypi sshd[18071]: Failed password for root from 221.231.139.150 port 3582 ssh2
Mar 31 20:44:04 raspberrypi sshd[18079]: Failed password for root from 221.231.139.150 port 3649 ssh2
Mar 31 20:44:05 raspberrypi sshd[18071]: Failed password for root from 221.231.139.150 port 3582 ssh2
Mar 31 20:44:06 raspberrypi sshd[18079]: Failed password for root from 221.231.139.150 port 3649 ssh2
Mar 31 20:44:08 raspberrypi sshd[18071]: Failed password for root from 221.231.139.150 port 3582 ssh2
Mar 31 20:44:08 raspberrypi sshd[18071]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3582 ssh2 [preauth]
Mar 31 20:44:08 raspberrypi sshd[18071]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:08 raspberrypi sshd[18079]: Failed password for root from 221.231.139.150 port 3649 ssh2
Mar 31 20:44:09 raspberrypi sshd[18125]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:11 raspberrypi sshd[18079]: Failed password for root from 221.231.139.150 port 3649 ssh2
Mar 31 20:44:11 raspberrypi sshd[18079]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3649 ssh2 [preauth]
Mar 31 20:44:11 raspberrypi sshd[18079]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:11 raspberrypi sshd[18125]: Failed password for root from 221.231.139.150 port 4033 ssh2
Mar 31 20:44:12 raspberrypi sshd[18135]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:13 raspberrypi sshd[18125]: Failed password for root from 221.231.139.150 port 4033 ssh2
Mar 31 20:44:14 raspberrypi sshd[18135]: Failed password for root from 221.231.139.150 port 4117 ssh2
Mar 31 20:44:16 raspberrypi sshd[18125]: Failed password for root from 221.231.139.150 port 4033 ssh2
Mar 31 20:44:16 raspberrypi sshd[18135]: Failed password for root from 221.231.139.150 port 4117 ssh2
Mar 31 20:44:18 raspberrypi sshd[18125]: Failed password for root from 221.231.139.150 port 4033 ssh2
Mar 31 20:44:18 raspberrypi sshd[18135]: Failed password for root from 221.231.139.150 port 4117 ssh2
Mar 31 20:44:20 raspberrypi sshd[18125]: Failed password for root from 221.231.139.150 port 4033 ssh2
Mar 31 20:44:21 raspberrypi sshd[18135]: Failed password for root from 221.231.139.150 port 4117 ssh2
Mar 31 20:44:23 raspberrypi sshd[18125]: Failed password for root from 221.231.139.150 port 4033 ssh2
Mar 31 20:44:23 raspberrypi sshd[18125]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4033 ssh2 [preauth]
Mar 31 20:44:23 raspberrypi sshd[18125]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:23 raspberrypi sshd[18135]: Failed password for root from 221.231.139.150 port 4117 ssh2
Mar 31 20:44:25 raspberrypi sshd[18164]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:25 raspberrypi sshd[18135]: Failed password for root from 221.231.139.150 port 4117 ssh2
Mar 31 20:44:25 raspberrypi sshd[18135]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4117 ssh2 [preauth]
Mar 31 20:44:25 raspberrypi sshd[18135]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:27 raspberrypi sshd[18164]: Failed password for root from 221.231.139.150 port 4534 ssh2
Mar 31 20:44:29 raspberrypi sshd[18178]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:30 raspberrypi sshd[18164]: Failed password for root from 221.231.139.150 port 4534 ssh2
Mar 31 20:44:31 raspberrypi sshd[18178]: Failed password for root from 221.231.139.150 port 4630 ssh2
Mar 31 20:44:32 raspberrypi sshd[18164]: Failed password for root from 221.231.139.150 port 4534 ssh2
Mar 31 20:44:34 raspberrypi sshd[18178]: Failed password for root from 221.231.139.150 port 4630 ssh2
Mar 31 20:44:34 raspberrypi sshd[18164]: Failed password for root from 221.231.139.150 port 4534 ssh2
Mar 31 20:44:36 raspberrypi sshd[18178]: Failed password for root from 221.231.139.150 port 4630 ssh2
Mar 31 20:44:36 raspberrypi sshd[18164]: Failed password for root from 221.231.139.150 port 4534 ssh2
Mar 31 20:44:38 raspberrypi sshd[18178]: Failed password for root from 221.231.139.150 port 4630 ssh2
Mar 31 20:44:39 raspberrypi sshd[18164]: Failed password for root from 221.231.139.150 port 4534 ssh2
Mar 31 20:44:39 raspberrypi sshd[18164]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4534 ssh2 [preauth]
Mar 31 20:44:39 raspberrypi sshd[18164]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:40 raspberrypi sshd[18204]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:40 raspberrypi sshd[18178]: Failed password for root from 221.231.139.150 port 4630 ssh2
Mar 31 20:44:42 raspberrypi sshd[18204]: Failed password for root from 221.231.139.150 port 1183 ssh2
Mar 31 20:44:43 raspberrypi sshd[18178]: Failed password for root from 221.231.139.150 port 4630 ssh2
Mar 31 20:44:43 raspberrypi sshd[18178]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4630 ssh2 [preauth]
Mar 31 20:44:43 raspberrypi sshd[18178]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:44 raspberrypi sshd[18204]: Failed password for root from 221.231.139.150 port 1183 ssh2
Mar 31 20:44:46 raspberrypi sshd[18204]: Failed password for root from 221.231.139.150 port 1183 ssh2
Mar 31 20:44:47 raspberrypi sshd[18219]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:48 raspberrypi sshd[18219]: Failed password for root from 221.231.139.150 port 1305 ssh2
Mar 31 20:44:48 raspberrypi sshd[18204]: Failed password for root from 221.231.139.150 port 1183 ssh2
Mar 31 20:44:51 raspberrypi sshd[18204]: Failed password for root from 221.231.139.150 port 1183 ssh2
Mar 31 20:44:52 raspberrypi sshd[18219]: Failed password for root from 221.231.139.150 port 1305 ssh2
Mar 31 20:44:54 raspberrypi sshd[18204]: Failed password for root from 221.231.139.150 port 1183 ssh2
Mar 31 20:44:54 raspberrypi sshd[18204]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1183 ssh2 [preauth]
Mar 31 20:44:54 raspberrypi sshd[18204]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:54 raspberrypi sshd[18219]: Failed password for root from 221.231.139.150 port 1305 ssh2
Mar 31 20:44:54 raspberrypi sshd[18239]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:44:56 raspberrypi sshd[18219]: Failed password for root from 221.231.139.150 port 1305 ssh2
Mar 31 20:44:56 raspberrypi sshd[18239]: Failed password for root from 221.231.139.150 port 1568 ssh2
Mar 31 20:44:58 raspberrypi sshd[18219]: Failed password for root from 221.231.139.150 port 1305 ssh2
Mar 31 20:44:59 raspberrypi sshd[18239]: Failed password for root from 221.231.139.150 port 1568 ssh2
Mar 31 20:45:01 raspberrypi sshd[18219]: Failed password for root from 221.231.139.150 port 1305 ssh2
Mar 31 20:45:01 raspberrypi sshd[18219]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1305 ssh2 [preauth]
Mar 31 20:45:01 raspberrypi sshd[18219]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:01 raspberrypi sshd[18239]: Failed password for root from 221.231.139.150 port 1568 ssh2
Mar 31 20:45:04 raspberrypi sshd[18239]: Failed password for root from 221.231.139.150 port 1568 ssh2
Mar 31 20:45:05 raspberrypi sshd[18260]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:06 raspberrypi sshd[18239]: Failed password for root from 221.231.139.150 port 1568 ssh2
Mar 31 20:45:07 raspberrypi sshd[18260]: Failed password for root from 221.231.139.150 port 1795 ssh2
Mar 31 20:45:08 raspberrypi sshd[18239]: Failed password for root from 221.231.139.150 port 1568 ssh2
Mar 31 20:45:08 raspberrypi sshd[18239]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1568 ssh2 [preauth]
Mar 31 20:45:08 raspberrypi sshd[18239]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:09 raspberrypi sshd[18293]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:10 raspberrypi sshd[18260]: Failed password for root from 221.231.139.150 port 1795 ssh2
Mar 31 20:45:11 raspberrypi sshd[18293]: Failed password for root from 221.231.139.150 port 1985 ssh2
Mar 31 20:45:13 raspberrypi sshd[18260]: Failed password for root from 221.231.139.150 port 1795 ssh2
Mar 31 20:45:13 raspberrypi sshd[18293]: Failed password for root from 221.231.139.150 port 1985 ssh2
Mar 31 20:45:16 raspberrypi sshd[18260]: Failed password for root from 221.231.139.150 port 1795 ssh2
Mar 31 20:45:16 raspberrypi sshd[18293]: Failed password for root from 221.231.139.150 port 1985 ssh2
Mar 31 20:45:18 raspberrypi sshd[18293]: Failed password for root from 221.231.139.150 port 1985 ssh2
Mar 31 20:45:18 raspberrypi sshd[18260]: Failed password for root from 221.231.139.150 port 1795 ssh2
Mar 31 20:45:21 raspberrypi sshd[18293]: Failed password for root from 221.231.139.150 port 1985 ssh2
Mar 31 20:45:21 raspberrypi sshd[18260]: Failed password for root from 221.231.139.150 port 1795 ssh2
Mar 31 20:45:21 raspberrypi sshd[18260]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1795 ssh2 [preauth]
Mar 31 20:45:21 raspberrypi sshd[18260]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:23 raspberrypi sshd[18293]: Failed password for root from 221.231.139.150 port 1985 ssh2
Mar 31 20:45:23 raspberrypi sshd[18293]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1985 ssh2 [preauth]
Mar 31 20:45:23 raspberrypi sshd[18293]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:23 raspberrypi sshd[18321]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:24 raspberrypi sshd[18330]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:26 raspberrypi sshd[18321]: Failed password for root from 221.231.139.150 port 2316 ssh2
Mar 31 20:45:26 raspberrypi sshd[18330]: Failed password for root from 221.231.139.150 port 2391 ssh2
Mar 31 20:45:28 raspberrypi sshd[18321]: Failed password for root from 221.231.139.150 port 2316 ssh2
Mar 31 20:45:28 raspberrypi sshd[18330]: Failed password for root from 221.231.139.150 port 2391 ssh2
Mar 31 20:45:31 raspberrypi sshd[18321]: Failed password for root from 221.231.139.150 port 2316 ssh2
Mar 31 20:45:31 raspberrypi sshd[18330]: Failed password for root from 221.231.139.150 port 2391 ssh2
Mar 31 20:45:33 raspberrypi sshd[18321]: Failed password for root from 221.231.139.150 port 2316 ssh2
Mar 31 20:45:33 raspberrypi sshd[18330]: Failed password for root from 221.231.139.150 port 2391 ssh2
Mar 31 20:45:36 raspberrypi sshd[18321]: Failed password for root from 221.231.139.150 port 2316 ssh2
Mar 31 20:45:36 raspberrypi sshd[18330]: Failed password for root from 221.231.139.150 port 2391 ssh2
Mar 31 20:45:38 raspberrypi sshd[18321]: Failed password for root from 221.231.139.150 port 2316 ssh2
Mar 31 20:45:38 raspberrypi sshd[18321]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2316 ssh2 [preauth]
Mar 31 20:45:38 raspberrypi sshd[18321]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:39 raspberrypi sshd[18330]: Failed password for root from 221.231.139.150 port 2391 ssh2
Mar 31 20:45:39 raspberrypi sshd[18330]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2391 ssh2 [preauth]
Mar 31 20:45:39 raspberrypi sshd[18330]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:39 raspberrypi sshd[18369]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:41 raspberrypi sshd[18369]: Failed password for root from 221.231.139.150 port 2806 ssh2
Mar 31 20:45:41 raspberrypi sshd[18361]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:43 raspberrypi sshd[18361]: Failed password for root from 221.231.139.150 port 2799 ssh2
Mar 31 20:45:43 raspberrypi sshd[18369]: Failed password for root from 221.231.139.150 port 2806 ssh2
Mar 31 20:45:46 raspberrypi sshd[18361]: Failed password for root from 221.231.139.150 port 2799 ssh2
Mar 31 20:45:46 raspberrypi sshd[18369]: Failed password for root from 221.231.139.150 port 2806 ssh2
Mar 31 20:45:48 raspberrypi sshd[18369]: Failed password for root from 221.231.139.150 port 2806 ssh2
Mar 31 20:45:49 raspberrypi sshd[18361]: Failed password for root from 221.231.139.150 port 2799 ssh2
Mar 31 20:45:51 raspberrypi sshd[18369]: Failed password for root from 221.231.139.150 port 2806 ssh2
Mar 31 20:45:52 raspberrypi sshd[18361]: Failed password for root from 221.231.139.150 port 2799 ssh2
Mar 31 20:45:53 raspberrypi sshd[18369]: Failed password for root from 221.231.139.150 port 2806 ssh2
Mar 31 20:45:53 raspberrypi sshd[18369]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2806 ssh2 [preauth]
Mar 31 20:45:53 raspberrypi sshd[18369]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:53 raspberrypi sshd[18397]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:55 raspberrypi sshd[18361]: Failed password for root from 221.231.139.150 port 2799 ssh2
Mar 31 20:45:56 raspberrypi sshd[18397]: Failed password for root from 221.231.139.150 port 3180 ssh2
Mar 31 20:45:57 raspberrypi sshd[18361]: Failed password for root from 221.231.139.150 port 2799 ssh2
Mar 31 20:45:57 raspberrypi sshd[18361]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2799 ssh2 [preauth]
Mar 31 20:45:57 raspberrypi sshd[18361]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:45:57 raspberrypi sshd[18397]: Failed password for root from 221.231.139.150 port 3180 ssh2
Mar 31 20:45:58 raspberrypi sshd[18410]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:00 raspberrypi sshd[18397]: Failed password for root from 221.231.139.150 port 3180 ssh2
Mar 31 20:46:00 raspberrypi sshd[18410]: Failed password for root from 221.231.139.150 port 3294 ssh2
Mar 31 20:46:02 raspberrypi sshd[18397]: Failed password for root from 221.231.139.150 port 3180 ssh2
Mar 31 20:46:02 raspberrypi sshd[18410]: Failed password for root from 221.231.139.150 port 3294 ssh2
Mar 31 20:46:04 raspberrypi sshd[18397]: Failed password for root from 221.231.139.150 port 3180 ssh2
Mar 31 20:46:04 raspberrypi sshd[18410]: Failed password for root from 221.231.139.150 port 3294 ssh2
Mar 31 20:46:07 raspberrypi sshd[18397]: Failed password for root from 221.231.139.150 port 3180 ssh2
Mar 31 20:46:07 raspberrypi sshd[18397]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3180 ssh2 [preauth]
Mar 31 20:46:07 raspberrypi sshd[18397]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:07 raspberrypi sshd[18410]: Failed password for root from 221.231.139.150 port 3294 ssh2
Mar 31 20:46:08 raspberrypi sshd[18453]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:09 raspberrypi sshd[18410]: Failed password for root from 221.231.139.150 port 3294 ssh2
Mar 31 20:46:09 raspberrypi sshd[18453]: Failed password for root from 221.231.139.150 port 3567 ssh2
Mar 31 20:46:12 raspberrypi sshd[18410]: Failed password for root from 221.231.139.150 port 3294 ssh2
Mar 31 20:46:12 raspberrypi sshd[18410]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3294 ssh2 [preauth]
Mar 31 20:46:12 raspberrypi sshd[18410]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:12 raspberrypi sshd[18453]: Failed password for root from 221.231.139.150 port 3567 ssh2
Mar 31 20:46:14 raspberrypi sshd[18466]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:15 raspberrypi sshd[18453]: Failed password for root from 221.231.139.150 port 3567 ssh2
Mar 31 20:46:16 raspberrypi sshd[18466]: Failed password for root from 221.231.139.150 port 3679 ssh2
Mar 31 20:46:17 raspberrypi sshd[18453]: Failed password for root from 221.231.139.150 port 3567 ssh2
Mar 31 20:46:19 raspberrypi sshd[18466]: Failed password for root from 221.231.139.150 port 3679 ssh2
Mar 31 20:46:19 raspberrypi sshd[18453]: Failed password for root from 221.231.139.150 port 3567 ssh2
Mar 31 20:46:21 raspberrypi sshd[18466]: Failed password for root from 221.231.139.150 port 3679 ssh2
Mar 31 20:46:21 raspberrypi sshd[18453]: Failed password for root from 221.231.139.150 port 3567 ssh2
Mar 31 20:46:21 raspberrypi sshd[18453]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3567 ssh2 [preauth]
Mar 31 20:46:21 raspberrypi sshd[18453]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:22 raspberrypi sshd[18490]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:23 raspberrypi sshd[18466]: Failed password for root from 221.231.139.150 port 3679 ssh2
Mar 31 20:46:24 raspberrypi sshd[18490]: Failed password for root from 221.231.139.150 port 3946 ssh2
Mar 31 20:46:26 raspberrypi sshd[18466]: Failed password for root from 221.231.139.150 port 3679 ssh2
Mar 31 20:46:26 raspberrypi sshd[18490]: Failed password for root from 221.231.139.150 port 3946 ssh2
Mar 31 20:46:28 raspberrypi sshd[18466]: Failed password for root from 221.231.139.150 port 3679 ssh2
Mar 31 20:46:28 raspberrypi sshd[18466]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3679 ssh2 [preauth]
Mar 31 20:46:28 raspberrypi sshd[18466]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:28 raspberrypi sshd[18490]: Failed password for root from 221.231.139.150 port 3946 ssh2
Mar 31 20:46:30 raspberrypi sshd[18508]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:30 raspberrypi sshd[18490]: Failed password for root from 221.231.139.150 port 3946 ssh2
Mar 31 20:46:31 raspberrypi sshd[18508]: Failed password for root from 221.231.139.150 port 4124 ssh2
Mar 31 20:46:33 raspberrypi sshd[18490]: Failed password for root from 221.231.139.150 port 3946 ssh2
Mar 31 20:46:34 raspberrypi sshd[18508]: Failed password for root from 221.231.139.150 port 4124 ssh2
Mar 31 20:46:35 raspberrypi sshd[18490]: Failed password for root from 221.231.139.150 port 3946 ssh2
Mar 31 20:46:35 raspberrypi sshd[18490]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3946 ssh2 [preauth]
Mar 31 20:46:35 raspberrypi sshd[18490]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:36 raspberrypi sshd[18528]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:36 raspberrypi sshd[18508]: Failed password for root from 221.231.139.150 port 4124 ssh2
Mar 31 20:46:38 raspberrypi sshd[18528]: Failed password for root from 221.231.139.150 port 4370 ssh2
Mar 31 20:46:39 raspberrypi sshd[18508]: Failed password for root from 221.231.139.150 port 4124 ssh2
Mar 31 20:46:40 raspberrypi sshd[18528]: Failed password for root from 221.231.139.150 port 4370 ssh2
Mar 31 20:46:41 raspberrypi sshd[18508]: Failed password for root from 221.231.139.150 port 4124 ssh2
Mar 31 20:46:42 raspberrypi sshd[18528]: Failed password for root from 221.231.139.150 port 4370 ssh2
Mar 31 20:46:43 raspberrypi sshd[18508]: Failed password for root from 221.231.139.150 port 4124 ssh2
Mar 31 20:46:43 raspberrypi sshd[18508]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4124 ssh2 [preauth]
Mar 31 20:46:43 raspberrypi sshd[18508]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:44 raspberrypi sshd[18550]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:44 raspberrypi sshd[18528]: Failed password for root from 221.231.139.150 port 4370 ssh2
Mar 31 20:46:46 raspberrypi sshd[18550]: Failed password for root from 221.231.139.150 port 4636 ssh2
Mar 31 20:46:46 raspberrypi sshd[18528]: Failed password for root from 221.231.139.150 port 4370 ssh2
Mar 31 20:46:49 raspberrypi sshd[18550]: Failed password for root from 221.231.139.150 port 4636 ssh2
Mar 31 20:46:49 raspberrypi sshd[18528]: Failed password for root from 221.231.139.150 port 4370 ssh2
Mar 31 20:46:49 raspberrypi sshd[18528]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4370 ssh2 [preauth]
Mar 31 20:46:49 raspberrypi sshd[18528]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:50 raspberrypi sshd[18567]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:51 raspberrypi sshd[18550]: Failed password for root from 221.231.139.150 port 4636 ssh2
Mar 31 20:46:52 raspberrypi sshd[18567]: Failed password for root from 221.231.139.150 port 4852 ssh2
Mar 31 20:46:53 raspberrypi sshd[18550]: Failed password for root from 221.231.139.150 port 4636 ssh2
Mar 31 20:46:54 raspberrypi sshd[18567]: Failed password for root from 221.231.139.150 port 4852 ssh2
Mar 31 20:46:55 raspberrypi sshd[18550]: Failed password for root from 221.231.139.150 port 4636 ssh2
Mar 31 20:46:55 raspberrypi sshd[18567]: Failed password for root from 221.231.139.150 port 4852 ssh2
Mar 31 20:46:58 raspberrypi sshd[18550]: Failed password for root from 221.231.139.150 port 4636 ssh2
Mar 31 20:46:58 raspberrypi sshd[18550]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4636 ssh2 [preauth]
Mar 31 20:46:58 raspberrypi sshd[18550]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:46:58 raspberrypi sshd[18567]: Failed password for root from 221.231.139.150 port 4852 ssh2
Mar 31 20:47:00 raspberrypi sshd[18589]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:01 raspberrypi sshd[18567]: Failed password for root from 221.231.139.150 port 4852 ssh2
Mar 31 20:47:03 raspberrypi sshd[18589]: Failed password for root from 221.231.139.150 port 1138 ssh2
Mar 31 20:47:03 raspberrypi sshd[18567]: Failed password for root from 221.231.139.150 port 4852 ssh2
Mar 31 20:47:03 raspberrypi sshd[18567]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4852 ssh2 [preauth]
Mar 31 20:47:03 raspberrypi sshd[18567]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:04 raspberrypi sshd[18621]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:05 raspberrypi sshd[18589]: Failed password for root from 221.231.139.150 port 1138 ssh2
Mar 31 20:47:05 raspberrypi sshd[18621]: Failed password for root from 221.231.139.150 port 1236 ssh2
Mar 31 20:47:07 raspberrypi sshd[18589]: Failed password for root from 221.231.139.150 port 1138 ssh2
Mar 31 20:47:08 raspberrypi sshd[18621]: Failed password for root from 221.231.139.150 port 1236 ssh2
Mar 31 20:47:10 raspberrypi sshd[18621]: Failed password for root from 221.231.139.150 port 1236 ssh2
Mar 31 20:47:10 raspberrypi sshd[18589]: Failed password for root from 221.231.139.150 port 1138 ssh2
Mar 31 20:47:12 raspberrypi sshd[18621]: Failed password for root from 221.231.139.150 port 1236 ssh2
Mar 31 20:47:12 raspberrypi sshd[18589]: Failed password for root from 221.231.139.150 port 1138 ssh2
Mar 31 20:47:14 raspberrypi sshd[18621]: Failed password for root from 221.231.139.150 port 1236 ssh2
Mar 31 20:47:15 raspberrypi sshd[18589]: Failed password for root from 221.231.139.150 port 1138 ssh2
Mar 31 20:47:15 raspberrypi sshd[18589]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1138 ssh2 [preauth]
Mar 31 20:47:15 raspberrypi sshd[18589]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:15 raspberrypi sshd[18649]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:16 raspberrypi sshd[18621]: Failed password for root from 221.231.139.150 port 1236 ssh2
Mar 31 20:47:16 raspberrypi sshd[18621]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1236 ssh2 [preauth]
Mar 31 20:47:16 raspberrypi sshd[18621]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:17 raspberrypi sshd[18649]: Failed password for root from 221.231.139.150 port 1474 ssh2
Mar 31 20:47:19 raspberrypi sshd[18649]: Failed password for root from 221.231.139.150 port 1474 ssh2
Mar 31 20:47:19 raspberrypi sshd[18658]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:22 raspberrypi sshd[18649]: Failed password for root from 221.231.139.150 port 1474 ssh2
Mar 31 20:47:22 raspberrypi sshd[18658]: Failed password for root from 221.231.139.150 port 1517 ssh2
Mar 31 20:47:24 raspberrypi sshd[18649]: Failed password for root from 221.231.139.150 port 1474 ssh2
Mar 31 20:47:25 raspberrypi sshd[18658]: Failed password for root from 221.231.139.150 port 1517 ssh2
Mar 31 20:47:27 raspberrypi sshd[18658]: Failed password for root from 221.231.139.150 port 1517 ssh2
Mar 31 20:47:27 raspberrypi sshd[18649]: Failed password for root from 221.231.139.150 port 1474 ssh2
Mar 31 20:47:28 raspberrypi sshd[18658]: Failed password for root from 221.231.139.150 port 1517 ssh2
Mar 31 20:47:29 raspberrypi sshd[18649]: Failed password for root from 221.231.139.150 port 1474 ssh2
Mar 31 20:47:29 raspberrypi sshd[18649]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1474 ssh2 [preauth]
Mar 31 20:47:29 raspberrypi sshd[18649]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:29 raspberrypi sshd[18687]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:30 raspberrypi sshd[18658]: Failed password for root from 221.231.139.150 port 1517 ssh2
Mar 31 20:47:31 raspberrypi sshd[18687]: Failed password for root from 221.231.139.150 port 1770 ssh2
Mar 31 20:47:33 raspberrypi sshd[18658]: Failed password for root from 221.231.139.150 port 1517 ssh2
Mar 31 20:47:33 raspberrypi sshd[18658]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1517 ssh2 [preauth]
Mar 31 20:47:33 raspberrypi sshd[18658]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:34 raspberrypi sshd[18687]: Failed password for root from 221.231.139.150 port 1770 ssh2
Mar 31 20:47:34 raspberrypi sshd[18700]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:36 raspberrypi sshd[18700]: Failed password for root from 221.231.139.150 port 1842 ssh2
Mar 31 20:47:36 raspberrypi sshd[18687]: Failed password for root from 221.231.139.150 port 1770 ssh2
Mar 31 20:47:38 raspberrypi sshd[18700]: Failed password for root from 221.231.139.150 port 1842 ssh2
Mar 31 20:47:39 raspberrypi sshd[18687]: Failed password for root from 221.231.139.150 port 1770 ssh2
Mar 31 20:47:40 raspberrypi sshd[18700]: Failed password for root from 221.231.139.150 port 1842 ssh2
Mar 31 20:47:40 raspberrypi sshd[18687]: Failed password for root from 221.231.139.150 port 1770 ssh2
Mar 31 20:47:42 raspberrypi sshd[18700]: Failed password for root from 221.231.139.150 port 1842 ssh2
Mar 31 20:47:42 raspberrypi sshd[18687]: Failed password for root from 221.231.139.150 port 1770 ssh2
Mar 31 20:47:42 raspberrypi sshd[18687]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1770 ssh2 [preauth]
Mar 31 20:47:42 raspberrypi sshd[18687]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:44 raspberrypi sshd[18725]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:45 raspberrypi sshd[18700]: Failed password for root from 221.231.139.150 port 1842 ssh2
Mar 31 20:47:46 raspberrypi sshd[18725]: Failed password for root from 221.231.139.150 port 2003 ssh2
Mar 31 20:47:47 raspberrypi sshd[18700]: Failed password for root from 221.231.139.150 port 1842 ssh2
Mar 31 20:47:47 raspberrypi sshd[18700]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1842 ssh2 [preauth]
Mar 31 20:47:47 raspberrypi sshd[18700]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:48 raspberrypi sshd[18725]: Failed password for root from 221.231.139.150 port 2003 ssh2
Mar 31 20:47:48 raspberrypi sshd[18738]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:50 raspberrypi sshd[18725]: Failed password for root from 221.231.139.150 port 2003 ssh2
Mar 31 20:47:51 raspberrypi sshd[18738]: Failed password for root from 221.231.139.150 port 2104 ssh2
Mar 31 20:47:52 raspberrypi sshd[18725]: Failed password for root from 221.231.139.150 port 2003 ssh2
Mar 31 20:47:52 raspberrypi sshd[18738]: Failed password for root from 221.231.139.150 port 2104 ssh2
Mar 31 20:47:54 raspberrypi sshd[18725]: Failed password for root from 221.231.139.150 port 2003 ssh2
Mar 31 20:47:54 raspberrypi sshd[18738]: Failed password for root from 221.231.139.150 port 2104 ssh2
Mar 31 20:47:57 raspberrypi sshd[18725]: Failed password for root from 221.231.139.150 port 2003 ssh2
Mar 31 20:47:57 raspberrypi sshd[18725]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2003 ssh2 [preauth]
Mar 31 20:47:57 raspberrypi sshd[18725]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:57 raspberrypi sshd[18738]: Failed password for root from 221.231.139.150 port 2104 ssh2
Mar 31 20:47:57 raspberrypi sshd[18762]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:47:59 raspberrypi sshd[18738]: Failed password for root from 221.231.139.150 port 2104 ssh2
Mar 31 20:47:59 raspberrypi sshd[18762]: Failed password for root from 221.231.139.150 port 2256 ssh2
Mar 31 20:48:02 raspberrypi sshd[18738]: Failed password for root from 221.231.139.150 port 2104 ssh2
Mar 31 20:48:02 raspberrypi sshd[18738]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2104 ssh2 [preauth]
Mar 31 20:48:02 raspberrypi sshd[18738]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:02 raspberrypi sshd[18762]: Failed password for root from 221.231.139.150 port 2256 ssh2
Mar 31 20:48:03 raspberrypi sshd[18762]: Failed password for root from 221.231.139.150 port 2256 ssh2
Mar 31 20:48:05 raspberrypi sshd[18762]: Failed password for root from 221.231.139.150 port 2256 ssh2
Mar 31 20:48:05 raspberrypi sshd[18796]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:07 raspberrypi sshd[18762]: Failed password for root from 221.231.139.150 port 2256 ssh2
Mar 31 20:48:07 raspberrypi sshd[18796]: Failed password for root from 221.231.139.150 port 2409 ssh2
Mar 31 20:48:09 raspberrypi sshd[18762]: Failed password for root from 221.231.139.150 port 2256 ssh2
Mar 31 20:48:09 raspberrypi sshd[18762]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2256 ssh2 [preauth]
Mar 31 20:48:09 raspberrypi sshd[18762]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:09 raspberrypi sshd[18796]: Failed password for root from 221.231.139.150 port 2409 ssh2
Mar 31 20:48:10 raspberrypi sshd[18816]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:11 raspberrypi sshd[18796]: Failed password for root from 221.231.139.150 port 2409 ssh2
Mar 31 20:48:11 raspberrypi sshd[18816]: Failed password for root from 221.231.139.150 port 2743 ssh2
Mar 31 20:48:13 raspberrypi sshd[18796]: Failed password for root from 221.231.139.150 port 2409 ssh2
Mar 31 20:48:14 raspberrypi sshd[18816]: Failed password for root from 221.231.139.150 port 2743 ssh2
Mar 31 20:48:15 raspberrypi sshd[18816]: Failed password for root from 221.231.139.150 port 2743 ssh2
Mar 31 20:48:15 raspberrypi sshd[18796]: Failed password for root from 221.231.139.150 port 2409 ssh2
Mar 31 20:48:17 raspberrypi sshd[18816]: Failed password for root from 221.231.139.150 port 2743 ssh2
Mar 31 20:48:17 raspberrypi sshd[18796]: Failed password for root from 221.231.139.150 port 2409 ssh2
Mar 31 20:48:17 raspberrypi sshd[18796]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2409 ssh2 [preauth]
Mar 31 20:48:17 raspberrypi sshd[18796]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:18 raspberrypi sshd[18839]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:19 raspberrypi sshd[18816]: Failed password for root from 221.231.139.150 port 2743 ssh2
Mar 31 20:48:21 raspberrypi sshd[18839]: Failed password for root from 221.231.139.150 port 3596 ssh2
Mar 31 20:48:22 raspberrypi sshd[18816]: Failed password for root from 221.231.139.150 port 2743 ssh2
Mar 31 20:48:22 raspberrypi sshd[18816]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 2743 ssh2 [preauth]
Mar 31 20:48:22 raspberrypi sshd[18816]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:22 raspberrypi sshd[18839]: Failed password for root from 221.231.139.150 port 3596 ssh2
Mar 31 20:48:24 raspberrypi sshd[18852]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:25 raspberrypi sshd[18839]: Failed password for root from 221.231.139.150 port 3596 ssh2
Mar 31 20:48:26 raspberrypi sshd[18852]: Failed password for root from 221.231.139.150 port 4160 ssh2
Mar 31 20:48:27 raspberrypi sshd[18839]: Failed password for root from 221.231.139.150 port 3596 ssh2
Mar 31 20:48:27 raspberrypi sshd[18852]: Failed password for root from 221.231.139.150 port 4160 ssh2
Mar 31 20:48:28 raspberrypi sshd[18839]: Failed password for root from 221.231.139.150 port 3596 ssh2
Mar 31 20:48:29 raspberrypi sshd[18852]: Failed password for root from 221.231.139.150 port 4160 ssh2
Mar 31 20:48:30 raspberrypi sshd[18839]: Failed password for root from 221.231.139.150 port 3596 ssh2
Mar 31 20:48:30 raspberrypi sshd[18839]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3596 ssh2 [preauth]
Mar 31 20:48:30 raspberrypi sshd[18839]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:31 raspberrypi sshd[18876]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:31 raspberrypi sshd[18852]: Failed password for root from 221.231.139.150 port 4160 ssh2
Mar 31 20:48:33 raspberrypi sshd[18876]: Failed password for root from 221.231.139.150 port 1428 ssh2
Mar 31 20:48:34 raspberrypi sshd[18852]: Failed password for root from 221.231.139.150 port 4160 ssh2
Mar 31 20:48:35 raspberrypi sshd[18876]: Failed password for root from 221.231.139.150 port 1428 ssh2
Mar 31 20:48:36 raspberrypi sshd[18852]: Failed password for root from 221.231.139.150 port 4160 ssh2
Mar 31 20:48:36 raspberrypi sshd[18852]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 4160 ssh2 [preauth]
Mar 31 20:48:36 raspberrypi sshd[18852]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:36 raspberrypi sshd[18893]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:37 raspberrypi sshd[18876]: Failed password for root from 221.231.139.150 port 1428 ssh2
Mar 31 20:48:38 raspberrypi sshd[18893]: Failed password for root from 221.231.139.150 port 1971 ssh2
Mar 31 20:48:40 raspberrypi sshd[18876]: Failed password for root from 221.231.139.150 port 1428 ssh2
Mar 31 20:48:40 raspberrypi sshd[18876]: Connection closed by 221.231.139.150 [preauth]
Mar 31 20:48:40 raspberrypi sshd[18876]: PAM 3 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:40 raspberrypi sshd[18893]: Failed password for root from 221.231.139.150 port 1971 ssh2
Mar 31 20:48:42 raspberrypi sshd[18893]: Failed password for root from 221.231.139.150 port 1971 ssh2
Mar 31 20:48:45 raspberrypi sshd[18893]: Failed password for root from 221.231.139.150 port 1971 ssh2
Mar 31 20:48:47 raspberrypi sshd[18893]: Failed password for root from 221.231.139.150 port 1971 ssh2
Mar 31 20:48:49 raspberrypi sshd[18893]: Failed password for root from 221.231.139.150 port 1971 ssh2
Mar 31 20:48:49 raspberrypi sshd[18893]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 1971 ssh2 [preauth]
Mar 31 20:48:49 raspberrypi sshd[18893]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:49 raspberrypi sshd[18923]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:48:52 raspberrypi sshd[18923]: Failed password for root from 221.231.139.150 port 3085 ssh2
Mar 31 20:48:54 raspberrypi sshd[18923]: Failed password for root from 221.231.139.150 port 3085 ssh2
Mar 31 20:48:56 raspberrypi sshd[18923]: Failed password for root from 221.231.139.150 port 3085 ssh2
Mar 31 20:48:58 raspberrypi sshd[18923]: Failed password for root from 221.231.139.150 port 3085 ssh2
Mar 31 20:49:00 raspberrypi sshd[18923]: Failed password for root from 221.231.139.150 port 3085 ssh2
Mar 31 20:49:02 raspberrypi sshd[18923]: Failed password for root from 221.231.139.150 port 3085 ssh2
Mar 31 20:49:02 raspberrypi sshd[18923]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3085 ssh2 [preauth]
Mar 31 20:49:02 raspberrypi sshd[18923]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:49:03 raspberrypi sshd[18961]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:49:05 raspberrypi sshd[18961]: Failed password for root from 221.231.139.150 port 3855 ssh2
Mar 31 20:49:07 raspberrypi sshd[18961]: Failed password for root from 221.231.139.150 port 3855 ssh2
Mar 31 20:49:09 raspberrypi sshd[18961]: Failed password for root from 221.231.139.150 port 3855 ssh2
Mar 31 20:49:11 raspberrypi sshd[18961]: Failed password for root from 221.231.139.150 port 3855 ssh2
Mar 31 20:49:13 raspberrypi sshd[18961]: Failed password for root from 221.231.139.150 port 3855 ssh2
Mar 31 20:49:16 raspberrypi sshd[18961]: Failed password for root from 221.231.139.150 port 3855 ssh2
Mar 31 20:49:16 raspberrypi sshd[18961]: Disconnecting: Too many authentication failures for root from 221.231.139.150 port 3855 ssh2 [preauth]
Mar 31 20:49:16 raspberrypi sshd[18961]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:49:16 raspberrypi sshd[18984]: pam_unix(sshd:auth): authentication failure; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root
Mar 31 20:49:18 raspberrypi sshd[18984]: Failed password for root from 221.231.139.150 port 4500 ssh2
Mar 31 20:49:21 raspberrypi sshd[18984]: Failed password for root from 221.231.139.150 port 4500 ssh2
Mar 31 20:49:22 raspberrypi sshd[18984]: Failed password for root from 221.231.139.150 port 4500 ssh2
Mar 31 20:49:24 raspberrypi sshd[18984]: Failed password for root from 221.231.139.150 port 4500 ssh2
Mar 31 20:49:24 raspberrypi sshd[18984]: Connection closed by 221.231.139.150 [preauth]
Mar 31 20:49:24 raspberrypi sshd[18984]: PAM 3 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=221.231.139.150  user=root


```



 来自 俄罗斯 和 江苏镇江的  root 尝试登陆

![1](https://dn-shimo-image.qbox.me/zt8HPnUvjogzqXJU.png)



![13](https://dn-shimo-image.qbox.me/KQ4aLFmfYJoltnnG.png)



大量 auth.log日志记录发现 ，被入侵后 好像给我生成了某些cron脚本，导致频繁执行，
在删掉某用户后，提示不能找到什么云云。
![2](https://dn-shimo-image.qbox.me/I7H3zU83OQUcYIcy.png!thumbnail)
![3](https://dn-shimo-image.qbox.me/50nKPo024uASlo1l.png)
被 fail2ban记录禁止的 来自 美国vps的攻击尝试。

![11](https://dn-shimo-image.qbox.me/88HCllAhcPYHCtZy.png)

原来 是给我的 cron写入一个每时每刻每分每秒都在执行的任务，。。。。。。。
![10](https://dn-shimo-image.qbox.me/tom2B8mF14US6oyx.png)
特么的 服。。。。

 date:  2016年 04月 02日 星期六 22:30:33 CST
 ![16](https://dn-shimo-image.qbox.me/ljiJ4HmcL1E4UulJ.png)
 又开始了。
 ![17](https://dn-shimo-image.qbox.me/2NeNOKhHJWgV5wkZ.png)
