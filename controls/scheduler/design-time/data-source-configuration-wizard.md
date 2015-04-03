---
title: Data Source Configuration Wizard
page_title: Data Source Configuration Wizard | UI for ASP.NET AJAX Documentation
description: Data Source Configuration Wizard
slug: scheduler/design-time/data-source-configuration-wizard
tags: data,source,configuration,wizard
published: True
position: 1
---

# Data Source Configuration Wizard



The Data Source Configuration Wizard helps you bind a __RadScheduler__ control to a data source and specifythe fields that provide data for appointment properties. There are two ways to display the Data Source Configuration Wizard:

* Right click the __RadScheduler__ and select __Choose Data Source...__

* Bring up the __RadScheduler__[Smart Tag]({%slug scheduler/design-time/smart-tag%}) and click on __Choose Data Source ...__

>note Clicking on the __DataSourceID__ property of the scheduler does not start the scheduler'sData Source Configuration Wizard, only the standard Microsoft Data Source Configuration Wizard. If you choose to bind yourscheduler this way, you will need to enter the field bindings separately.
>


## Data Source Configuration Wizard

1. If you have already added a DataSource component to your page, you can select the DataSource from the __Select adatasource__ drop-down list. If you do not have a DataSource component on the page, select<New data source...> from the list; the wizard will guide you through the steps of defining a new datasource. For more information on how to define a new data source, see [Data Source Configuration Wizard](http://msdn.microsoft.com/en-us/library/w4dd7z6t(VS.80).aspx) on the Microsoft Web site. There are also examples in the[Getting Started]({%slug scheduler/getting-started%}) tutorial and in[Using The Data Source Property]({%slug scheduler/data-binding/using-the-data-source-property%}).

1. Once you have selected a data source, you must specify the fields that the __RadScheduler__uses to represent aspects of an appointment.

* The __Key field__ is a unique identifier of the record for a specificappointment. This field is required.

* The __Start Time field__ holds the starting time of the appointment.This field is required.

* The __End Time field__ holds the ending time of the appointment.This field is required.

* The __Subject field__ holds the subject of the appointment.This field is required.

* The __Description field__ holds the description of the appointment.As this field is optional by default it is not enabled. To enable it you need to set the__EnableDescriptionField="true"__.

* The __Reminder field__ holds a string that encodes information about the reminders of the appointments.This field is only needed if you want to allow reminders by __Reminders-Enabled="true"__. For more information see [Reminders Overview]({%slug scheduler/reminders/overview%})

* The __Recurrence Storage field__ holds a string that encodes information about the recurrence of the appointment (its frequency, and how long the recurrence persists). This field is only needed if you want to allowrecurring appointments. If you do allow recurring appointments, you must also set the Recurrence Parent Key field.

* The __Recurrence Parent Key field__ is used when the user edits a single occurrence of a recurringappointment. It holds the key field for the recurring appointment definition of which the single occurrence is a member.

![Data Source Configuration](images/scheduler_datasourceconfiguration.png)

# See Also

 * [Overview]({%slug scheduler/data-binding/overview%})