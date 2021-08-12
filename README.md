# Remote Control Infrared Codes

#### Note

Repeat codes in both remotes mean that
the button pressed is transmitted once,
then while the button is still pressed, it
sends out the repeat code.
When you let go of the button and 
press a key again, the button code is 
transmitted again once, folowed by the
the repeat code for as long as the button
is pressed.

## LG 42" LCD TV

**Repeat code:** `FFFF FFFF`

| Button | Code |
| --- | --- |
| Power on/off | ` 20DF 10EF` |
| Switch to TV | ` 20DF F00F` |
| Caption | ` 20DF 9C63` |
| Settings | ` 20DF C23D` |
| Search | ` 20DF 1EE1` |
| Choose input | ` 20DF D02F` |
| Channel 1 | ` 20DF 8877` |
| Channel 2 | ` 20DF 48B7` |
| Channel 3 | ` 20DF C837` |
| Channel 4 | ` 20DF 28D7` |
| Channel 5 | ` 20DF A857` |
| Channel 6 | ` 20DF 6897` |
| Channel 7 | ` 20DF E817` |
| Channel 8 | ` 20DF 18E7` |
| Channel 9 | ` 20DF 9867` |
| LIST / - | ` 20DF 32CD` |
| Channel 0 | ` 20DF 08F7` |
| Q-View | ` 20DF 58AF` |
| Vol Up | ` 20DF 40BF` |
| Vol Down | ` 20DF C03F` |
| Favorites | ` 20DF 7887` |
| Info | ` 20DF 55AA` |
| Mute | ` 20DF 906F` |
| Page Up | ` 20DF 00FF` |
| Page Down | ` 20DF 807F` |
| Recent | ` 20DF AD52` |
| Home | ` 20DF 3EC1` |
| Live Menu | ` 20DF 7986` |
| Guide | ` 20DF D52A` |
| Up | ` 20DF 02FD` |
| Live Zoom | ` 20DF F50A` |
| Left | ` 20DF E01F` |
| OK | ` 20DF 22DD` |
| Right | ` 20DF 609F` |
| Back | ` 20DF 14EB` |
| Down | ` 20DF 827D` |
| Exit | ` 20DF DA25` |
| Help | ` 20DF 5EA1` |
| RECORD | ` 20DF BD42` |
| Stop | ` 20DF 8D72` |
| Rewind | ` 20DF F10E` |
| Play | ` 20DF 0DF2` |
| Pause | ` 20DF 5DA2` |
| Fast forward | ` 20DF 718E` |
| RED / 1 | ` 20DF 4EB1` |
| Green / 2 | ` 20DF 8E71` |
| Yellow / 3 | ` 20DF C639` |
| Blue / 4 | ` 20DF 8679` |

## LG DVD Home Theater

### Main Buttons

**Repeat code:** `4AB0 F7B6`

| Button | Code |
| --- | --- |
| Input selection | ` F789 1447` |
| Disk skip | ` 6C78 F3A1` |
| Power | ` 876E 1365` |
| Eject | ` EE10 70C3` |
| Sleep | ` 6D2D D746` |
| Info / Display | ` 3509 A4A2` |
| Home | ` 8CE0 9A02` |
| Disc menu | ` DC0D 357E` |
| Up | ` 227A 8EDE` |
| Left | ` 7139 0566` |
| Enter | ` 2A27 E402` |
| Right | ` C71E C262` |
| Down | ` 961B 05E2` |
| Return | ` A8AA 1BA6` |
| Title | ` 67AD 1002` |
| Stop | ` A014 D267` |
| Play | ` 6C2F 5EA1` |
| Pause / Step | ` 7EB6 A3A3` |
| Previous | ` 263D 2F05` |
| Rewind | ` ADD6 B687` |
| Fast forward | ` 259D CA41` |
| Next | ` E4F9 FE83` |
| Auto DJ | ` A310 6F7E` |
| Sound effects | ` 8AB C10A1` |
| Volume Up | ` 506A 9BC7` |
| Volume down | ` DBCB 3A41` |
| Speaker level | ` E75E 041D` |
| Mute | ` DBA4 FE23` |
| Channel 1 | ` 2618 E067` |
| Channel 2 | ` 9798 77C5` |
| Channel 3 | ` 1581 8B03` |
| Marker | ` 4724 A8A2` |
| Channel 4 | ` CAFB 919D` |
| Channel 5 | ` D79B 6363` |
| Channel 6 | ` 8509 6201` |
| Repeat | ` CA3B E325` |
| Channel 7 | ` E30B AAC7` |
| Channel 8 | ` 6027 6185` |
| Channel 9 | ` 6852 037B` |
| Channel 0 | ` E0A4 72DF` |
| Record | ` 984C 2B23` |
| Clear | ` 5E9A D67E` |
| Mic vol up | ` 8E2B E102` |
| Echo vol up | ` 20CD CA62` |
| Mic vol down | ` F72B 59DE` |
| Echo vol down | ` B139 2A42` |
| Vocal fader | ` 5ABB AE65` |

### Built-in TV buttons

The LG DVD Home Theater
remote has a small section dedicated to
controlling a TV (I guess of its time, it's
obviously incompatible with my LG 42"
LCD TV), which employs a different
method for long-presses that doesn't
involve a repeat code.

These codes, unlike the buttons above,
do not use a repeat
signal, meaning even if you long-press
a button, it will keep sending the same
signal. However, everytime you press a
button, it toggles a mask, from 
0000 to 0800 and vice versa.
This mask is ORed with the button
code, affecting the final signal
transmitted. That means the first time
you press POWER ON, it sends 000C
(even if you long press). But the next
time you press it (or any other key),
the value is now ORed with 0800,
meaning the signal transmitted is now
08xx (08C0, if POWER ON)
Next time you press any other button,
it's 00xx (00C0 if POWER ON).

| Button | Code |
| --- | --- |
| Power on | ` 0C` |
| Channel Up | ` 20` |
| Volume up | ` 10` |
| AV/Input Toggle | ` 38` |
| Channel down | ` 21` |
| Volume down | ` 11` |
