# 卸载文件存储

通过在云主机实例上运行umount命令可以卸载已挂载的文件存储，在登录云主机实例后，运行以下命令，如文件存储挂载在efs目录：

`umount efs`

 

卸载完成后，可通过运行以下命令验证是否成功：

`df -h`

