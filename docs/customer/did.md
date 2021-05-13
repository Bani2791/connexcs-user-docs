# DID
**Management :material-menu-right: Customer :material-menu-right: [Customer Name] :material-menu-right: DID**

A **Direct Inward Dial (DID)** number is one that exists on the public telephone network. When dialed, the carrier delivers the call to ConnexCS, which then passes it to the customer based on the settings configured here, allowing inbound calls to bypass a PBX or other routing to connect directly to the destination number. 

Create and edit **DID (Direct Inward Dial)** parameters within the individual customer cards, either using `Bulk Upload` or manually **Configure DID** as shown below. 

!!! tip "Stats Button"
    Use the **`Stats`** button to view the **Per Number Report** of DIDs.
    
!!! note "Global DID"
    DID may also be configured and managed for specific Customers or Carriers under **Global :material-menu-right: DID**, which displays all configured DID.
    


## Configure DID
To configured individual DIDs, click the :material-plus::

### Basic
+ **Customer**: Assign the number to the customer.
+ **Customer Card**: Select the desired billing (see [**Customer Rate Cards**](https://docs.connexcs.com/customer-ratecard/) for configuration).
+ **Provider**: Select the Carrier desired for routing.
+ **Provider Card**: Select from Carrier Cards assigned to that Carrier (see [**Provider Rate Cards**](https://docs.connexcs.com/provider-ratecard/) for configuration).
+ **DID**: Enter the specific number. 
+ **Retain Display Name**: If Enabled, it will display the Name in the FROM field of the SIP INVITE. 
+ **Enabled**: Enable or Disable the DID

### Destination
Select where to deliver calls that come in for the DID:

+ **URI**: Set the Destination DID (number or extension) and IP to forward calls to a specific SIP URI
+ **External**: To send the call back out to the internet, use a prefix (defined in Customer > Routing) to select the outbound route, then the number to send the call to
+ **Internal**: Send internally to an extension, a Class5 feature, or even to another customer
+ **Circuit Test**: *in progress*


### Capacity Limits
Set maximum number of INBOUND concurrent calls in **Channels**, and Calls Per Second (CPS) in **Flow Speed**. 

### Media
For more details on these fields, see [**Media in Customer Routing**](https://docs.connexcs.com/customer/routing/#media). 

+ **RTP Proxy Mode**: If connection via our service fails, and relaxed is selected, it will failover to backup automatically.
    
    :material-menu-right: `Strict`- This will enforce the proxy engagement. 
    
    :material-menu-right: `Relaxed`- This will perform best efforts to engage the RTP Proxy, if it can't then the calls will connect directly.

+  **RTP Media Proxy**: This defaults to Auto but selecting a zone (by continent) is the current recommendation. The following options allow you to set where RTP media server for this route for this customer:
    
    :material-menu-right: `Auto`- Selects the least expensive path between your customer and provider.
    
    :material-menu-right: `Direct RTP (no proxy)`- Bypass ConnexCS, so media flows directly between the customer and carrier. 
    
    :material-menu-right: `Zone (recommended)`- Select any of the regional servers

+ **Call Recording**: Select the percent of calls to record for this customer
    + Disabled- never record calls
    + 1% Sampling
    + 5% Sampling
    + 25% Sampling
    + 50% Sampling
    + Enabled (Always On)
+ **Timeout**: Set various options to help with call timeout for missed BYEs.
+ **Max Duration**: Set the maximum amount of time (in seconds) that the call will be allowed to exist before being terminated, typically in the case of a missed BYE.

### Billing
Select a predefined **Package** to determine costs and billing. This will decrement Frequency Match and Setup Cost against that package for the account. 

### Advanced

+ **Tags**: Add these for informational purposes
+ **P-Asserted-ID**: Either `Remove` the P-Asserted-ID so it doesn't reach the customer or leave it at `Default` so it is preserved. 

### Script Forge
Run a custom script on calls to the DID to performs actions such as route based on time of day or if specific users or numbers are active.

## Bulk Upload
For batches of DIDs, you can use Bulk Upload to add multiple DIDs at one time using a CSV (comma-separated values) file which is then mapped to the correct values in Control Panel during the upload process. This can be performed for individual Customer (**Management :material-menu-right: Customer :material-menu-right: [Customer Name] :material-menu-right: DID**) or Globally (**Global :material-menu-right: DID**).  

!!! Caution "CSV files ONLY"
    Use only a CSV file to upload DID numbers. If you upload a regular spreadsheet or another file, the Control Panel becomes unresponsive and you must log out and log in to use the Control Panel. 

Step 1: Create the CSV

1. In Microsoft Excel, open a new workbook and save it as a CSV (Comma delimited) file. 
2. In the first row, add the names of the input fields as column headers. In step 2, you will have a chance to map these fields to the exact fields in ConnexCS, so these don't need to be exact.
3. From the second row on, add the values of the input fields, one row per DID.

!!! tip "Tips for creating the CSV file"
    There are several steps you can take to ensure that the next step goes smoothly:
    
        + The CSV file must contain only one sheet.
        + Include as many fields as you can when creating your columns to leverage the benefits of the bulk upload feature. 
        + Note the number of first and last rows, as these will be the range (minimum and maximum) values in Step 2. 
        + Input fields that correlate to drop-down lists: The entered value must match an existing entry (the Control Panel does not create values from drop-down lists on-the-fly). Ex: "Retain Display Name" only takes Enabled or Disabled; any other value will be rejected. 
        + Input fields that are pre-created objects (ex: customer names and customer card names): You can enter "dummy" values because you must associate the corresponding cell with the input value to the actual value (name of the pre-defined object) before you upload the DID numbers to the server.
        + Input fields that use numerical or free-text values: Enter the permissible range of values.
	+ Input fields that accept values on-the-fly (ex: tags): Enter any meaningful value.
	+ Do not include input fields such as check boxes. You must manually select or clear a check box after you upload the DID number to the server.
	+ Do not include a DID number that already exists on the Control Panel. The entre DID Bulk Upload will fail if Control Panel finds at least one identical DID number.

Step 2: Upload the CSV to ConnexCS

1. Click the Bulk Upload button.
2. Click Upload and select the CSV file (created in previous step).
3. The DID page displays the values in the CSV file.
4. Associate the input fields to the column headers in the CSV file.
    + Right-click the top row of data and select "Set Start Row".
    + Right-click any value in the DID column and click "Map Column" > "DID".
    + If the rest of the input fields match the Control Panel column headers, then you can upload the DID numbers to the server. If not, the rest of the columns should be mapped by right-clicking then selecting the corresponding headers in "Map Column". 
    + (Optional) If you want to change a value in a column that represents a drop-down list, click the cell and enter an different value in the drop-down list. 
    + (Optional) If you want to associate an input value in a column that represents a pre-created object such as the name of a customer, right-click the cell and click Map Column > [name of the input field].
    + (Optional) If you want to change a value in a column that accepts free-text or numerical values, click the cell and enter a different value in the drop-down list. 
    + (Optional) Change values for all cells in the columns that represent pre-created objects, drop-down lists, or accept free-text or numerical values, to reduce your operational time to fine-tune the DID numbers' input fields manually one-by-one, later.
7. Click Upload to Server, confirm the pop-up.
8. At this point, the DIDs and associated values are uploaded to the server. If there are any duplicate DIDs in the system, the entire operation will fail. The Control Panel does not have the ability to indicate which DID is the duplicate, so you will need to review the DIDs independently. 


See [**Script Forge**](https://docs.connexcs.com/developers/scriptforge/) for more information. 


