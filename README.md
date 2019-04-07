# 2.1利用线性布局

运行结果：

![](https://github.com/wjswxx/layout/blob/master/ing/%E5%9B%BE%E7%89%871.png)

代码：

```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <Button
            android:id="@+id/OneOne"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="One,One" />

        <Button
            android:id="@+id/OneTwo"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="One,Two" />

        <Button
            android:id="@+id/OneThree"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="One,Three" />

        <Button
            android:id="@+id/OneFour"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="One,Tour" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:id="@+id/TwoOne"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Two,One"/>
        <Button
            android:id="@+id/TwoTwo"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Two,Two"/>
        <Button
            android:id="@+id/TwoThree"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Two,Three"/>
        <Button
            android:id="@+id/TwoOneFour"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Two,Tour"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <Button
            android:id="@+id/ThreeOne"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Three,One" />

        <Button
            android:id="@+id/ThreeTwo"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Three,Two" />

        <Button
            android:id="@+id/ThreeThree"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Three,Three" />

        <Button
            android:id="@+id/ThreeFour"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Three,Tour" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <Button
            android:id="@+id/FourOne"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Four,One" />

        <Button
            android:id="@+id/FourTwo"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Four,Two" />

        <Button
            android:id="@+id/FourThree"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Four,Three" />

        <Button
            android:id="@+id/FourFour"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Four,Tour" />
    </LinearLayout>
</LinearLayout>
```
# 2.2constrainlayout布局

运行结果：

![](https://github.com/wjswxx/layout/blob/master/ing/%E5%9B%BE%E7%89%874.png)

代码：

```
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <Button
        android:id="@+id/button2"
        android:layout_width="110dp"
        android:layout_height="77dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:background="@color/colorPrimaryDark"
        android:backgroundTint="@android:color/holo_red_dark"
        android:text="RED"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button3"
        android:layout_width="116dp"
        android:layout_height="77dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:backgroundTint="@android:color/holo_orange_dark"
        android:text="ORANGE"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button4"
        android:layout_width="115dp"
        android:layout_height="75dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="16dp"
        android:backgroundTint="@android:color/holo_orange_light"
        android:text="YELLOW"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button5"
        android:layout_width="97dp"
        android:layout_height="83dp"
        android:layout_marginStart="56dp"
        android:layout_marginTop="88dp"
        android:backgroundTint="@android:color/holo_green_light"
        android:text="GREEN"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button2" />

    <Button
        android:id="@+id/button6"
        android:layout_width="93dp"
        android:layout_height="61dp"
        android:layout_marginStart="12dp"
        android:layout_marginTop="96dp"
        android:backgroundTint="@android:color/holo_blue_dark"
        android:text="BLUE"
        app:layout_constraintStart_toEndOf="@+id/button5"
        app:layout_constraintTop_toBottomOf="@+id/button3" />

    <Button
        android:id="@+id/button7"
        android:layout_width="93dp"
        android:layout_height="61dp"
        android:layout_marginStart="16dp"
        android:layout_marginTop="96dp"
        android:backgroundTint="@android:color/holo_purple"
        android:text="INDOGO"
        app:layout_constraintStart_toEndOf="@+id/button6"
        app:layout_constraintTop_toBottomOf="@+id/button4" />

    <Button
        android:id="@+id/button8"
        android:layout_width="745dp"
        android:layout_height="78dp"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:backgroundTint="@color/colorAccent"
        android:text="VIOLET"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent" />
</android.support.constraint.ConstraintLayout>
```
# 2.2利用表格布局

运行结果：

![](https://github.com/wjswxx/layout/blob/master/ing/%E5%9B%BE%E7%89%873.png)

代码：

```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="180dp"
    android:orientation="vertical">

    <TableRow
        android:layout_width="match_parent"
        android:layout_height="30dp">

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:text="Open..." />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="5"
            android:text="         " />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:hint="Ctrl-O" />
    </TableRow>
    <TableRow
        android:layout_width="fill_parent"
        android:layout_height="30dp">

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:text="Save..." />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="5"
            android:text="         " />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:hint="Ctrl-S" />
    </TableRow>
    <TableRow
        android:layout_width="fill_parent"
        android:layout_height="30dp">

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:text="Save As..." />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="5"
            android:text="         " />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:hint="Ctrl-Shift-S" />
    </TableRow>
    <View android:layout_height="1px"
        android:background="#000000"
        android:layout_width="fill_parent">
    </View>
    <TableRow
        android:layout_width="fill_parent"
        android:layout_height="30dp">

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:text="X Import..." />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="5"
            android:text="         " />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:hint=" " />
    </TableRow>
    <TableRow
        android:layout_width="fill_parent"
        android:layout_height="30dp">

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:text="X Export..." />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="5"
            android:text="         " />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:hint="Ctrl-E" />
    </TableRow>
    <View android:layout_height="1px"
        android:background="#000000"
        android:layout_width="fill_parent">
    </View>
    <TableRow
        android:layout_width="fill_parent"
        android:layout_height="30dp">

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:text="Quit" />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="5"
            android:text="         " />

        <TextView
            android:layout_width="0px"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:hint=" " />
    </TableRow>

</LinearLayout>
···
