# 来源 http://www.imooc.com/article/18024?block_id=tuijian_wz
# 在理解的基础上有所改动
# 前提
在一切开始之前，你需要打开Git Bash（Git命令行工具），并使用cd命令进入要上传的新项目的根目录下。  

# 第一步  
添加 README.md 文件和 .gitignore文件。执行以下命令自动生成对应的空文件，可根据情况编写自己的 README.md 文件。.gitignore 的作用是告诉Git哪些文件不需要添加到版本管理中。 

touch README.md;  
touch .gitignore;  


# 第二步   
建立Git仓库。在当前项目目录中生成一个本地的Git仓库。会生成一个名字为.git的隐藏目录。

git init  


# 第三步   
添加当前目录中的所有文件到索引中  

git add .


# 第四步  
将上一步中添加的文件提交到本地仓库中，并附带一个 -m 参数后面加上提交的一段注释，用于说明本次提交的代码都做了什么  

git commit -m "项目名称"


# 第五步 ----这一步很关键   
在GitHub上新建一个Repository（远程仓库），假如新建的仓库地址为 https://github.com/stevewei95/example.git    执行以下命令将开始我们建立的本地的仓库关联到这个Github远程仓库上。别名为origin，默认位master分支。  

git remote add origin https://github.com/stevewei95/example.git


# 第六步 
上传到Github仓库之前，我们养成先pull一下的习惯，保证我们拿到的是远程仓库的最新代码，执行以下命令:

git pull origin master


# 第七步  
最后我们把本地仓库中的代码上传到GitHub远程目标仓库中     

git push origin master  
