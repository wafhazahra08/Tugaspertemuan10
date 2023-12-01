# Tugaspertemuan10

Nama : Wafha Zahra Mulqiya

NIM : 312210577

Kelas : TI.22.A.5

Mata Kuliah : Pemrograman Mobile 1

Dosen : Donny Maulana S.Kom.,M.M.S.I

##TUGAS

Buatlah tampilan menu Versi 02 dari project-project yang sudah dibuat sebelumnya

dengan tambahan memanggil method Maps

dengan tampilan sebagai berikut :

![launcher](https://github.com/wafhazahra08/Tugaspertemuan10/assets/131223804/c5f31d58-4a54-4a46-a483-49afd7028667)

##1. MENU UTAMA

Pertama yang harus kita lakukan adalah mengganti tampilan menu utamanya dengan code yang baru agar ikon tombol berubah menjadi gambar, caranya adalah : Jika awal pembuatan project kita memilih template Empty Views Activity, maka pada layout otomatis terbuat file activity_main.xml dan pada java akan ada MainActivity.java. Maka langsung saja kita buka activity_main.xml, dan buat code seperti berikut ini:

'''
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context="com.example.ProjectWafha.MainActivity">
    <RelativeLayout
        android:layout_width="500dp"
        android:layout_height="match_parent"
        android:background="@drawable/bghome">
    </RelativeLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginLeft="16dp"
        android:layout_marginTop="100dp"
        android:layout_marginRight="16dp"
        android:orientation="vertical">
        <TextView
            android:id="@+id/textView"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:fontFamily="serif"
            android:text="Menu Program Wafha"
            android:textAlignment="center"
            android:textColor="@color/white"
            android:textSize="34sp"
            android:textStyle="bold" />
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="150dp"
            android:layout_margin="5dp"
            android:orientation="horizontal">
            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu1"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">
                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">
                    <ImageView
                        android:id="@+id/imageView0"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/iconhello" />
                    <TextView
                        android:id="@+id/textView0"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Hello World"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu2"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">
                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">
                    <ImageView
                        android:id="@+id/imageView1"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/iconcount" />
                    <TextView
                        android:id="@+id/textView1"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Fibonacci"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
        </LinearLayout>
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="150dp"
            android:layout_margin="5dp"
            android:orientation="horizontal">
            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu3"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">
                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">
                    <ImageView
                        android:id="@+id/imageView2"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/iconscroll" />
                    <TextView
                        android:id="@+id/textView2"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Scroll Movie"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu4"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">
                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">
                    <ImageView
                        android:id="@+id/imageView3"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/iconalarm" />
                    <TextView
                        android:id="@+id/textView3"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Alarm"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
        </LinearLayout>
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="150dp"
            android:layout_margin="5dp"
            android:orientation="horizontal">
            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu5"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">
                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">
                    <ImageView
                        android:id="@+id/imageView4"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/iconactivity" />
                    <TextView
                        android:id="@+id/textView4"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Two Activity"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu6"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">
                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">
                    <ImageView
                        android:id="@+id/imageView5"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/iconmaps" />
                    <TextView
                        android:id="@+id/textView5"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Maps"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
        </LinearLayout>
    </LinearLayout>
</RelativeLayout>
'''

