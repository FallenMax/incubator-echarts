# Echarts

基于官方Echarts的一些patch

分支说明：

- master
  - 拉取官方master分支更新，不做任何改动
- patch-x
  - 基于master分支的本地修复
  - 可选地，提PR给上游
  - 要求
    - 评估patch的必要性，尽可能不patch，等待官方修复或从外部绕过
    - 每个patch分支只改动一个问题，改动尽可能小，减少未来的合并冲突，尽可能合入上游
- private-release
  - 基于最新echarts发版commit的内部发版分支，用于在公司内部npm registry上发包, 打对应版本的git tag
  - cherry-pick patch改动，echarts发新版后rebase
