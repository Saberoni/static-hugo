# static-hugo

## Development

Run the local development container in vscode as this will contain all the tools required.

To run the development server run `hugo server -D`

## FAQ

Q. I can't push changes to git due to an ssh agent error.
A. The dev container mounts the ssh keys from wsl, so you probably just need to make sure windows is running the ssh agent. 
Run the following in Powershell as Administrator.

```Powershell
Get-Service ssh-agent | Set-Service -StartupType Automatic
Start-Service ssh-agent
```
