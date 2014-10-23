```
public class SplashBroadcastReceiver extends BroadcastReceiver {
    public void onReceive(Context context, Intent intent) {
        Toast.makeText(
                context,
                intent.getStringExtra("SplashServiceBroadcast"),
                Toast.LENGTH_LONG
        ).show();
    }
}
```

```
public class SplashService extends IntentService {
    // Constructors omitted
    @Override
    protected void onHandleIntent(Intent intent) {
        Intent broadcastIntent = new Intent("SplashBroadcast");

        broadcastIntent.putExtra("SplashServiceBroadcast", "Hello, World!");
        sendBroadcast(broadcastIntent);
    }
}
```
