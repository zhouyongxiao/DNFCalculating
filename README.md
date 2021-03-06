# DNFCalculating

执行程序下载:https://wws.lanzous.com/b01bfj76f 或 https://pan.lanzou.com/b01bfj76f

python（3.8）编写，使用 pyqt5（5.14.2） 图形 GUI 库<br>
主框架由纸飞机实现，西瓜提供数据公式并协助修改，SCUDRT 对算法进行优化修改，风之凌殇添加多进程优化<br>

## 程序目录结构说明

### Part 目录

职业相关文件目录,由职业名.py 及 sum.py 组成,职业名.py 负责各个职业的个性化数据,sum.py 负责引用所有职业<br>
若项目文件打开时图片显示不正常请将 pyqt5 版本更新至 5.14.2 或以上<br>

### ResourceFiles 目录

资源文件目录,由公用资源文件及职业资源文件组成<br>

### main.py

程序入口页面,职业相关部分已经抽出,无需修改<br>

### PublicReference 目录

公共实现部分,由 base.py 装备.py 装备函数.py 组成

#### PublicReference/base.py

核心算法及主体界面绘制部分<br>
常规无需修改该部分,如需要优化程序的效率及部分算法，可尝试修改<br>
主体核心可优化空间比较大,但由于接触 PY 才几个礼拜,对 PY 多核心运算的不熟悉,暂不打算修改,欢迎尝试优化

#### PublicReference/装备.py

装备及套装数据部分<br>
如需要添加修改装备.可在此处修改,注意装备的后缀数字,需要与 img/装备下的文件名一致(新增需要同步添加图标)

#### PublicReference/装备函数.py

一些计算公式部分,除非公式出现偏差,否则无需修改<br>

## 更新说明

### 2020/7/25

1. 第五页增加批量选择改造套装(85SS+改造)选项<br>
2. 优化第五页计算逻辑，第五页显示装备属性<br>
3. 增加装备对比显示，需要在第五页设置/清空基准值<br>

### 2020/7/24

1. 修正 100 传说套装在未佩戴上衣耳环手镯时的装备属性和描述<br>
2. 修正手搓上衣描述<br>
3. 修正混沌魔灵 60 技能 CP 数据<br>
4. 增加第二页选项自动保存<br>
5. 修正部分装备描述，修正 85SS 转甲后的基础属性<br>
6. 修正排行界面等级溢出显示(白金时装未选择溢出技能时按钮不会变红)<br>
7. 统一了各职业名称，改动职业本地存档(set 文件夹)需要手动复制继承<br>
8. 修正完美掌控装备属性和描述<br>

### 2020/7/23

1. 修正次元数据：<br>

- 技能数据全部更换为数组。<br>
- 修正了二觉攻击次数。<br>
- 添加了是否取消次元：思维聚爆持续伤害的选项。<br>
- 添加了护石的 CD 缩减数据。<br>
- 现在是否强化次元：粒子风暴的选项会受到护石选择的影响了。<br>
- 调整了技能顺序，现在按照等级从低到高排列。<br>
- 使用了更极限的技能模板。<br>

2. 修正部分职业技能数据<br>
3. 修正暗之腐蚀套装属性描述<br>
4. 修正剑宗 CD(取消一觉 CD 默认生效)<br>
5. 修正驱魔落雷符 CD<br>
6. 修正元素，魔灵，暗枪人物基础<br>
