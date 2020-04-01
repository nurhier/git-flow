# git-flow
### git-flow分支

1. master 分支
也就是我们经常使用的Master分支，这个分支最近发布到生产环境的代码，最近发布的release， 这个分支只能从其他分支合并，不能在这个分支直接修改。每一次提交都需要打一次tag。
2. develop 分支
这个分支是我们是我们的主开发分支，包含所有要发布到下一个release的代码，这个主要合并与其他分支，比如feature分支。最终是保持包含master上的所有代码。
3. feature 分支
这个分支主要是用来开发一个新的功能，一旦开发完成，合并到develop分支
4. release分支
当你需要一个发布一个新Release的时候，我们基于Develop分支创建一个release分支，完成release后，我们合并到master和develop分支，这个分支也可以修复bug。
5. hotfix分支
当我们在master发现新的bug时候，我们需要创建一个hotfix, 完成hotfix后，我们合并回master和develop分支，所以hotfix的改动会进入下一个release。
