---
title: Widget FAQs
layout: page
order: 1
---

# {{ page.title }}

**What is a widget?**

A widget is an app extension that gives the user a quick view of your app’s content on the home screen.  Tapping on the widget opens your app for a more detailed look.


**Can a single app have more than one widget?**

Yes.  You can define multiple types of widgets for your app.  It’s recommended to include all widgets in the same widget extension, but you can have separate extensions if necessary.

Your users can also add multiple copies of the same widget to their home screen, each customized differently.


**Can a user customize the widget?**

Yes, if your app includes a custom intent.  The intent can take in any type of user data, like a zipcode needed to track local weather, or package number to track a delivery.


**Are widgets required to be built with SwiftUI?**

iOS 14 widgets designed for the home screen must use SwiftUI.  The earlier widgets seen on the Today view can still use UIKit.


**Can a user add a widget without ever opening the widget’s app?**

No.  In order for a widget to even show up as an option in the Widget Gallery, the user must open the associated app at least once.
