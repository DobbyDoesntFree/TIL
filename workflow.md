# Clone, Pull

## Clone

1. Go to github and paste url of repo
2. Reun gitbash terminal and set path
3. Use command git clone URL
   - the path must be dosen't set with git init command
4. git init, git remote add(Link hub repo) commands dosen't need
   - As this file is a clone, it has been set already
   - As this file is a clone, it share branch and workflow of origin

## Pull

> Imagine push(post) and pull(grab)

- Command : git pull origin master
- grab file from repo as latest version

  - origin and master is default value, Can be changed if need

# Branch

> Parrallel world

Sounds might be silly but it's rrrrreally good discription.
![img](https://hphk-edu.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fd6378065-5864-4832-8122-0fde3eb4f6ec%2FUntitled.png?table=block&id=c1098d7b-0ae2-4c68-befe-ece29a09f197&spaceId=f7ab64f0-6613-4035-b609-06b6865d9b61&width=1940&userId=&cache=v2)

## Useful commands (except prefix git)

|           Command           |            Explane             |
| :-------------------------: | :----------------------------: |
|         branch "##"         |   Create branch name as "##"   |
|       branch "##" -r        |        Show branch list        |
|       branch -d "##"        |    Remove branch name "##"     |
|         switch "##"         |     Change branch to "##"      |
|         merge "##"          | merge Current branch with "##" |
| log --oneline --all --graph |      Show branch edit log      |

- Caution)
  - If use -D instead of -d, it can remove unmerged branch
  - Merge confilct : Change text with same line to commit same version once.
    - Sol) Add additional commit

---

# Workflow

## Case 1. Work alone

> Simple. handle master branch as canvas
> If need, create new branch

## Case 2. Work with others

> Never use master branch as work canvas

1. Fork base repo someone created
2. Clone the forked repo
3. Set branch on local and work
4. Merge to forked repo and get module of final result
5. Pull try and review to accept as final result
