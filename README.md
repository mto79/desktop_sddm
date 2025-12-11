

## Install


- [`For Fedora Linux`]
`sddm` `qt6-qtsvg` `qt6-qtvirtualkeyboard` `qt6-qtmultimedia`

## Configure

Edit the or create if it does not exist `/etc/sddm.conf` (with any text editor with **raised** privileges), so that it looks like this:

```bash
sudo nano /etc/sddm.conf # use any text editor with raised privileges
```

add this lines

```sh
[Theme]
Current=simple_sddm_2

[General]
InputMethod=qtvirtualkeyboard

```


### Language and time format
- By default, it is configured with 24H format. You can change to AM/PM variant by editing the theme.conf
```bash
sudo nano /usr/share/sddm/themes/simple_sddm_2/theme.conf  # use any text editor with raised privileges
```
- `HourFormat="hh:mm AP` . Make sure to disable the above of this part

### 🖼️ Default SDDM background
- To change the default background, put desired image in the `/usr/share/sddm/themes/simple_sddm_2/Backgrounds/` folder and add the name of the image followed by its extension (`.jpg` or `.png`) in `theme.conf` file.

- You can also customize it further if you wish in the `/usr/share/sddm/themes/simple_sddm_2/theme.conf`
(blur, form position, etc).



