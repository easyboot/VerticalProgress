# VerticalProgress
非常简单的一个垂直进度条
带有数字显示
使用示例

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
  在build.gradle总加入
  
  	dependencies {
	        implementation 'com.github.easyboot:VerticalProgress:0.0.1'
	}
  
  
  在xml中加入
  
         <com.easyboot.mylibrary.VerticalProgress
            android:id="@+id/vpb_Printing"
            android:layout_width="25dp"
            android:layout_height="match_parent"
            android:layout_centerInParent="true"
            app:layout_constraintRight_toRightOf="parent"
            app:progress_border_enable="true"
            app:progress_gradient_enable="true"
            app:myprogress_progress="55"
            app:myprogress_background="@color/color_4EA6FD"
            app:myprogress_progress_background="@color/light_gray"
            app:myprogress_progress_start_color="@color/white"
            app:myprogress_progress_end_color="@color/white">

        </com.easyboot.mylibrary.VerticalProgress>
        
  
下面是可用的属性

  <declare-styleable name="verticalProgress"> 

        <attr name="myprogress_background_show" format="boolean" />
        <attr name="progress_border_width" format="dimension" />
        <attr name="progress_gradient_enable" format="boolean" />
        <attr name="myprogress_progress"  format="integer"/>
        <attr name="myprogress_radius" format="dimension" />
        <attr name="myprogress_background" format="color" />
        <attr name="myprogress_progress_background" format="color" />
        <attr name="myprogress_progress_start_color" format="color" />
        <attr name="myprogress_progress_end_color" format="color" />
    </declare-styleable>
