
VS Code PowerShell as Administrator
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted



Delete existing dependencies and lock file:

Remove-Item -Recurse -Force .\node\

Remove-Item -Recurse -Force .\.frontend-maven-plugin\

Remove-Item -Recurse -Force node_modules

Remove-Item package-lock.json




Clear npm cache:
npm cache clean --force





Reinstall dependencies:
npm install --verbose


Run the app:
npm run dev



