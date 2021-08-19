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
            android:layout_width="20dp"
            android:layout_height="match_parent"
            android:layout_centerInParent="true"
            app:layout_constraintRight_toLeftOf="@id/print_progress"
            app:mprogress="55"
            app:progress_border_enable="true"
            app:progress_end_color="@color/blue_end"
            app:progress_solid_color="@color/white"
            app:progress_gradient_enable="false"
            app:progress_border_width="@dimen/dp_5">

        </com.easyboot.mylibrary.VerticalProgress>
        
  
