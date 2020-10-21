---
layout: page
title: Widgets
---

FAQs
What is a widget?
A widget is an app extension that gives the user a quick view of your app’s content on the home screen.  Tapping on the widget opens your app for a more detailed look.
Can a single app have more than one widget?
Yes.  You can define multiple types of widgets for your app.  It’s recommended to include all widgets in the same widget extension, but you can have separate extensions if necessary.

Your users can also add multiple copies of the same widget to their home screen, each customized differently.
Can a user customize the widget?
Yes, if your app includes a custom intent.  The intent can take in any type of user data, like a zipcode needed to track local weather, or package number to track a delivery.
Are widgets required to be built with SwiftUI?
iOS 14 widgets designed for the home screen must use SwiftUI.  The earlier widgets seen on the Today view can still use UIKit.
Can a user add a widget without ever opening the widget’s app?
No.  In order for a widget to even show up as an option in the Widget Gallery, the user must open the associated app at least once. 
Widget Setup
A widget needs the following information:
Kind: this is a unique identifier and should be descriptive of the particular widget
Provider: an object that conforms to a TimelineProvider and will produce a timeline of custom TimelineEntry objects that defines when the widget’s display should be updated
Content: a close of SwiftUI views that gets called with a TimelineEntry each time the widget needs to be rendered
(optional) Custom Intent: defines user-configurable properties
Custom Intents
If you want users to be able to customize the widget, you’ll need to include Configuration Intents when creating the original Widget Extension.
StaticConfiguration: for widgets that don’t have user-configurable properties
IntentConfiguration: for widgets with user-configurable properties that will be defined by SiriKit intents

Timeline Providers
Timeline providers conform to the TimelineProvider protocol and specify when a widget’s display should be updated.  TimeEntry...
