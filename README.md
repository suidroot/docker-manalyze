This is dockerfile image for manalyze (https://github.com/JusticeRage/Manalyze)


# Usage


`docker pull evanowe/manalyze:latest`

or

`docker build -t manalyze .`

## Scan folder with malware samples

```bash
cd /malwares
docker run -it --rm -v `pwd`:/data evanowe/manalyze /Manalyze/bin/manalyze -p all -r /data/
```

## Scan one file

```bash
docker run -it --rm -v `pwd`:/data evanowe/manalyze /Manalyze/bin/manalyze -p all /data/malware_sample
```

## You can make alias in bashrc/zshrc:

```bash
alias manalyze='docker run -it --rm -v `pwd`:/data evanowe/manalyze /Manalyze/bin/manalyze'
```

