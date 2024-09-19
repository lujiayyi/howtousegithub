# howtousegithub
directions for using github
* 下载github 注册账号并登录
* 创建仓库
* 下载git
* 打开git
  输入
  ```
  ssh-keygen -t rsa -C "你的git邮箱账号"
   ```
  以获取ssh密匙
* 在文件资源管理器中找到id_rsa.pub，并复制全部文字
* 返回github，在setting中找到ssh，点击new ssh key，粘贴刚才复制的文字，点击add ssh key
* 返回git
  输入
  ```
  ssh -T git@github.com
  ```
来检查是否成功绑定。如果输入之后选择yes出来是这样说明就成功了。
* 输入
* ```git config --global user.name "你的git账号"
     git config --global user.email "你的git邮箱"
  ```
* 在GitHub中找到你创建的仓库的url
* 在文件资源管理器中找一个你想存放该仓库的地方，然后右键更多选项，以git bash here打开
* 输入
  ```
  git clone 你复制的仓库url
  ```
* 此时你能看到仓库的文件已经创建好了
* 在这个文件中任意新建一个你想要的文件
* 右键运行git bash
  输入
  ```
  git add 你刚才新增的文件
  ```
  例如
  ```
  git add test.txt
  ```
* 输入
  ```
  git commit -m "justtest"
  ```
  引号中的内容作为备注可以随意改动
* 输入
  ```
  git push origin main
  ```
  然后你会发现刚才创建的文件已经成功上传到github了
  
