# aos_sdk
Android SDK Guide

어드민에 매체를 등록한 후 APP_ID 를 발급 받는다.
APP_ID 를 AndroidManifest.xml 파일에 등록한다.
'''xml
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android">

    <application
        android:usesCleartextTraffic="true"
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.S2sdk">
        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>

        <activity android:name="s2.adapi.sdk.offerwall.S2OfferwallActivity" android:exported="true"/>

        <meta-data android:name="s2_app_id" android:value="0d724e96d380f016521e1bba1d9142eae52893d29f484033cb06c3ad0f2ca651" />
    </application>

</manifest>
'''
