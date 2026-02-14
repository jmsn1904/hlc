# Helpful Linux Commands

## Git Filter Repo (git filter-repo)

Rewrite git history across all commits.

```bash
git filter-repo --commit-callback '
    if commit.author_name == b"old author name":
        commit.author_name = b"new author name"
        commit.author_email = b"new email"'
```

## Git Worktree (git worktree)

Enables git branches as separate directories.

```bash
# Create directory for bare repo and branch directories
mkdir -p repo_name
cd repo_name
# Clone bare repository, enabling worktree functionality
git clone --bare <remote_url> .bare
# Makes git commands work in this directory
echo "gitdir: ./.bare" > .git
# Add branch as directory
git worktree add <branch_name>
# Create new branch based on existing branch
git worktree add -b <new_branch_name> <branch_dir_name> <existing_branch_name>

# Do work

# Remove worktree (can't delete local branch if being used as worktree)
git worktree remove <worktree_dir_name>
# Delete branch if needed
git branch -D <branch _name>
```

## Process Status (ps)

```bash
# Every process on the system:
ps aux
# Process tree:
ps axjf
ps auxf
```

## Socket Cat (socat)

```bash
# Proxy TCP Port
sudo socat TCP-LISTEN:66,fork,reuseaddr TCP:192.168.1.100:8080
```

### TODO List

(because I keep forgetting what I should be adding to this doc...)

- curl
- du
- ffmpeg
- fzf
- ip
- jq
- ln (because I always forget if source or destination comes first)
- nmap
- nmcli
- ping (just because there's some cool hidden flags imo)
- rclone or rsync ?
- rg
- tar (!!!!)
- tmux (sessions...)
