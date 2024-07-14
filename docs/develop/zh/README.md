开发 teedoc
===========


## 获得源码

```
git clone https://github.com/Neutree/teedoc
```

## 安装环境

```
sudo apt install python3 python3-pip
cd teedoc
pip3 install -r requirements.txt
```



## 运行源码

* 安装插件

```
python3 teedoc/teedoc_main.py  -p examples/teedoc_site install
```

* 运行

```
python3 teedoc/teedoc_main.py  -p examples/teedoc_site build
python3 teedoc/teedoc_main.py  -p examples/teedoc_site serve
```

* 插件导入问题和更新调试问题

在`site_config.json`中设置插件的本地路径，比如：
```json
"teedoc-plugin-markdown-parser":{
            "from": "../../plugins/teedoc-plugin-markdown-parser"
        }
```
然后在运行时将会优先从这个路径导入包（将这个路径加入`sys.path`，然后导入），而不是系统路径，可以保证修改及时生效




## 调试

在 vscode 中调试，直接调试单文件 `teedoc_debug.py` 文件即可


## 参与贡献

可以在 `github` `fork` 一份源码， 修改代码后， 提交`PR`(`pull request`) 即可






