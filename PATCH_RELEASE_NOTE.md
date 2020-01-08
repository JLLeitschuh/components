---
version: 7.2.1
module: https://talend.poolparty.biz/coretaxonomy/42
product:
- https://talend.poolparty.biz/coretaxonomy/23
---

# TPS-3575 <!-- mandatory -->

| Info             | Value |
| ---------------- | ---------------- |
| Patch Name       | Patch\_20200108\_TPS-3575\_v1-7.2.1 |
| Release Date     | 2020-01-08 |
| Target Version   | 20190620\_1446-V7.2.1 |
| Product affected | Talend Studio |

## Introduction <!-- mandatory -->

This is the first patch of Netsuite component for 7.2.1.

**NOTE**: For information on how to obtain this patch, reach out to your Support contact at Talend.

## Fixed issues <!-- mandatory -->

This is the first patch of Netsuite components for 7.2.1 and it contains the following fix:

- TPS-3575 [7.2.1] Unable to retrieve schema for NetsuiteInput/Output (TDI-42556)

## Prerequisites <!-- mandatory -->

Consider the following requirements for your system:

- Talend Studio 7.2.1 must be installed.
- Patch TPS-3570 must be installed.

## Installation <!-- mandatory -->

<!--
- Detailed installation steps for the customer.
- If any files need to be backed up before installation, it should be mentioned in this section.
- Two scenarios need to be considered for the installation:
 1. The customer has not yet installed any patch before => provide instructions for this
 2. The customer had installed one previous cumulative patch => provide instructions for this
-->
### Installing the patch using Software update <!-- if applicable -->

1) Logon TAC and switch to Configuration->Software Update, then enter the correct values and save referring to the documentation: https://help.talend.com/reader/f7Em9WV_cPm2RRywucSN0Q/j9x5iXV~vyxMlUafnDejaQ

2) Switch to Software update page, where the new patch will be listed. The patch can be downloaded from here into the nexus repository.

3) On Studio Side: Logon Studio with remote mode, on the logon page the Update button is displayed: click this button to install the patch.

### Installing the patch using Talend Studio <!-- if applicable -->

1) Create a folder named "patches" under your studio installer directory and copy the patch .zip file to this folder.

2) Restart your studio: a window pops up, then click OK to install the patch, or restart the commandline and the patch will be installed automatically.

### Installing the patch using Commandline <!-- if applicable -->

Execute the following commands:

1. Talend-Studio-win-x86_64.exe -nosplash -application org.talend.commandline.CommandLine -consoleLog -data commandline-workspace startServer -p 8002 --talendDebug
2. initRemote {tac_url} -ul {TAC login username} -up {TAC login password}
3. checkAndUpdate -tu {TAC login username} -tup {TAC login password}

## Uninstallation <!-- if applicable -->

In case this patch cannot be uninstalled, it is your responsibility to define the backup procedures for your organization before installing.

## Affected files for this patch <!-- if applicable -->

The following files are installed by this patch:

- configuration/.m2/repository/org/talend/components/components-netsuite-definition/0.27.4/components-netsuite-definition-0.27.4.jar
- configuration/.m2/repository/org/talend/components/components-netsuite-runtime/0.27.4/components-netsuite-runtime-0.27.4.jar
- configuration/.m2/repository/org/talend/components/components-netsuite-runtime_2014\_2/0.27.4/components-netsuite-runtime\_2014\_2-0.27.4.jar
- configuration/.m2/repository/org/talend/components/components-netsuite-runtime_2016\_2/0.27.4/components-netsuite-runtime\_2016\_2-0.27.4.jar
- configuration/.m2/repository/org/talend/components/components-netsuite-runtime_2018\_2/0.27.4/components-netsuite-runtime\_2018\_2-0.27.4.jar
- plugins/org.talend.components.netsuite\_0.27.4.jar
