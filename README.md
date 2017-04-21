
# mego 

mego主要针对ssh做了进一步封装，免除咱们登录远程服务器记不住密码的尴尬，免除登录远程服务器从着陆机上穿越的麻烦。

## 使用方法
 - Usage: bash mego [Options] <server name>
 - Params:
   - server name: 远程服务器名，根据您的配置来决定
 - Options:
   - -s: 显示配置信息，不进行登录 
 - Example:
   - bash mego 11
   - bash mego -s 11

## 环境要求
 - 您的本地服务器必须拥有bash 4.x以上版本
 - Mac更新方法：http://www.1207.me/archives/284.html

## 其他注意
 - 在使用前您需要配置您的服务器，很简单，它就在mego主文件下
 - 建议您将该命令放在$HOME/bin下，并将它纳入您的环境变量下
 - 由于该工具是将密码明文卸载代码中，请注意安全


# mescp

mescp主要针对scp做了进一步封装，免除咱们scp到远程服务器记不住密码的尴尬，免除scp到远程服务器从跳板机上穿越的麻烦。

## 使用方法
 - Usage: bash mecp <server name> <local file> <remote file>
 - Param:
   - server name: 远程服务器名，根据您的配置来决定
   - local file: 需要上传的文件路径
   - remote file: 需要上传打远程路径
 - Example:
   - bash mescp 11 /tmp/file1 /tmp/file2

## 环境要求
 - 您的本地服务器必须拥有bash 4.x以上版本

## 其他注意
 - 在使用前您需要配置您的服务器，很简单，它就在opscp主文件下
 - 建议您将该命令放在$HOME/bin下，并将它纳入您的环境变量下
 - 由于该工具是将密码明文写在代码中，请注意安全
