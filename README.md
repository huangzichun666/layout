# layout
实验二

线性布局实验截图：


![](https://raw.githubusercontent.com/huangzichun666/layout/master/image/XM37P%7DZ3[ED%%7B49$%7BSOC[YW.png)


约束布局实验截图：


![](https://raw.githubusercontent.com/huangzichun666/layout/master/image/sdf.png)


表格布局实验截图：


![](https://raw.githubusercontent.com/huangzichun666/layout/master/image/KG_@HN2QI[LB7EJJRETY%7BO7.png)



线性布局代码xml文件：

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    tools:context=".MainActivity">

   <LinearLayout
       android:layout_width="match_parent"
       android:layout_height="wrap_content"
       android:orientation="horizontal">
       <Button
           android:layout_width="wrap_content"
           android:layout_height="wrap_content"
           android:textSize="10dp"
           android:text="One,One"/>
       <Button
           android:layout_width="wrap_content"
           android:layout_height="wrap_content"
           android:textSize="10dp"
           android:text="One,Two"/>
       <Button
           android:layout_width="wrap_content"
           android:layout_height="wrap_content"
           android:textSize="10dp"
           android:text="One,Three"/>
       <Button
           android:layout_width="wrap_content"
           android:layout_height="wrap_content"
           android:textSize="10dp"
           android:text="One,Four"/>
   </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Two,One"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Two,Two"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Two,Three"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Two,Four"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Three,One"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Three,Two"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Three,Three"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Three,Four"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Four,One"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Four,Two"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Four,Three"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="10dp"
            android:text="Four,Four"/>
    </LinearLayout>

    <Button
        android:id="@+id/constrain_btn"
        android:layout_marginTop="30dp"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="约束布局"/>


    <Button
        android:id="@+id/table_btn"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="表格布局"/>
</LinearLayout>

约束布局代码xml:
