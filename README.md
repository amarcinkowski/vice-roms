vice-roms
=========

I became tired of manually copying over the Commodore ROMs whenever I decide to go for a fresh reinstall, so that's why I set up this repo.

Usage
-----
```bash
cd ~/git
git clone https://github.com/amarcinkowski/vice-roms
cat <<EOF >> ~/.zshrc
ROMSPATH="$HOME/git/vice-roms"
alias xx='x64sc +confirmonexit -saveres -basic "$ROMSPATH/C64/basic" -chargen "$ROMSPATH/C64/chargen" -kernal "$ROMSPATH/C64/kernal"  +VICIIdsize +VICIIdscan -VICIIextpal -VICIIpalette "colodore"'
EOF
```
