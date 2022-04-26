# My Bash Profile
My local .bash_profile file contents to speed up CLI interaction

```bash
# Git commands
alias glog='git log --oneline --graph'
alias gpull='git pull origin $(git rev-parse --abbrev-ref HEAD)'
alias gpush='git push origin $(git rev-parse --abbrev-ref HEAD)'
alias gf='git fetch --prune'
alias grh='git reset --hard'
alias grs='git reset --soft'
alias gs='git status -sb'
alias gc='git checkout'
alias gcb='git checkout -b'

# Docker commands
alias dkr='docker compose'

# Docker-PHP commands
alias composer='docker compose exec app composer'
alias phpunit='docker compose exec app vendor/bin/phpunit'

# Docker-Laravel commands
alias artisan='docker compose exec app php artisan'
alias migrate='artisan migrate'
alias mf='artisan migrate:fresh'
alias mfs='artisan migrate:fresh --seed'
```
