```java
public class SplashActivity extends FragmentActivity {
    @Override
    public void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.main);
        getSupportFragmentManager()
                .beginTransaction()
                .replace(R.id.fl_fragment_container,
                    new SplashFragment(), "SplashFragment")
                .commit();
    }
}
```

```xml
<?xml version="1.0" encoding="utf-8"?>
<!-- main.xml -->
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
              android:layout_width="match_parent"
              android:layout_height="match_parent">
    <FrameLayout android:id="@+id/fl_fragment_container"
                 android:layout_width="match_parent"
                 android:layout_height="match_parent"/>
</LinearLayout>
```
