Base PC2 Configurations for Java practice contests

pc2-x.x.x-base.zip has unnecessary elements deleted.

pc2-x.x.x-initial.zip has contest password, language, and scoring already set up.

pc2-x.x.x-team.zip has the only the essential team files.

## Notes
Set up initial and base configs in Linux/Mac when new versions are released. The Profile generated by Windows uses `\` path delimiters, which do not work with Linux/Mac.

These configurations are intended for practice contests. They are not guaranteed to work for actual contests (especially web elements like scoreboard).

## Standardization
Adhere to these rules if a contest will potentially be setup/run/transferred across computers.

**Use hyphens as filename delimiters**

Use Git LFS to store large files to save disk space
  - **NOTE:** will require all contributors to have git-lfs installed

Use a Windows account named `PC2`.
  - clone repos to `C:\Users\PC2\Desktop`
  - Judge data path should generally be `C:\Users\PC2\Desktop\${repo-name}\JudgeData`

Site 1 Server IP should be `192.168.1.2`
  - Reserve this IP on the contest router
  - Make sure to change IPs in `pc2v9.ini` before committing

## team pc2 zip file
make sure server has been zipped

delete everything in bin except
  - pc2env*
  - pc2team*
  - pc2v9.ini
