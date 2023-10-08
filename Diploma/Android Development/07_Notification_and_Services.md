# Broadcast Receiver
- Broadcast is a system-wide event that occurs when system starts, airplane mode, Bluetooth, Wi-Fi, etc…
- Broadcast receiver are used to respond to these system-wide events/intents.
- Broadcast receiver allows us to register for the system events, and application events, and when that even happens, then register receiver got notified.
**There are mainly two types of Broadcast Receivers:**
1. **Static Broadcast Receivers:** These types of Receivers are declared in the manifest file and works even if the app is closed.
2. **Dynamic Broadcast Receivers:** These types of receivers work only if the app is active or minimized.
**Intents:** `android.intent.action.BATTERY_LOW`, `android.intent.action.BOOT_COMPLETED`, `android.intent.action.CALL`, `android.intent.action.DATE_CHANGED`, `android.intent.action.DATE_CHANGED`, `android.net.conn.CONNECTIVITY_CHANGE`, `android.intent.ACTION_AIRPLANE_MODE_CHANGED`.
```java
public class changeAirplaneMode extends BroadcastReceiver{
	@override
	public void onReceiver(Context context, Intent intent){
		if (isAirplaneModeOn(context.getApplicationContext())){
			Toast.MakeText(context, "Airplane Mode On", Toast.Length_Long).show();
		}
		else{
			Toast.MakeText(context, "Airplane Mode Off", Toast.Length_Long).show();
		}
	}
}
```
**There are 2 different type to register broadcast receiver:**
1. **Statically (manifest-declared):** The receiver can be registered via AndroidManifest.xml file.
2. **Dynamically (context-registered):** This registers a receiver dynamically via the Context.registerReceiver() method.

# Notification
- It is a message you can display to the user outside the normal UI's.
- When you tell the system to issue a notification, it first appears as an icon in the notification area.
- To see the details of notification, user have to open notification drawer.
- Both the notification area and the notification drawer are system-controlled areas that the user can view at any time.
- `NotificationCompact.Builder mBuilder = new NotificationCompact.Builder(this)`
- **Some notification areas are:**
	1. **setSmallIcon()**.
	2. **setContentTitle()**.
	3. **setContentText()**.
	4. **setAutoCancel()**.
	5. **setPriority()**.

# Services
- It is an android component that allows an application to run in background to perform long-running tasks.
- The prime aim of the service is to ensure that the application is running in the background so that the user can operate many applications at the same time.
- A service can continuously in background even if user closed or switches to another location.
![Types of Services](https://media.geeksforgeeks.org/wp-content/uploads/20200911235638/Typesofandroidservices-660x404.png)
#### 1. Foreground Services:
- Services that notify user about its ongoing operation.
- User can interact with the services by notification provided.
- Ex- Downloading of file.
#### 2. Background Services:
- Services that do not notify user about its ongoing operation.
- User can not interact with the services by notification provided.
- Ex- Syncing of data.
#### Bound Services:
- Services that allows components of application to bound themselves with it.
- These services perform their tasks as long as any of the application components is bound with it.
- More than one component is allowed to bind themselves with a service at a time. 
- In order to bind an application component with a service, **bindService()** method is used.

### Life Cycle of Services
##### 1. Started Service (Unbounded Services):
- Service will initiate when an application component call the `startService()`.
- Once initiated, the service can run continuously in the background even if the component is destroyed which was responsible for the start of the service.
- To stop the service, one of these two methods can be used:
	1. By calling `stopService()` method.
	2. The service can stop service by itself by invoke `stopSelf()` method.
##### 2. Bounded Services:
-  Service will initiate when an application component is bounded with service `bindService()`.
- To stop the execution of this service, all the components must unbind themselves from the service by using **unbindService()** method.
![Lifecycle of Service](https://static.javatpoint.com/images/androidimages/service_lifecycle.png)
