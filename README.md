# github 配置
* 生成sshkey,最后得到了两个文件：id_rsa和id_rsa.pub
    
    ssh-keygen -t rsa -C "nicoleefang@gmail.com"

* 进入github的setting -> SSH keys,填入 id_rsa.pub

# sublime配置及插件
*   sublime下载地址：[sublime text 3](https://www.sublimetext.com/3)
*   安装 [package Control](https://packagecontrol.io/installation#st3) 
    
        import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)

*   打开sublime text3, Ctrl + `粘贴进去回车，安装好后重启sublime text
*   Ctrl + Shift + p,输入 install Package命令 回车，sublime text会在线加载插件，选择需要安装的插件即可