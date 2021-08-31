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
	        implementation 'com.github.easyboot:VerticalProgress:0.1.0'
	}
  
  
  在xml中加入
  
        <com.easyboot.mylibrary.VerticalProgress
            android:id="@+id/vpb_Printing"
            android:layout_width="25dp"
            android:layout_height="match_parent"
            android:layout_centerInParent="true"
            app:layout_constraintRight_toRightOf="parent"
            app:my_background_show="true"
            app:my_gradient_enable="true"
            app:my_progress="55.5"
            app:my_background="@color/color_4EA6FD"
            app:my_progress_background="@color/light_gray"
            app:my_progress_start_color="@color/white"
            app:my_progress_end_color="@color/white"
            app:my_progress_txt_color="@color/gray">
        </com.easyboot.mylibrary.VerticalProgress>
        
  
下面是可用的属性

  <declare-styleable name="verticalProgress"> 

           <attr name="my_background_show" format="boolean" />
        <attr name="progress_border_width" format="dimension" />
        <attr name="my_gradient_enable" format="boolean" />
        <attr name="my_progress"  format="integer"/>
        <attr name="my_radius" format="dimension" />
        <attr name="my_background" format="color" />
        <attr name="my_progress_background" format="color" />
        <attr name="my_progress_start_color" format="color" />
        <attr name="my_progress_end_color" format="color" />
        <attr name="my_progress_txt_color" format="color" />
    </declare-styleable>
    
    
    java 中使用
     private com.easyboot.mylibrary.VerticalProgress verticalProgress;
     
       verticalProgress = findViewById(R.id.vpb_Printing);
       
        verticalProgress.setProgress(progress++);
       
