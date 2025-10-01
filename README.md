<!--
 Minimal, terminal-esque GitHub Profile README
 ASCII art generated (figlet -f slant "Asnan")
-->

```
                                      
_____    ______ ____ _____    ____  
\__  \  /  ___//    \\__  \  /    \ 
 / __ \_\___ \|   |  \/ __ \|   |  \
(____  /____  >___|  (____  /___|  /
     \/     \/     \/     \/     \/ 
             @Asnan
```

> minimal | terminal-first | hacking on systems, dev tooling, and indie products

---

### $ whoami
```bash
dev_user=asnan
focus=( systems linux backend full-stack ai tooling devops )
editor="neovim"
shell="bash"
distro="Arch btw"
motto="Ship small. Iterate. Automate."
```

### $ stack --badges
<p>
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=ffdd54" />
  <img src="https://img.shields.io/badge/JavaScript-181717?style=flat-square&logo=javascript&logoColor=F7DF1E" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/MongoDB-001e2b?style=flat-square&logo=mongodb&logoColor=4EA94B" />
  <img src="https://img.shields.io/badge/Linux-000000?style=flat-square&logo=linux&logoColor=FCC624" />
</p>

### $ about
```bash
cat <<'EOF'
I like: low-level curiosity, lean web stacks, CLI ergonomics, reproducible envs,
fast feedback loops, automating boring ops, and exploring AI + systems crossover.
EOF
```

### $ workflow
```bash
tools=( tmux nvim fzf fd ripgrep lazygit gh docker podman kubectl )
principles=( "text-first" "script-not-click" "measure-before-optimize" "delete-fearlessly" )
```

---

### $ current_projects
- kernel-sandbox: Tiny userspace playground to experiment with syscalls & isolation tricks.
- ai-shell-tools: Modular CLI helpers wrapping LLM endpoints with caching + streaming.
- react-minimal-dashboard: Headless components + dark terminal theme for internal tools.
- mongo-event-pipeline: Lightweight CDC -> queue -> worker pattern with metrics & retries.
- dotfiles-bare: Reproducible dev env bootstrap (bash, neovim, tmux, linting, CI hooks).

```bash
for proj in kernel-sandbox ai-shell-tools react-minimal-dashboard mongo-event-pipeline dotfiles-bare; do
  printf "cloning %s ... done\n" "$proj"
done
```

---

### $ stats
<p align="center">
  <img height="150" src="https://github-readme-stats.vercel.app/api?username=Asnan07&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true" />
  <img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Asnan07&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />
</p>
<p align="center">
  <img height="150" src="https://streak-stats.demolab.com?user=Asnan07&theme=tokyonight&hide_border=true" />
</p>

---

### $ net.links
<p>
  <a href="https://www.linkedin.com/in/asnan" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://twitter.com/asnan_dev" target="_blank">
    <img src="https://img.shields.io/badge/Twitter-121212?style=flat-square&logo=twitter&logoColor=1DA1F2" />
  </a>
  <a href="mailto:asnan.dev@proton.me">
    <img src="https://img.shields.io/badge/Email-181717?style=flat-square&logo=gmail&logoColor=D14836" />
  </a>
</p>

---

### $ ~/.bashrc (excerpt)
```bash
# Prompt
PS1='\[\e[38;5;40m\]\u\[\e[0m\]@\[\e[38;5;81m\]\h\[\e[0m\]:\[\e[38;5;214m\]\w\[\e[0m\]\$ '

# Quick nav
alias dotfiles='git --git-dir=$HOME/.cfg/ --work-tree=$HOME'
alias gs='git status -sb'
alias k='kubectl'
alias d='docker'
alias ports='ss -tulpn'
alias lg='lazygit'

# Search helpers
f() { find . -iname "*$1*"; }
grepi() { rg -i "$1"; }

# Virtual env quick create
mkpy() { python -m venv .venv && source .venv/bin/activate && pip install -U pip; }

# JSON pretty
alias jpp='python -m json.tool'

# Fast note
note() { printf "# %s\n\n" "$(date -Iseconds)" >> ~/NOTES.md && ${EDITOR:-nvim} ~/NOTES.md; }
```

---

### $ fun.echo
```bash
function coffee() {
  echo "[*] compiling caffeine..."
  sleep 0.7
  echo "[+] done. latency reduced."
}

matrix() {
  tr -dc '01' </dev/urandom | head -c 4096 | fold -w64
}

fortune_like() {
  msgs=(
    "Ship > Perfect."
    "Cache invalidation & naming—still hard."
    "Automate the repetitive, craft the critical."
    "Small scripts grow into platforms."
  )
  printf "%s\n" "${msgs[$RANDOM % ${#msgs[@]}]}"
}

coffee && fortune_like
```

---

### $ exit
```bash
echo "Session closed. (ctrl+c to reopen?)"
```

<!-- End -->
