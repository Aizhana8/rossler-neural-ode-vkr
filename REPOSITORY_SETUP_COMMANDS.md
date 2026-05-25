# Команды для публикации репозитория на GitHub

```bash
cd rossler-neural-ode-vkr

git init
git add .
git commit -m "Initial commit: Rossler Neural ODE experiments"

git branch -M main
git remote add origin https://github.com/<username>/rossler-neural-ode-vkr.git
git push -u origin main
```

Если в будущем появятся большие файлы моделей или датасетов, можно подключить Git LFS:

```bash
git lfs install
git lfs track "*.pt"
git add .gitattributes
git add checkpoints/*.pt
git commit -m "Track model checkpoints with Git LFS"
```
