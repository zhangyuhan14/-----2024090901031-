解题代码：
<!DOCTYPE html>
<html>
<head>
    <title>社团报名表单</title>
</head>
<body style="width:90%;margin:0 auto;">
    <div>
        <h1 style="text-align:center;">社团报名表单</h1>
        <form action="" method="post">
            <fieldset>
                <legend>个人信息</legend>
                <table style="width:70%;margin:0 auto;">
                    <tr>
                        <th>姓名</th>
                        <th>电话</th>
                        <th>性别</th>
                    </tr>
                    <tr style="text-align:center;">
                        <td>
                            <input type="text" style="width:120px;" placeholder="请输入姓名">
                        </td> 
                        <td>
                            <input type="tel" style="width:120px;" placeholder="请输入电话">
                        </td>
                        <td>
                            <div>
                                <label>
                                    <input type="radio" name="gender"><span>男</span>
                                </label>
                                <label>
                                    <input type="radio" name="gender"><span>女</span>
                                </label>
                            </div>
                        </td>
                    </tr>
                    <tr>
                        <th>班级</th>
                        <th>邮箱</th>
                        <th>出生日期</th>
                    </tr>
                    <tr style="text-align:center;">
                        <td>
                            <input type="text" style="width:120px;" placeholder="请输入班级">
                        </td>
                        <td>
                            <input type="email" style="width:120px;" placeholder="请输入邮箱">
                        </td>
                        <td>
                            <input type="text" style="width:120px;"placeholder="如:2000-01-01">
                        </td>
                    </tr>
                </table>
            </fieldset>
            <fieldset>
                <legend>所在院系</legend>
                <div>
                    <label>
                        学院：<input type="text" placeholder="请输入学院">
                    </label><br>
                    <label>
                        专业：<input type="text" placeholder="请输入专业">
                    </label>
                </div>
            </fieldset>
            <fieldset>
                <legend>年级</legend>
                <div>
                    <label><b>年级：</b></label>
                    <select>
                        <option selected>2025级</option>
                        <option>2024级</option>
                        <option>2023级</option>
                        <option>2022级</option>
                    </select>
                </div>
            </fieldset>
            <fieldset>
                <legend>想加入的社团类型</legend>
                <div>
                    <label>
                        <input type="checkbox">
                        <span>科技类</span>
                    </label>
                    <label>
                        <input type="checkbox">
                        <span>文艺类</span>
                    </label>
                    <label>
                        <input type="checkbox">
                        <span>体育类</span>
                    </label>
                    <label>
                        <input type="checkbox">
                        <span>公益类</span>
                    </label>
                    <label>
                        <input type="checkbox">
                        <span>学术类</span>
                    </label>
                </div>
            </fieldset>
            <fieldset>
                <legend>兴趣爱好</legend>
                <div style="text-align:center;">
                    <textarea placeholder="请输入兴趣爱好，不限个数" style="width:100%;height:50px;resize:none;"></textarea>
                </div>
            </fieldset>
            <fieldset>
                <legend>报名须知</legend>
                <div>
                    <input type="checkbox">
                    <label for="agreement">我已阅读并同意报名须知</label>
                </div>
            </fieldset>
            <div style="text-align:center;">
                <input type="submit" value="提交报名" style="margin:20px;">
            </div>
        </form>
    </div>
</body>
</html>

HTML 表单相关知识点总结与学习心得
一、相关知识点总结
1.如果要使用HTML表单 需要使用 <form>；
2.<input>控制输入类型，使用type控制，主要有以下几个类型：
password：密码输入框，输入内容会被隐藏；radio：单选按钮，如果多个radio的“name”相同，就仅能选一个；checkbox：复选框，可多选；
submit：提交按钮，用value存放按钮中的内容；button：普通按钮。
3.下拉菜单 <select> 与 <option>，<select>为下拉菜单的容器，<option>表示下拉菜单的单个选项，标签体为选项显示的文字；selected则用于标志设置默认的选中项。
4.多行文本域 <textarea>支持输入多行文本，使用”resize:none”即可固定文本域的大小。
5.placeholder中可以输入提示内容，在用户输入信息之后会被覆盖；
6.<legend>需要与<fieldset>一起使用，并且必须作为fieldset的第一个子元素，可以实现对表单的分组。
二、学习中的感悟或心得（遇到的问题及解决方式）
在对于html的学习中，我首先在菜鸟教程等网站里进行了相关学习，充分了解了相关的必备知识，然后根据任务中的要求给各类信息划分区域，初步建立了一个未加修饰的
表单，在完善与装饰表单的过程中，我一度遇见了一些困难：
1.对于附加要求，首先是照片上传，因为我想把照片放在那个个人信息部分，但是因为那里已经有表格，然后照片的位置实在不知道怎么插进去，所以放弃了；
2.然后一开始因为排版的问题纠结过，后面发现用了legend分块之后的排版还是比较好看的，所以就没有调整特别多；
3.然后就是对于那个提交报名的按钮，一开始他是离上面那个部分太近了，之后学完CSS后又回来用margin调整好了;
4.因为对下拉菜单设置默认项这个在教程里没找到，之后求助了AI学习到了这个知识点。