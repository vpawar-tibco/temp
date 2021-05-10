# Visual diff viewer metadata files for TIBCO ActiveMatrix BusinessWorks™ Plugins

The Visual Process Diff tool provides the ability to view changes made to process files visually for different revisions. For the plugins to participate in the diff viewer, a mapping file in the JSON format needs to be created. This mapping file contains the information related to each activity's UI fields and the corresponding EMF attribute.

## Prerequisites
1. Either of TIBCO ActiveMatrix BusinessWorks™ or TIBCO BusinessWorks™ Container Edition should be installed.
2. Visual diff Tool should be enabled either on TIBCO ActiveMatrix BusinessWorks™ or TIBCO BusinessWorks™ Container Edition.


## Setup 

### Setp 1 : Enabling Visual Diff Tool
To enable diff viewer, navigate to **Windows > Preferences > BusinessWorks > Team Development**
Select the Enable visual diff check box under Diff Tool Options. By default, this check box is always selected.
	![](./images/Enable-Visual-Diff.png)

### Step 2 : Copy the JSON files to the following locations	
`<TIBCO_HOME> -> bw -> <BW_VERSION> -> system -> mappings -> palettes`

`<TIBCO_HOME> -> bw -> <BW_VERSION> -> system -> mappings -> sr`
> Note: If mappings and its subfolders are not available, please create the folders manually.

## How to use Diff Viewer

## Prerequisites
1. Import a sample project or create a new BusinessWorks Application project.
2. The selected process should be modified and saved at least once before comparing the two revisions. This ensures that there is a local history available in the workspace.

## Steps for Process Diff Viewer
1. In Project Explorer view, right-click on the selected process and select **Compare With > Local History or Team > Show Local History**
![](./images/bw-process-compare-with-local-history.png)
	The **History** tab is displayed.
2. On the **History** tab, select the two different revisions to compare. Right-click and select **Compare with Each Other** option.
![](./images/bw-process-compare-with-each-other.png)
A **BW Compare** view is displayed, that displays the visual diff between the two different revisions of the selected process.
![](./images/bw-compare.png)

In the above example, there is a change in the **General** and **Description** tab hence they are marked in blue.


- After comparing the different revisions of a process, the diff viewer displays the process with decorations to indicate the changes in activities. It also navigates controls through the modified activities and their properties.
![](./images/bw-process-after-comparing-with-local-history.png)
- Change Indicators- These are small indicators displayed on the process to indicate the activity change.
![](./images/change-indicators.png)



On the **General** tab, a change is made in the **Name** field, hence it is highlighted in yellow.

### For more details, please refer the following documentation: [Diff Viewer](https://docs.tibco.com/pub/bwce/2.6.0/doc/html/GUID-97FE2042-9D75-43D2-8957-827CF0902835.html)
