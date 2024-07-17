# Git Large File Storage

## Prepare a new git repository

- `git init`
- `git add README.md`
- `git commit -m "first commit"`
- `git branch -M main`
- `git remote add origin https://github.com/thomaschang710114/large-file-goodbuy.git`
- `git push -u origin main`

## On local dev environment

- `brew install git-lfs`
- Verity the installation `git lfs install`
  - Should output `Git LFS initialized.`
- Track file `git lfs track "*.csv" "*.h5"`
  - Output `Tracking "*.csv"`
  - .gitattributes shows `*.csv filter=lfs diff=lfs merge=lfs -text`
- `git lfs push --all origin main`

## Push to main

- `git add .`
- `git commit -m "update by 20240708 23:22"`
- `git push -u origin main`
- `git log`

## Misc

- `git lfs track` 查看已追蹤的檔案
  - 或使用手動加入 `git lfs track 開高低收簡化.h5`
- `git lfs ls-files`

## 每日任務

- 更新新的 h5 檔案
- `git add .`
- `git commit -m "update by 20240708 23:22"`
- `git push -u origin main`
