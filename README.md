<p align="center">
    <a href="https://github.com/dlamspl/splunk_attack_range_reporting/releases">
        <img src="https://img.shields.io/github/v/release/dlamspl/splunk_attack_range_reporting" /></a>
    <a href="https://github.com/dlamspl/splunk_attack_range_reporting/graphs/contributors" alt="Contributors">
        <img src="https://img.shields.io/github/contributors/dlamspl/splunk_attack_range_reporting" /></a>
</p>

# Splunk Attack Range Reporting

![Logo](appserver/static/docs/img/logo.png?raw=true "Logo")

A Splunk App for Attack Range Reporting. Provides dashboards for insights on your attack range simulations. 

The Splunk Attack Range project can be found [here](https://github.com/splunk/attack_range).

## What is it ?
It is a Splunk app that provides dashboards that enable a user of Splunk Attack Range to have better view of what simulations were run, relevant security content from other Splunk apps and overview of the available Atomic Red tests.

## Compatibility and dependencies
v1.0.x of the app is compatible with the following:

+ Splunk 8.x or later
+ [Splunk Security Content v3.x or later](https://splunkbase.splunk.com/app/3449/)
+ [Security Security Essentials v3.x or later](https://splunkbase.splunk.com/app/3435/)

### Dependencies
This application has the following depencencies:

+ [Splunk Security Essentials v3.x.x](https://splunkbase.splunk.com/app/3435/) _(Installed with Attack Range)_
+ [Punchcard - Custom Visualization](https://splunkbase.splunk.com/app/3129/)
+ [Status Indicator - Custom Visualization](https://splunkbase.splunk.com/app/3119/)
+ [Sankey Diagram - Custom Visualization](https://splunkbase.splunk.com/app/3112/)
+ [Parallel Coordinates - Custom Visualization](https://splunkbase.splunk.com/app/3137)
+ [Treemap - Custom Visualization](https://splunkbase.splunk.com/app/3118)

**Note:** The application will fallback to not showing any panels that rely on prerequisite visualizations if they are missing.

## What does it look like ?

The Main dashboard gives you an overview of the simulations run, users, hosts, MITRE ATT&CK tactics and techniques, tests executed and potential mapping with analytic stories. 

![Main Dashboard](appserver/static/docs/img/ar_main_dashboardv1.0.png?raw=true "Main Dashboard")

The second dashboard (Navigator) shows all the available Atomic Red tests and their potential mappings to security content.  The reason we categorize those as "potential" is because the mapping is simply made based on the MITRE technique/subtechnique referenced in the test and the security content. This does not necessarily mean that a specific Atomic Red Test will trigger a particular detection.   This is where you should read more on what ATT&CK is all about and how the Splunk [Security Content](https://research.splunk.com) maps to it.  :)

![Navigator](appserver/static/docs/img/ar_navigator_dashboardv1.0.png?raw=true "Navigator")

The 3rd dashboard allows you to search for potential Splunk Security Detections, Atomic Red Tests or determine PurpleSharp support for one or more MITRE Att&ck Technique/Subtechnique.

![MITRE Content Based Search](appserver/static/docs/img/ar_mitre_content_search_dashboard.png?raw=true "Content Search")

Finally there is a dashboard made with Splunk dashboards - Beta which looks nice but still in beta !

![Main - Beta](appserver/static/docs/img/ar_dashboards_beta_preview.png?raw=true "Main-Beta")

## Contributors
[Christian Cloutier](https://github.com/ccl0utier)