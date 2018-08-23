# Updatelibrary
apk下载工具类，支持自动删除下载的apk

1.添加依赖



2.注册广播接收者

 <receiver android:name="com.plgf.updatelibrary.receiver.InstallReceiver">
            <intent-filter android:priority="20">
                <action android:name="android.intent.action.DOWNLOAD_COMPLETE" />
            </intent-filter>
        </receiver>

3.
downloadId = UpdateAppManager.downloadApk(UpdateActivity.this, url, "版本升级", "apk");

查询进度百分比
(int) (((pross[0]*1.0)/pross[1])*100)



