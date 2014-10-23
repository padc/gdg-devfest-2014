```java
public class SplashFragment extends Fragment {
    @Override
    public View onCreateView(
                LayoutInflater inflater, ViewGroup container,
                Bundle savedInstanceState) {
        return inflater.inflate(R.splash_fragment, container, false);
    }
}
```

```xml
<?xml version="1.0" encoding="utf-8"?>
<!-- splash_fragment.xml -->
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
              android:orientation="vertical"
              android:layout_width="match_parent"
              android:layout_height="match_parent"
              android:gravity="center">
    <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Hello, World!"
            android:textSize="40sp"
            android:gravity="center"/>
</LinearLayout>
```
