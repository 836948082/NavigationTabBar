# NavigationTabBar
# 多彩标签栏

https://github.com/DevLight-Mobile-Agency/NavigationTabBar

<devlight.io.library.ntb.NavigationTabBar
   android:id="@+id/ntb"
   android:layout_width="match_parent"
   android:layout_height="50dp"
   app:ntb_animation_duration="400"
   app:ntb_preview_colors="@array/colors"
   app:ntb_corners_radius="10dp"
   app:ntb_active_color="#fff"
   app:ntb_inactive_color="#000"
   app:ntb_badged="true"
   app:ntb_titled="true"
   app:ntb_scaled="true"
   app:ntb_tinted="true"
   app:ntb_title_mode="all"
   app:ntb_badge_position="right"
   app:ntb_badge_gravity="top"
   app:ntb_badge_bg_color="#ffff0000"
   app:ntb_badge_title_color="#ffffffff"
   app:ntb_typeface="fonts/custom_typeface.ttf"
   app:ntb_badge_use_typeface="true"
   app:ntb_swiped="true"
   app:ntb_bg_color="#000"
   app:ntb_icon_size_fraction="0.5"
   app:ntb_badge_size="10sp"
   app:ntb_title_size="10sp"/>

<devlight.io.library.ntb.NavigationTabBar 各属性详解
    全局:
    app:ntb_bg_color="#000"             ntb的背景颜色                可自定义
    app:ntb_active_color="#000"         ntb活动时的图标+标题颜色      可自定义
    app:ntb_inactive_color="#0f0"       ntb不活动时的图标+标题颜色    可自定义
    app:ntb_corners_radius="10dp"       ntb切换时的动画弧度大小       可自定义
    app:ntb_animation_duration="1000"   ntb切换时的动画时间           单位:ms
    图标相关:
    app:ntb_icon_size_fraction="1"      图标所占的大小比例            最佳值:0.5
    标题相关:
    app:ntb_titled="true"               是否显示图标所对应的标题       默认为false
    app:ntb_title_mode="active"         图片所对应的标题显示模式       active:活动时才显示 all:总是显示  PS:app:ntb_titled属性值为 true 时才可用
    app:ntb_title_size="10sp"           设置图标所对应的标题文字大小    请自定义
    勋章相关:
    app:ntb_badged="false"              是否显示勋章                  默认为false
    app:ntb_badge_gravity="top"         勋章的上下位置                top|bottom
    app:ntb_badge_position="right"      勋章的左右位置                left(25%), center(50%) and right(75%)
    app:ntb_badge_bg_color="#ffff0000"  勋章的背景颜色                可自定义
    app:ntb_badge_title_color="#000000" 勋章的标题文字颜色             可自定义 PS:不设置的话默认为切换动画的背景色
    app:ntb_badge_size="12sp"           勋章的标题文字大小             可自定义
    字体相关:
    app:ntb_badge_use_typeface="false"  是否使用自定义字体             默认为false
    app:ntb_typeface="fonts/by3500.ttf" 设置ntb的自定义字体            请将自定义的字体文件放在 asset/fonts 文件夹下
    其他:
    app:ntb_preview_colors="@array/colors"
    app:ntb_scaled="true"
    app:ntb_tinted="true"
    app:ntb_swiped="true"/>


    app:layout_scrollFlags="scroll|enterAlways|snap"//随着滑动显示、隐藏，(拉出超过75%自动展开)
    app:layout_scrollFlags="scroll|enterAlways"//随着滑动显示、隐藏，拉出一半就地停留
    app:layout_scrollFlags="scroll|exitUntilCollapsed|snap"//(只有滑动到顶部时)随着滑动显示、隐藏，(拉出超过75%自动展开)