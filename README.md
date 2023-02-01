# myTest2.1
2023.2.1进行git协同开发测试
测试场景如下：

1.由陈静基于测试项目创建本地仓库；创建远程仓库，推送项目到远程仓库。
创建cj.html
内容
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <div>第一次 陈静创建初始项目并推送到github</div>
</body>
</html>


2.李珊，王君月从远程仓库克隆项目到自己电脑的vsCode中。
内容与上面一致。


3.李珊修改工作区，提交到本地仓库，再推送到远程仓库。
修改操作：李珊增加一个ls.html
内容为：
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <div>第二次 李珊修改项目新增文件并推送到github</div>
</body>
</html>

4.陈静，王君月直接从远程仓库获取最新的代码。




5.王君月对工作区进行修改，提交到本地仓库，再推送到远程仓库。
修改操作：王君月增加一个wjy.html
内容为：
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <div>第三次 王君月修改项目新增文件并推送到github</div>
</body>
</html>

6.陈静，李珊直接从远程仓库获取最新的代码。
7.陈静对工作区进行修改，提交到本地仓库，再推送到远程仓库。
修改操作：陈静增加一个test.html
内容为：
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <div>第四次 陈静创建测试文件并推送到github</div>
</body>
</html>
8.王君月，李珊直接从远程仓库获取最新的代码。
9.李珊和王君月修改test.html文件的同一行，提交到本地没有问题，但是推送到远程仓库时，后一个推送操作就会失败。
李珊先修改div行改为
 <div>第五次 李珊修改测试文件并推送到github</div>
推送成功后
王君月修改test行改为
 <div>第六次 王君月创建测试文件并推送到github</div>
发生冲突
解决方法：1.需要先获取远程仓库的代码到本地仓库，编辑冲突，提交并推送代码。
  2.在github上会在提交时给出处理提示，在github上进行修改编辑冲突。
10.三人分别创建一个远程仓库的分支，创建文件推送到远程仓库分支上之后进行合并到主分支操作。
