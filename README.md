ListControlExtensions
=====================

This is use for asp.net mvc to extend RadioButtonList and CheckBoxList

Getting Started
=====================
1.将ListControlExtensions.cs,ListControlUtil.cs 两个文件扔到项目里。
2.引入bootstrap的<a href="https://github.com/fronteed/iCheck">icheck插件</a>。

Methods
=====================
- Html.RadioButtonList(string name, List<SelectListItem> items, string cssClass=null)
- Html.RadioButtonListFor<TModel, TProperty>(Expression<Func<TModel, TProperty>> expression, List<SelectListItem> items, string cssClass=null)
- Html.CheckBoxList(string name, List<SelectListItem> items,  string cssClass = null)
- Html.CheckBoxListFor<TModel, TProperty>(Expression<Func<TModel, TProperty>> expression, List<SelectListItem> items,  string cssClass = null)
i.e.
====================

