<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.example.auth_practice">

    <!-- Add a uses-permission element to the manifest -->
    <uses-permission android:name="android.permission.INTERNET"/>
    <!-- this one is Optionnal -->
    <!--<uses-permission android:name="com.google.android.gms.permission.AD_ID" tools:node="remove"/>-->

    <queries>
      <provider android:authorities="com.facebook.katana.provider.PlatformProvider"/>
    </queries> 


    <application
        android:label="auth_firebase"
        android:name="${applicationName}"
        android:icon="@mipmap/ic_launcher">
        
        <!-- Add meta-data elements to the application  -->
        <meta-data android:name="com.facebook.sdk.ApplicationId" android:value="@string/facebook_app_id"/>
   	    <meta-data android:name="com.facebook.sdk.ClientToken" android:value="@string/facebook_client_token"/>

        <!-- Add activity for Facebook for Chrome Custom Tabs  -->
        <activity android:name="com.facebook.FacebookActivity"
            android:configChanges=
                    "keyboard|keyboardHidden|screenLayout|screenSize|orientation"
            android:label="@string/app_name" />
        <activity
            android:name="com.facebook.CustomTabActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.VIEW" />
                <category android:name="android.intent.category.DEFAULT" />
                <category android:name="android.intent.category.BROWSABLE" />
                <data android:scheme="@string/fb_login_protocol_scheme" />
            </intent-filter>
        </activity>
        <!-- End of activity for facebook -->


        <activity
            android:name=".MainActivity"
            android:exported="true"
            android:launchMode="singleTop"
            android:theme="@style/LaunchTheme"
            android:configChanges="orientation|keyboardHidden|keyboard|screenSize|smallestScreenSize|locale|layoutDirection|fontScale|screenLayout|density|uiMode"
            android:hardwareAccelerated="true"
            android:windowSoftInputMode="adjustResize">
            <!-- Specifies an Android theme to apply to this Activity as soon as
                 the Android process has started. This theme is visible to the user
                 while the Flutter UI initializes. After that, this theme continues
                 to determine the Window background behind the Flutter UI. -->
            <meta-data
              android:name="io.flutter.embedding.android.NormalTheme"
              android:resource="@style/NormalTheme"/>
            
            <intent-filter>
                <action android:name="android.intent.action.MAIN"/>
                <category android:name="android.intent.category.LAUNCHER"/>
            </intent-filter>

        </activity>
        <!-- Don't delete the meta-data below.
             This is used by the Flutter tool to generate GeneratedPluginRegistrant.java -->
        <meta-data
            android:name="flutterEmbedding"
            android:value="2" />
    </application>
</manifest>
