# Linux

### 环境配置

- vmware 14,破解码网上找

  - 可能需要设置intelvituralxxxx，开机F1F2在bios中的security中打开

  - 下载centos7安装包dvd.iso，教程链接https://www.cnblogs.com/ysocean/p/7689146.html#_label1_4

  - 默认centos是没有自动联网需要配置

    - nmcli d识别机器中安装的以太网卡

    - 打开**/ etc / sysconfig / network-scripts /** 找到对应上面打印网卡的名称进行修改

      ```LINUX
      BOOTPROTO=dhcp
      ONBOOT=yes
      ```

    - ip addr 打印地址后即可用xftp和xshell连接管理文件代码

  - ​

1.mkdir

2.cd/ 

3.mv $HOME/testFolder /var/tmp 移动文件

4.rm -rf 删除目录

5.ls /etc  使用 ls 命令查看 /etc 目录下所有文件和文件夹

6.touch ~/testFile 创建文件

7.cp ~/testFile ~/testNewFile 复制文件

8.grep 'root' /etc/passwd 过滤含有root关键字的内容

9.grep -r 'linux' /var/log/  递归过滤出含有linux关键字的内容

10.