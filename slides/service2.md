```
public class SplashService extends IntentService {
    public SplashService() {
        super(TAG);
    }

    public SplashService(String name) {
        super(name);
    }

    @Override
    protected void onHandleIntent(Intent intent) {
        Toast.makeText(this, "Hello, World!", Toast.LENGTH_LONG).show();
    }
}
```
