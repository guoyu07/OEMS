# OEMS
Online Examination System

帮学校做的一个在线答题系统，包含不定项选择题（多选、少选均不得分）和判断题，分成了两个版本。

V1：考生边答题边计算和更新分数，将数据写入到数据库。

V2：后台管理员统计计算分数，并写入考生数据表中。

当考生人数比较多的时候，考生答题时更新分数就会不断向user表中写入数据，容易照成卡顿，且计算分数的操作比较复杂。
后期进行了优化，考试结束之后，由管理员通过对数据库的查询计算得到每个考生的分数，并依此写到数据库中。

该系统由BootStrap+PHP+Mysql编写而成，除了前端借助了框架之外，其他的都是自写的，算是自己做的第一个大项目，收获颇丰。
