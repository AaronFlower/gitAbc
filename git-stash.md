##Git Stash
## Git Stash 
用途，将工作区的内容暂存起来。
常用命令：
1. git stash save 'work on add stash function' # 保存 working diretory 的内容，使其变成一个 clean working directory.
2. git stash list # 查看 stash 的内容
3. git stash apply stash@{0}# 恢复 working directory, 但是并不会从 stash list 中删掉。
4. git stash pop # 恢复 working diretory, 并且从 stash list 中删除。
5. git stash drop stash@{0} # 直接指定删除 stash list 中的内容。
6. git stash clear # 即 git stash drop all, 删除所有 stash 的内容。

**提示：** git stash 可以在 branch 之间进行传递，所以在错误分支上修改可以使用 git stash, 然后通过切换到新的 branch 上进行提交。

gsta='git stash'          -- stash 文档
gstaa='git stash apply'   -- 恢复stash的文件 但是stash不会被删除，自己执行stash drop
gstd='git stash drop'     -- stash drop stash@{0}
gstl='git stash list'     
gstp='git stash pop'      -- 等价于 git stash apply | git stash drop
gsts='git stash show --text' -- 可以查看 git stash 的内容与 working directory 的diff'

