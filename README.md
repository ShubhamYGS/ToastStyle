# ToastStyle
Android Studio- Toast Messages with some Effects :)

### Screenshot:

![whatsapp image 2019-01-10 at 4 03 25 pm](https://user-images.githubusercontent.com/33577947/50962986-7be83480-14f1-11e9-9b57-d3955ff26438.jpeg)


Getting bored with old simple looking Toast Messages. So here I am presenting some amazing toast message style's for you.

# How to get? 
* Note: Here, I only show you the one text style other you can try.
* Special Thanks to GrenderG for making these toast style's.

## Step 1: Add these lines in Build.gradle (Project)
```
allprojects {
    repositories {
        google()
        jcenter()
        maven { url "https://jitpack.io" }
    }
}
```
## Step 2: Add this line in Build.gradle (app)
```
implementation 'com.github.GrenderG:Toasty:1.3.0'
```
## Step 3: Sync your projcet
## Step 4: Create Button in Activity_Main.xml
```
<Button
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:textAlignment="center"
        android:layout_centerVertical="true"
        android:id="@+id/button"
        android:text="This is Toast Button"
        />
```
## Step 5: Implement OnClickListener in Main_Activity.java file
```
Button b1;
b1=(Button)findViewById(R.id.button);

        b1.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Toasty.error(MainActivity.this,"This is Error Message", Toast.LENGTH_LONG).show();
            }
        });
 ```
 
 ## bingo! You did it :)
