{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# CLI and Dev Tools
{: #cli}

*Last updated: 10 November 2015*

Powerful tools for {{site.data.keyword.Bluemix_short}}.
{:shortdesc}

## ![Command line interfaces](./images/CLI.png) Command line interfaces
{: #downloads}

Download and install command line interfaces to support your {{site.data.keyword.Bluemix_notm}} experience. The Cloud Foundry cf command line interface is a prerequisite for all other {{site.data.keyword.Bluemix_notm}} CLI tools.


| *Cloud Foundry: cf* |	*{{site.data.keyword.IBM}} Containers for {{site.data.keyword.Bluemix_notm}}: ice* | *{{site.data.keyword.Bluemix_notm}} Live Sync: bl* |
|---------------------|---------------|---------------|
| [Download CLI](https://github.com/cloudfoundry/cli/releases)  <br> [View Docs](#.//reference/cfcommands/index.html) |[Download Docker](https://docs.docker.com/installation/) <br> [ice Mac Installer](ftp://public.dhe.ibm.com/cloud/bluemix/cli/Bluemix_ice.pkg) <br> [ice Windows Installer](ftp://public.dhe.ibm.com/cloud/bluemix/cli/Bluemix_ice.exe) <br> [ice Linux Installer](ftp://public.dhe.ibm.com/cloud/bluemix/cli/Bluemix_ice.tar.gz) <br> [View Docs](../containers/container_cli_ice_ov.html) | [Mac Installer](ftp://public.dhe.ibm.com/cloud/bluemix/cli/Bluemix_bl.pkg) <br> [Windows Installer](ftp://public.dhe.ibm.com/cloud/bluemix/cli/Bluemix_bl.exe) <br> [View Docs](./reference/bl/index.html) |


## ![Command line interface plug-ins](./images/CLI_Plugin.png) Command line interface plug-ins

Easily extend your {{site.data.keyword.Bluemix_notm}} command line interface with more commands. To access the {{site.data.keyword.Bluemix_notm}} command line interface plug-ins, see the [{{site.data.keyword.Bluemix_notm}} CLI Plug-in Repository](http://plugins.{DomainName}/).

1. To install cf CLI plug-ins from the {{site.data.keyword.Bluemix_notm}} registry, set the plug-in registry endpoint:
```
cf add-plugin-repo bluemix-cf-staging http://plugins.{DomainName}
```
2. Run the following command to install a plug-in:
```
cf install-plugin plugin_name -r bluemix-cf-staging
```

| *Active Deploy* |  *Development Mode* | {{site.data.keyword.IBM}} Containers for {{site.data.keyword.Bluemix_notm}} |
|-----------------|-----------------|--------------------|----------------------------|
| Plug-in name: active-deploy <br>  [View Docs](../services/ActiveDeploy/index.html#cli) |  Plug-in name: development-name <br> [View Docs](./plugins/dev_mode/index.html) | Plug-in name: ibm-containers <br> [View Docs](../containers/container_cli_cfic.html#container_cli_cfic) |

## ![Integrated development tools](./images/Integrated_Dev_Tools.png) Integrated development tools


Download and install plug-ins to integrate your favorite {{site.data.keyword.Bluemix_notm}} services.

| *{{site.data.keyword.jazzhub_short}}* | *Liberty for Java* | *MobileFirst* | *{{site.data.keyword.rules_short}}* |
|-------------|----------|----------|----------|
| [Egit Eclipse Plug-in](https://hub.jazz.net/docs/reference/gitclient/#eclipse_using_egit) <br> [RTC Eclipse Plug-in](https://hub.jazz.net/docs/reference/gitclient/#eclipse_using_rtc) | [Liberty Eclipse Plug-in](https://developer.ibm.com/wasdev/downloads/liberty-profile-using-eclipse/) | [Eclipse Plug-in](https://marketplace.eclipse.org/content/ibm-mobilefirst-platform-studio) | [Rules Designer Eclipse Plug-in](../services/rules/index.html#rulov002) |