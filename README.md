# Git Large File Storage

## Prepare a new git repository

git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/thomaschang710114/large-file-goodbuy.git
git push -u origin main

## On local dev environment

- `brew install git-lfs`
- Verity the installation `git lfs install`
  - Should output `Git LFS initialized.`
- Track file `git lfs track "*.csv"`
  - Output `Tracking "*.csv"`
  - .gitattributes shows `*.csv filter=lfs diff=lfs merge=lfs -text`
- `git lfs push --all origin main`

## Push to main

- `git add .`
- `git commit -m "update by 20240708 14:55"`
- `git push -u origin main`
- `git log`

## Bonus - 同時追蹤 csv, h5

- `git lfs track "*.csv,*.h5"`
- `git lfs ls-files` 查看已追蹤的檔案
