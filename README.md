ListControlExtensions
=====================

This is use for asp.net mvc to extend RadioButtonList and CheckBoxList

Getting Started
=====================
1.将ListControlExtensions.cs,ListControlUtil.cs 两个文件扔到项目里。<br/>
2.引入bootstrap的<a href="https://github.com/fronteed/iCheck">icheck插件</a>。

Methods
=====================
- Html.RadioButtonList(string name, List<SelectListItem> items, string cssClass=null)
- Html.RadioButtonListFor<TModel, TProperty>(Expression<Func<TModel, TProperty>> expression, List<SelectListItem> items, string cssClass=null)
- Html.CheckBoxList(string name, List<SelectListItem> items,  string cssClass = null)
- Html.CheckBoxListFor<TModel, TProperty>(Expression<Func<TModel, TProperty>> expression, List<SelectListItem> items,  string cssClass = null)
i.e.
====================
 @Html.RadioButtonListFor(model => model.Marriage, (Models.MarriagesEnum.已婚).ToSelectListItem((int)Models.MarriagesEnum.已婚), cssClass: "nav radio")

   &lt;script&gt;
   
        $('input:radio').each(function () {
            var self = $(this);
            self.iCheck({
                radioClass: 'iradio_flat-blue',
            });
        });
        $('input:checkbox').iCheck({
            checkboxClass: 'icheckbox_flat-blue',
        });

    &lt;/script&gt;

