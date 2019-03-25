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
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="RED"
        android:textColor="#ffffff"
        android:background="#FF0000"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="72dp"
        android:layout_marginEnd="8dp"
        android:text="ORANGE"
        android:textColor="#ffffff"
        android:background="	#FFA500"
        app:layout_constraintEnd_toStartOf="@+id/button3"
        app:layout_constraintHorizontal_bias="0.016"
        app:layout_constraintStart_toEndOf="@+id/button"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginEnd="8dp"
        android:text="YELLOW"
        android:textColor="#ffffff"
        android:background="#FFD700"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button4"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="44dp"
        android:layout_marginTop="68dp"
        android:text="GREEN"
        android:textColor="#ffffff"
        android:background="#2E8B57"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button" />

    <Button
        android:id="@+id/button5"
        android:layout_width="wrap_content"
        android:layout_height="52dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="64dp"
        android:layout_marginEnd="8dp"
        android:text="BLUE"
        android:textColor="#ffffff"
        android:background="#0000FF"
        app:layout_constraintEnd_toStartOf="@+id/button6"
        app:layout_constraintStart_toEndOf="@+id/button4"
        app:layout_constraintTop_toBottomOf="@+id/button2" />

    <Button
        android:id="@+id/button6"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="64dp"
        android:layout_marginEnd="40dp"
        android:text="INDIGO"
        android:textColor="#ffffff"
        android:background="#4B0082"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button3" />

    <Button
        android:id="@+id/button7"
        android:layout_width="373dp"
        android:layout_height="42dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="88dp"
        android:layout_marginEnd="8dp"
        android:text="VIOLET"
        android:textColor="#ffffff"
        android:background="#EE82EE"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.636"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button5" />
</android.support.constraint.ConstraintLayout>

表格布局代码xml文件：
