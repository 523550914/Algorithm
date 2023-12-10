# 📝 Algorithm
算法题练习记录博客（基于GitHub Action和GitHub Issue实现）。可通过提交issue，自动将刷题记录更新在项目的DailyLC.md中，并将issue内容备份在项目backup文件夹下。

## 🎯 Usage
1. fork这个项目（注意激活fork后的项目的Actions, 并将项目的Settings -> issue打开）
2. 每当你刷完一道算法题，可在你的项目上提交一个issue(！！issue title需要以‘R'开头，作为和真正issue的区分标识)，推荐将'R+所刷题目的标题'（比如R110.平衡二叉树）作为issue title，将题目的归属标签（比如二叉树、搜索）作为issue Labels，将你想记录的对这道题的思考作为issue的description。此时[DailyLC.md](./DailyLC.md)

    1） Calendar部分会基于issue创建日期在日历上标记一个star

    2） Records部分会新增一行记录, 各列分别记录：

         #: issue号
         Title: 截去R的issue title（点击可跳转至你所创建的issue）
         Tag： issue Labels
         Date: issue创建时间
    
3. 同时，backup文件夹下会以“issue号+#+截去R的issue title"作为文件名，生成一个对issue的备份文件，备份issue的description和comments
4. 当你编辑issue的title或description、修改issue的Labels、issue有新comment或者issue的comment被编辑时, [DailyLC.md](./DailyLC.md)和backup文件夹下issue的备份文件都会进行相应更新(FIXME: 当issue title被改变时，会生成一个新的备份文件，但原来的备份文件并不会被删除)

