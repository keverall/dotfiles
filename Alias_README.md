# Aliases for Chezmoi and Other Shell Commands  

All aliases are defined in `~/.zshrc` for easy access and management of your dotfiles and other shell commands.  

## Chezmoi Aliases  

The following chezmoi aliases have been added to `~/.zshrc` for convenient dotfile management:


- chezmoi git add . && chezmoi git commit -- -m "Update dotfiles"

### Basic Commands:  

- `cz` - `chezmoi` (main command)
- `cza` - `chezmoi add` (add files to chezmoi)
- `czap` - `chezmoi apply` (apply changes)
- `czs` - `chezmoi status` (check status)
- `czd` - `chezmoi diff` (show differences)
- `cze` - `chezmoi edit` (edit files)
- `czu` - `chezmoi update` (update from source)
- `czr` - `chezmoi re-add` (re-add files)
- `czm` - `chezmoi merge` (merge changes)

### Navigation:  

- `czcd` - `chezmoi cd` (change to chezmoi directory)

### Git Operations:  

- `czpu` - `chezmoi git push` (push to git)
- `czpl` - `chezmoi git pull` (pull from git)
- `czst` - `chezmoi git status` (git status)
- `czco` - `chezmoi git commit` (git commit)
- `czga` - `chezmoi git add .` (git add all)
- `czgca` - `chezmoi git add . && chezmoi git commit` (add and commit)

### Usage Examples  

```bash
# Check what files have changed
czs

# Add a new dotfile to chezmoi
cza ~/.bashrc

# Apply changes from chezmoi to your system
czap

# Edit a file managed by chezmoi
cze ~/.zshrc

# Show differences between managed and actual files
czd

# Update from remote source and apply changes
czu

# Navigate to chezmoi source directory
czcd

# Git workflow with chezmoi
czga                    # Stage all changes
czco -m "Update config" # Commit changes
czpu                    # Push to remote

# Accept diffs and update repository workflow
czs                     # Check status
czr                     # Re-add all managed files (accepts changes from target files)
czgca -m "Accept configuration changes"  # Add, commit in one command
czpu                    # Push to remote
```

## Other Shell Aliases  

The following additional aliases are available in `~/.zshrc`:

### Navigation:

- `..` - `cd ..` (go up one directory)
- `...` - `cd ../..` (go up two directories)
- `....` - `cd ../../..` (go up three directories)
- `.....` - `cd ../../../..` (go up four directories)
- `-` - `cd -` (go to previous directory)

### Git Commands:  

- `gaa` - `git add --all` (add all files)
- `gcm` - `git commit -m` (commit with message)
- `gcam` - `git commit -a -m` (commit all with message)
- `gco` - `git checkout` (checkout branch/commit)
- `gcb` - `git checkout -b` (create and checkout new branch)
- `gst` - `git status` (show status)
- `glog` - `git log --oneline --decorate --graph` (pretty log)
- `gp` - `git push` (push to remote)
- `gpl` - `git pull` (pull from remote)
- `gf` - `git fetch` (fetch from remote)
- `gr` - `git remote -v` (show remotes)
- `gd` - `git diff` (show differences)
- `gdc` - `git diff --cached` (show staged differences)

### System & Utilities:  

- `history` - `history -E` (show command history with timestamps)
- `gk` - `gitkraken` (open GitKraken)
- `ff` - `fastfetch --logo-type sixel --logo ~/Downloads/Ubuntu-nice.jpg --logo-width 30` (custom fastfetch)

### AWS Commands:

- `awsp` - `aws sts get-caller-identity` (show AWS profile)
- `awsl` - `aws s3 ls` (list S3 buckets)
- `awsec2` - `aws ec2 describe-instances` (list EC2 instances)
- `awslogs` - `aws logs describe-log-groups` (list CloudWatch log groups)

### JSON Processing:

- `jqp` - `jq .` (pretty print JSON)