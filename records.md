# nvm nodejs 升级
#### - 查看nvm,node,npm 版本  
  mvm --version  
  node -v   
  npm -v   

#### - 查看node npm 对应版本 ![]('https://nodejs.org/zh-cn/download/releases/')

#### - 安装nrm(npm registry manager 也就是npm的镜像源管理工具)  
  npm install -g nrm
  1. 命令：nrm ls 用于展示所有可切换的镜像地址
  2. 命令：nrm use cnpm 我们这样就可以直接切换到cnpm上了。当然也可以按照上面罗列的其他内容进行切换
  3. 命令：nrm test npm 测试当前镜像速度


项目下新建 .npmrc 文件，加入如下配置：

electron_mirror=https://npm.taobao.org/mirrors/electron/
即使用淘宝的源，重新 npm install

npm install --save-dev electron
如果速度还是很慢就把  package-lock.json 和 node-modules 删掉，重新 install


seanlocal branch
