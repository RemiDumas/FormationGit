# Formation-Git_R


## Git au Cefil



## Configurer la connexion avec Github

### Protocole utilisé
git_protocol() renvoit
i Defaulting to 'https' Git protocol
[1] "https"

### Configurer un token
https://stackoverflow.com/questions/68191392/password-authentication-is-temporarily-disabled-as-part-of-a-brownout-please-us/68199261#68199261
Here is a simple solution:
Go to GitHub → Settings → Developer settings → Personal access tokens. Regenerate your token and copy it.
On any of your local repositories, when git push, enter your username, and the password is the generated token
Instead of manually entering your token for every HTTPS Git operation, you can cache your token with a Git client.

In a terminal, enter the following:
# Set Git to use the credential memory cache
git config --global credential.helper cache
To change the default password cache timeout, enter the following:
# Set the cache to timeout after 1 hour (setting is in seconds)
git config --global credential.helper 'cache --timeout=3600'



Aller sur Github: 
> usethis::gh_token_help()
* GitHub host: 'https://github.com'
* Personal access token for 'https://github.com': <unset>
* To create a personal access token, call `create_github_token()`
* To store a token for current and future use, call `gitcreds::gitcreds_set()`
i Read more in the 'Managing Git(Hub) Credentials' article:
  https://usethis.r-lib.org/articles/articles/git-credentials.html
  
  
  
## Documentation

### Git
https://usethis.r-lib.org/articles/articles/git-credentials.html

### RStudio
https://resources.github.com/github-and-rstudio/
https://rfortherestofus.com/2021/02/how-to-use-git-github-with-r/
https://www.marvinschmitt.com/blog/website-tutorial-quarto/#optional-managing-github-directly-through-git

### Utilisation à l'Insee
