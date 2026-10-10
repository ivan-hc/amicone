## Usage
1. Create the missing-icons.txt file by cloning and entering the catalogue's repository:
```
git clone https://github.com/Portable-Linux-Apps/Portable-Linux-Apps.github.io.git
cd Portable-Linux-Apps.github.io/
for a in apps/*; do a=$(echo "$a" | sed 's#apps/##g'); [ ! -f icons/"$a".png ] && echo "$a" >> missing-icons.txt; done
```
2. Upload the resulting file to the root of this repository and run the workflow
3. Download the artifact
4. Extract and convert all icons to 128x128 PNG files
5. Upload the icons to https://github.com/Portable-Linux-Apps/Portable-Linux-Apps.github.io/tree/main/icons

NOTE: If the icons have not been extracted, wait for improvements to the ["AM" package manager](https://github.com/ivan-hc/AM) or proceed manually.
