## This is probably the shittiest code ever written; please don't use this; this just fixed a lot of graphical issue's I had with Studio and how it woun't create a stable link each installation, and a whole other magnitude of issues. It is basically just a stack with a lot of old troubleshooting.


<div style="display: flex; align-items: center;">
    <img src="https://github.com/fnstart/StudioFinder/blob/main/bin/logo.png?raw=true" alt="Logo" style="width: 100px; margin-right: 20px;">
    <h1>StudioFinder - @fnstart</h1>
</div>

<img src="https://github.com/fnstart/StudioFinder/blob/main/img1.png?raw=true" alt="Showcase1" style="width: 65%;">
<img src="https://github.com/fnstart/StudioFinder/blob/main/img2.png?raw=true" alt="Showcase2" style="width: 35%;">

## Install/Update Command  [MAKEPKG]
```sh
wget https://github.com/fnstart/StudioFinder/releases/latest/download/release.tar.gz
```
```sh
tar -xvzf release.tar.gz && mv bin StudioFinder
cd StudioFinder
makepkg -s --noconfirm --install
```

## Install/Update Command [OLD]
```sh
curl -s https://api.github.com/repos/fnstart/StudioFinder/releases/latest | grep "browser_download_url.*release.tar.gz" | cut -d : -f 2,3 | tr -d \" | wget -qi - -O - | tar -xz -C ~/ && sleep 1 && bash ~/StudioFinder/install.sh
```
