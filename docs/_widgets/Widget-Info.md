---
layout: page
title: Widget Info
---

{{ page.title }}

# Widget Setup
A widget needs the following information:
* Kind: this is a unique identifier and should be descriptive of the particular widget
* Provider: an object that conforms to a TimelineProvider and will produce a timeline of custom TimelineEntry objects that defines when the widget’s display should be updated
* Content: a close of SwiftUI views that gets called with a TimelineEntry each time the widget needs to be rendered
(optional) Custom Intent: defines user-configurable properties

# Custom Intents
If you want users to be able to customize the widget, you’ll need to include Configuration Intents when creating the original Widget Extension.
* StaticConfiguration: for widgets that don’t have user-configurable properties
* IntentConfiguration: for widgets with user-configurable properties that will be defined by SiriKit intents

# Timeline Providers
Timeline providers conform to the TimelineProvider protocol and specify when a widget’s display should be updated.  TimeEntry...