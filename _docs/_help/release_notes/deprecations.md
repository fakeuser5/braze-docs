---
nav_title: Deprecations
page_order: 10
---
# About Deprecations

Technology is always moving - inside Braze and outside it! And we do our best to keep up with it. Here, you'll find the origins of Braze and it's technology - how we supported people in the "before time" - before now, anyway...

You might have gotten here from searching a term for an integration or feature that no longer exists. This is our attempt to keep you informed on our progress and movement within the technology industry.

## Feedback

_Braze Feature_

_Support to be completely withdrawn July 1, 2019._

The Braze SDK provided a feedback widget that could be added to your app to allow users to leave feedback using the submitFeedback method and pass it into either Desk.com or Zendesk and was managed on the dashboard.

## Google Cloud Messaging (GCM)

_Replaced by: [Firebase Cloud Messaging (FCM)]({{ site.baseurl }}/developer_guide/platform_integration_guides/android/push_notifications/integration/#firebase-integration)_

_Integration_

_Support to be completely withdrawn between July 2018 and April 2019._

[Google will be removing support for GCM](https://developers.googleblog.com/2018/04/time-to-upgrade-from-gcm-to-fcm.html) as early as April 11, 2019. Braze may remove support for GCM from the Android SDKs at any point after July 31, 2018, which will be noted within [our Android SDK changelogs](https://github.com/Appboy/appboy-android-sdk/blob/master/CHANGELOG.md). This means that existing GCM tokens will continue to work and you will be able to message your existing users. However, you will not be able to message new users.

Customers that have not already migrated to [Firebase Cloud Messaging (FCM)]({{ site.baseurl }}/developer_guide/platform_integration_guides/android/push_notifications/integration/#firebase-integration) may be affected by this change.

If you have not transitioned to FCM by April 11, 2019, all GCM push tokens registrations will fail. If your apps are currently supporting GCM, you’ll need to work with your development teams on transitioning from GCM to Firebase Cloud Messaging (FCM).


## Eclipse

_Replaced by: [Android Studio]({{ site.baseurl }}/developer_guide/platform_integration_guides/android/initial_sdk_setup/android_sdk_integration/#using-android-studio)_

_Integration_

_Support withdrawn: 2014-2015_

Braze has deprecated support for the Eclipse IDE as [Google is sunsetting support for the Eclipse Android Developer Tools Plugin](http://android-developers.blogspot.com/2015/06/an-update-on-eclipse-android-developer.html). If you need assistance with your Eclipse integration prior to migration please [email Support]({{ site.baseurl }}/support_contact/) for assistance.

## The Raw Event Stream (RES)

_Replaced by: [Currents]({{ site.baseurl }}/technology_partners/currents/about/)_

_Braze Feature_

_Support withdrawn: July 2018_

The Raw Event Stream was the predecessor to [Currents]({{ site.baseurl }}/technology_partners/currents/about/) and was deprecated to make room for the future of Braze data.

## Delay While Idle

_Replaced by: n/a_

_GCM Feature_

_Support withdrawn: November 2016_

The Delay While Idle parameter was previously a part of the [GCM push options](https://developers.google.com/cloud-messaging/http-server-ref). Google withdrew support for this option on November 15th 2016. Previously, when set to **true**, it indicated that the message should not be sent until the device becomes active.


[11]: {% image_buster /assets/img_archive/feedback_dashboard_example.png %} "Feedback Response Dashboard"