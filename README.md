# progressBtn1
仿网易云音乐带进度条的播放按钮 
# ProgressBtn
# 1：效果图
![image](http://images2017.cnblogs.com/blog/969154/201711/969154-20171109191751356-2046434221.gif)
# 2.属性
    /*** view 环形的底色*/
    private int bgColor; 
    /**** view 进度颜色 */
    private int progressColor;
    /*** view 的宽高，(宽高应当相等)*/
    private float viewHeight, viewWidth;
    /*** view 圆环的宽度*/
    private float viewRoundWidth;

    /***View的中心 暂停，播放图标颜色*/

     private int centerColor;

    /*** view 的进度值，初始为0*/
    private int progressValue=0;
    /*** view 的进度最大值,默认为100 */
    private int progressMax=100;

    /**** 画笔*/
    private Paint paint;

    /**** 标识播放状态： 1是暂停  ; 2是播放*/
    private  int pauseOrPlay=1;
    
# 3：自定义属性
    <attr name="bgColor" format="color"/>
    <attr name="progressColor" format="color"/>
    <attr name="viewWidth" format="dimension"/>
    <attr name="viewHeight" format="dimension"/>
    <attr name="viewRoundWidth" format="dimension"/>
    
# 4：使用
    
    <com.guogali.progressbuttonlibrary.ProgressButton
        android:id="@+id/image"
        android:layout_marginLeft="10dp"
        android:layout_marginTop="10dp"
        android:layout_width="100dp"
        android:layout_height="100dp"
        app:bgColor="@color/colorAccent"
        app:progressColor="@color/colorPrimary"
        app:centerColor="@color/colorAccent"
        app:viewRoundWidth="4dp"/>
        
        
        
  ---------------------------------------------------------
  
# How  To
  
To get a Git project into your build:


# Gralde:

Step 1. Add the JitPack repository to your build file

Add it in your root build.gradle at the end of repositories:

allprojects {
		
		repositories {
			...
		
		maven { url 'https://jitpack.io' }
		
		}
	}
	
	
Step 2. Add the dependency


 dependencies {
	         
		 compile 'com.github.galibujianbusana:ProgressBtn:master-SNAPSHOT'
	 
	 }
	
	

# Maven:
	
	Step 1. Add the JitPack repository to your build file
	
	
	<repositories>
		<repository>
		    <id>jitpack.io</id>
		    <url>https://jitpack.io</url>
		</repository>
	</repositories>
	
	
	Step 2. Add the dependency
	
	<dependency>
	    <groupId>com.github.galibujianbusana</groupId>
	    <artifactId>ProgressBtn</artifactId>
	    <version>master-SNAPSHOT</version>
	</dependency>
	
 
    
    
