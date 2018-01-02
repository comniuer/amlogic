# 工作中的的修改流程记录  
## 修改DVBS中Dtvchannellist_dvbs.xml 
```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
	android:layout_width="fill_parent"
	android:layout_height="fill_parent">    
	
	<LinearLayout 
	    android:id="@+id/RelativeLayout01"
	    android:layout_width="644dp"
	    android:layout_height="650dp"
	    android:layout_gravity="left|top"
	    android:background="@drawable/channel_listcontent_bg"
	    android:orientation="vertical"
	    android:padding="0dp" >

	    <LinearLayout
	        android:layout_width="fill_parent"
	        android:layout_height="43dp"
	        android:layout_alignParentTop="true"
	        android:orientation="horizontal" >

	        <ImageView
	            android:id="@+id/arrow_left"
	            android:layout_width="63dp"
	            android:layout_height="63dp"
	            android:layout_alignParentBottom="true"
	            android:layout_marginLeft="20dp"
	            android:layout_weight="1"
	            android:background="@drawable/dtvchannellist_button_arrow_left" />

	        <TextView
	            android:id="@+id/Text_title"
	            android:layout_width="fill_parent"
	            android:layout_height="fill_parent"
	            android:layout_weight="6"
	            android:gravity="center"
	            android:textSize="30sp" >
	        </TextView>

	        <ImageView
	            android:id="@+id/arrow_right"
	            android:layout_width="63dp"
	            android:layout_height="63dp"
	            android:layout_alignParentBottom="true"
	            android:layout_marginRight="20dp"
	            android:layout_weight="1"
	            android:background="@drawable/dtvchannellist_button_arrow_right" />
	    </LinearLayout>

	    <LinearLayout
	        android:id="@+id/LinearLayoutListView"
	        android:layout_width="fill_parent"
	        android:layout_height="fill_parent"
	        android:layout_marginTop="8dp"
	        android:layout_alignParentBottom="true"
	        android:layout_centerInParent="true"
	        android:layout_weight="4.13"
	        android:background="@drawable/epg_content_bg4"
	        android:paddingLeft="10px"
	        android:paddingRight="13px"
	        android:paddingTop="10px"
	        android:paddingBottom="10px">

	        <!--
			    <ListView 
			      android:id="@+id/ListView_channel"
			      android:layout_width="fill_parent"
			      android:layout_height="fill_parent"		      
			    ></ListView>
	        -->
	        
	        <RelativeLayout 
				android:layout_width="match_parent"
				android:layout_height="match_parent">
				<com.amlogic.widget.FocusScrollListView
			            android:id="@+id/ListView_channel"
			            android:layout_width="match_parent"
			            android:layout_height="match_parent"
			            android:layout_margin="0dip"
			            android:listSelector="#00000000"
			            android:padding="0dip" 
			            android:layout_marginBottom="0dp">
			        </com.amlogic.widget.FocusScrollListView>
			        <ProgressBar  
			        	android:id="@+id/ProgressBar_channel"
					android:layout_width="40dp"  
					android:layout_height="40dp"  
					android:layout_centerInParent="true"  
					style="?android:attr/progressBarStyleSmall"  
				  />
		</RelativeLayout>
	    </LinearLayout>

	    <LinearLayout
	        android:layout_width="fill_parent"
	        android:layout_height="wrap_content"
	        android:orientation="vertical" >

	        <LinearLayout
	            android:layout_width="fill_parent"
	            android:layout_height="50dp"
	            android:layout_marginTop="10dp"
	            android:layout_alignParentTop="true"
	            android:background="@drawable/epg_content_bg2"
	            android:orientation="horizontal" >

	            <TextView
	                android:id="@+id/channel_info"
	                android:layout_width="fill_parent"
	                android:layout_height="fill_parent"
	                android:layout_weight="6"
	                android:gravity="center"
	                android:textSize="24sp"
	                android:singleLine="true">
	            </TextView>
	        </LinearLayout>

	        <LinearLayout
	            android:layout_width="match_parent"
	            android:layout_height="60dp"
	            android:layout_marginTop="10dp"
	            android:gravity="center"
	            android:orientation="horizontal" >

	            <ImageView
	                android:id="@+id/return_icon"	
	                android:layout_width="45dp"
	                android:layout_height="45dp"
	                android:background="@drawable/return_icon" >
	            </ImageView>

	            <TextView
	                android:layout_width="wrap_content"
	                android:layout_height="wrap_content"
	                android:layout_gravity="center"
					android:layout_marginRight="20dp"
	                android:text="@string/help_info_return"
	                android:textColor="#FFFFFFFF"
	                android:textSize="20sp" />
	            
	            <!--    
	            <ImageView
	                android:layout_width="45dp"
	                android:layout_height="45dp"
	                android:background="@drawable/goto_icon" >
	            </ImageView>

	            <TextView
	                android:layout_width="wrap_content"
	                android:layout_height="wrap_content"
	                android:layout_gravity="center"
	                android:layout_marginRight="20dp"
	                android:text="@string/goto_s"
	                android:textColor="#FFFFFFFF"
	                android:textSize="20sp" />
	            -->

	            <ImageView
	                android:layout_width="wrap_content"
	                android:layout_height="wrap_content"
	                android:background="@drawable/red_button" >
	            </ImageView>

	            <TextView
	                android:layout_width="wrap_content"
	                android:layout_height="wrap_content"
	                android:layout_gravity="center"
	                android:layout_marginRight="20dp"
	                android:text="@string/epg_book"
	                android:textColor="#FFFFFFFF"
	                android:textSize="20sp" />

	             <ImageView
	                android:layout_width="wrap_content"
	                android:layout_height="wrap_content"
	                android:background="@drawable/yellow_button" >
	            </ImageView>

	            <TextView
	                android:layout_width="wrap_content"
	                android:layout_height="wrap_content"
	                android:layout_gravity="center"
	                android:layout_marginRight="20dp"
	                android:text="@string/find"
	                android:textColor="#FFFFFFFF"
	                android:textSize="20sp" />  
	                
	            <ImageView
	                android:layout_width="wrap_content"
	                android:layout_height="wrap_content"
	                android:background="@drawable/blue_button" >
	            </ImageView>

	            <TextView
	                android:layout_width="wrap_content"
	                android:layout_height="wrap_content"
	                android:layout_gravity="center"
	                android:layout_marginRight="20dp"
	                android:text="@string/sort"
	                android:textColor="#FFFFFFFF"
	                android:textSize="20sp" />  
	                
	            <ImageView
	            	  android:id="@+id/filter_img"
	                android:layout_width="wrap_content"
	                android:layout_height="wrap_content"
	                android:background="@drawable/green_button" >
	            </ImageView>

	            <TextView
	            	  android:id="@+id/filter_text"
	                android:layout_width="wrap_content"
	                android:layout_height="wrap_content"
	                android:layout_gravity="center"
	                android:layout_marginRight="20dp"
	                android:text="@string/filter"
	                android:textColor="#FFFFFFFF"
	                android:textSize="20sp" />  
	        </LinearLayout>
	    </LinearLayout>
	</LinearLayout>
</LinearLayout>
```
## 修改single_choice_dialog.xml 
```
<?xml version="1.0" encoding="utf-8"?>

<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content" 
	android:gravity="center"
    android:orientation="vertical"
    android:layout_gravity="center_horizontal"
    android:id="@+id/layout_parent"
    > 
	<LinearLayout
		android:layout_width="wrap_content"
		android:layout_height="100dp"
		android:layout_alignTop="@+id/layout_parent"
    >
   </LinearLayout>
   <LinearLayout
   		android:id="@+id/layout_head"
		android:layout_width="wrap_content"
		android:layout_height="80dp"
		android:padding="14dp"
		android:gravity="center"
		android:background="@drawable/single_dia_head"
		>
		
		<TextView
			android:id="@+id/title"
			android:layout_width="wrap_content"
			android:layout_height="34dp"
			android:layout_gravity="center_horizontal"
			android:text="@string/enter_password"
			android:textColor="#FFFFFFFF"
			android:gravity="center"
			android:textSize="24sp" 
			android:layout_marginTop="20dp"
			android:layout_marginBottom="10dp" />	
	</LinearLayout> 

	

		<LinearLayout
			android:id="@+id/layout_body"
    		android:layout_width="match_parent"
    		android:layout_height="wrap_content"
    		android:paddingLeft="50dp"
    		android:paddingRight="50dp"
    		android:background="@drawable/single_dia_body"
    		android:layout_above="@+id/layout_tail" 
    		android:layout_below="@+id/layout_head" >

    		<LinearLayout
    			android:layout_width="match_parent"
    			android:layout_height="match_parent">
			<!--
			<ListView 
				android:id="@+id/list_item"
				android:layout_width="fill_parent"
				android:layout_height="wrap_content"
				android:cacheColorHint="#00000000"
				android:divider="#0000"
				android:dividerHeight="0px"
				android:focusable="true"
				android:layout_marginLeft="30px"
				android:layout_marginRight="30px" 			
			></ListView>   
			-->
			
			<com.amlogic.widget.FocusScrollListView 
				android:id="@+id/list_item"
				android:layout_width="match_parent"
				android:layout_height="wrap_content"
				android:listSelector="#00000000">
			</com.amlogic.widget.FocusScrollListView>
		</LinearLayout> 
	</LinearLayout> 
	
	<LinearLayout
		android:id="@+id/layout_tail" 
		android:layout_width="fill_parent"
		android:layout_height="90dp"
		android:background="@drawable/single_dia_tail"
		
		>
		
	    <LinearLayout
			android:layout_width="wrap_content"
			android:layout_height="wrap_content"
			android:orientation="horizontal"
			android:paddingLeft="120dp"
    			android:paddingRight="60dp"
    			android:paddingTop="45dp"
			android:gravity="center">
			
			<Button android:id="@+id/no"
			   android:layout_width="wrap_content"
	         	   android:layout_height="30dp"
	       	   android:background="@drawable/single_dia_button"
	       	   android:layout_weight="1"
	           />
	           <ImageView 
			   android:layout_width="30dp"
		          android:layout_height="30dp"
			   android:background="@drawable/move_icon_single" 
			   
			   android:layout_weight="1">
			  </ImageView>
	           
			<Button android:id="@+id/yes"
			   android:layout_width="wrap_content"
	          	   android:layout_height="30dp"
	       	   android:background="@drawable/single_dia_button"
	       	   android:layout_weight="1"
	           />
		</LinearLayout>
	</LinearLayout>	
	<LinearLayout
		android:layout_width="match_parent"
		android:layout_height="100dp"
		android:layout_alignBottom="@+id/layout_parent"
    >
    </LinearLayout>
</LinearLayout>
```
