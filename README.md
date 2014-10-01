<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <title>Windows Event Log Action Plugin</title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
    <meta http-equiv="X-UA-Compatible" content="IE=EmulateIE8" />
    <meta content="Scroll Wiki Publisher" name="generator"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/liquid.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/print.css" media="print"/>
    <link type="text/css" rel="stylesheet" href="css/content-style.css" media="screen, projection, print"/>
    <link type="text/css" rel="stylesheet" href="css/screen.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/print.css" media="print"/>
</head>
<body>
                <h1>Windows Event Log Action Plugin</h1>
    <div class="section-2"  id="158629944_WindowsEventLogActionPlugin-Overview"  >
        <h2>Overview</h2>
    <p>
            <img src="images_community/download/attachments/158629944/icon.png" alt="images_community/download/attachments/158629944/icon.png" class="confluence-embedded-image" />
            </p>
    <p>
The Windows Event Log Action Plugin enables dynaTrace to forward incidents into the Microsoft Windows Event Log.The plugin is based on the Windows &ldquo;eventcreate.exe&rdquo; command and allows event creation on local and remote machines.    </p>
    </div>
    <div class="section-2"  id="158629944_WindowsEventLogActionPlugin-PluginDetails"  >
        <h2>Plugin Details</h2>
    <div class="tablewrap">
        <table>
<thead class=" "></thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Author    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Christian Grimm (<a href="mailto:christian.grimm@compuware.com">christian.grimm@compuware.com</a>)    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
dynaTrace Versions    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
5.5, 5.6    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
License    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_5275722_2_dynaTraceBSD.txt">dynaTrace BSD</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Support    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="https://community/display/DL/Support+Levels">Not Supported</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Known Problems    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Release History    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
2014-03-03 Initial Release<br/>2014-03-04 Backward Compatibility for dynaTrace 5.5    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Download    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_158793845_1_com.compuwareapm.community.plugin.windowseventlogaction_0.8.1.jar">dynaTrace Windows Event Log Action Plugin 0.8.1</a>    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    </div>
    <div class="section-2"  id="158629944_WindowsEventLogActionPlugin-Installation"  >
        <h2>Installation</h2>
    <p>
Import the Plugin into the dynaTrace Server. For details how to do this please refer to the <a href="https://community/display/DOCDT56/Plugin+Management">Online Documentation on Plugin Management</a>.    </p>
    </div>
    <div class="section-2"  id="158629944_WindowsEventLogActionPlugin-Configuration"  >
        <h2>Configuration</h2>
    <p>
The following screenshot shows an example configuration:    </p>
    <p>
            <img src="images_community/download/attachments/158629944/PropertyConfig1.png" alt="images_community/download/attachments/158629944/PropertyConfig1.png" class="confluence-embedded-image" />
            </p>
    <p>
<strong class=" ">System:</strong><br/>Optional. Specifies the remote system to connect to.    </p>
    <p>
<strong class=" ">User:</strong><br/>Optional. [domain\]user specifies the user context under which the command should execute.    </p>
    <p>
<strong class=" ">Password:</strong><br/>Optional. Specifies the password for the given user context.    </p>
    <p>
<strong class=" ">Event Log Name:</strong><br/>Specifies the event log to create an event in.    </p>
    <p>
<strong class=" ">Type:</strong><br/>Specifies the type of event to create. Valid types: SUCCESS, ERROR, WARNING, INFORMATION.    </p>
    <p>
<strong class=" ">Source:</strong><br/>Specifies the source to use for the event (if not specified, source will default to 'eventcreate'). A valid source can be any string and should represent the application or component that is generating the event.    </p>
    <p>
<strong class=" ">ID:</strong><br/>Specifies the event ID for the event. A valid custom message ID is in the range of 1 - 1000.    </p>
    <p>
<strong class=" ">Description:</strong><br/>Specifies the description text for the new event. Variables can be used for dynamic text. Examle:    </p>
    <p>
            <img src="images_community/download/attachments/158629944/PropertyConfig2.png" alt="images_community/download/attachments/158629944/PropertyConfig2.png" class="confluence-embedded-image" />
            </p>
    </div>
    <div class="section-2"  id="158629944_WindowsEventLogActionPlugin-ExampleWindowsEventLog"  >
        <h2>Example Windows Event Log</h2>
    <p>
            <img src="images_community/download/attachments/158629944/ExampleWindowsEventLog.png" alt="images_community/download/attachments/158629944/ExampleWindowsEventLog.png" class="confluence-embedded-image" />
            </p>
    </div>
    <div class="section-2"  id="158629944_WindowsEventLogActionPlugin-Troubleshooting"  >
        <h2>Troubleshooting</h2>
    <p>
Please refer to the log file, which contains the full console output of the Windows Event Log Action Plugin:<br/>%dynaTraceInstallation%/log/server/com.compuwareapm.community.plugin.WindowsEventLogAction.action.0.0.log    </p>
    </div>
    <div class="section-2"  id="158629944_WindowsEventLogActionPlugin-Feedback"  >
        <h2>Feedback</h2>
    <p>
Please provide feedback on this plugin either by commenting on this page or by comments on the <a href="https://community/display/DTFORUM/Community+Plugins+and+Extensions">Community Plugins and Extensions</a>    </p>
    </div>
            </div>
        </div>
        <div class="footer">
        </div>
    </div>
</body>
</html>
