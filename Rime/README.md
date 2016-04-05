## Rime 引擎的小鹤双拼--语句流  


参考 : <http://www.dreamxu.com/install-config-squirrel/>  


### 使用  

放入 Rime 用户资料文件夹下  

Mac : `~/Library/Rime`  


### 当前项目结构  

1. 小鹤双拼-语句流语法及依赖文件 :  

	double_pinyin_flypy_fluency.schema.yaml	 // 小鹤双拼语句流语法文件
	chinese_contain_english.schema.yaml     // 中文输入包含英文语法文件(依赖)
	chinese_contain_english.dict.yaml	// 单词沾满是 tab  

2. 全局自定配置文件中增加输入方案并增加自定义全局配置 :  

	default.custom.yaml

3. 皮肤等外观设置(可选)  

	squirrel.custom.yaml

4. 小鹤双拼-语句流自定义配置文件(可选) :  

	double_pinyin_flypy_fluency.custom.yaml

除了可选,都是必选  


### 打字  

1. `[`,`]` 翻页  
2. 每页候选数 : 5  
3. 默认不使用语句流 : `express_editor` (语句流 : `fluency_editor`)  
4. 每次修改完配置,要使之生效需要:  
   切换到`鼠须管`输入法, 点击右上角的输入法图标,选择重新部署  
   或者直接 `Control+Option+``  
5. 设定应用程序默认输入状态, 见`squirrel.custom.yaml`  

### 小鹤双拼的基本安装配置  

...  

 
