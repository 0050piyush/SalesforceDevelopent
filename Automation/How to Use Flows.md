# Flow Users
Different types of users deploy flows in a variety of ways. Here are what each type of user will commonly do to deploy flows.

**Administrators:**
- Use a custom button or link, custom action, standard Lightning Component, or Utility Item to deploy flows
- Use processes to start Flows
- See real time details of what the flow does by using Debug log
- Use the flow fault email to troubleshoot flows

**Developers:**
- Deploy flows by creating Lightning pages or Visualforce pages.

**Users:**
- Run flows provided that they have the ‘Run Flows’ permission
 

# Flow Capabilities
## Main Flow Types
There are two main types of flow in Flow Builder which are described briefly below.

**SCREEN-BASED:** screen-based flow is basically a flow that uses the screen element that is used to capture or display information. It can be launched from a button, link, page, and more.

**AUTOLAUNCHED:** An autolaunched flow runs in the background while performing its actions. It can be triggered from a record change, process, Apex, platform event,schedule, etc.


## Capabilities of Flow Builder
The following describes some of the functional capabilities and features of flows in order to determine the scenarios where and when they can be used.

**RECORD CHANGE:** Run a flow when a record is created, updated, or deleted. A record criteria can be defined to run the flow conditionally. For create or update triggers, the flow can be set to run every time if the record matches a criteria, or only once when the record is updated to meet the criteria. 

**RUN ON SCHEDULE:** Configure a flow to run on scheduled timings to automate daily or weekly tasks.

**SUBSCRIBE TO EVENT:** Subscribe to a platform event and automatically run when an event message is received. 

**DECIDE CONDITIONALLY:** Execute a decision outcome in record-triggered flows using one of two options: 

- if the condition requirements are met

- or only if the record that triggered the flow to run is updated to meet the condition requirements.

**SYSTEM CONTEXT W/ SHARING:** Run in system context with sharing, which ignores object and field-level security of the current user.

**SYSTEM CONTEXT W/O SHARING:** Run in system context without sharing, which also ignores org-wide default settings, role hierarchies, sharing rules, manual sharing, teams, and territories.

**SYSTEM OR USER CONTEXT:** Run the flow in either system or user context depending on how the flow is launched.

**PERFORM ACTIONS:** Perform Actions such as quick actions, email alerts, or submit approval requests.

**SELECT RETURN FIELDS:** Choose to select all fields or specify certain fields only to return when querying records using the Get Records element.

**ACCESS EXTERNAL DATA:** Look up, create, or update data stored in an external system.

**ACCESS RECORDS:** Query, create, update, and delete records

**RESET PASSWORD:** The Reset Password flow walks agents through the customer password reset experience.

**VERIFY IDENTITY:** The Verify Identity flow helps agents resolve cases of missing credentials.


## Flow Builder Layout Types
There are two types of layout in Flow Builder. 
The layout type only determines how elements are added and visually aligned and connected on the canvas and does not have any impact on flow behavior.

**AUTO LAYOUT:** This is the default layout in Flow Builder. In this layout, elements are automatically aligned, spaced, and fixed. To add elements on the canvas, plus (+) buttons are provided along the flow paths.

**FREEFORM:** In this layout, the elements are available in the Elements tab of the Toolbox pane. To add elements, they are dragged-and-dropped onto the canvas. Alignments and spacings are manually adjusted to give full control on how the elements and connections are positioned on the canvas.


## Flow Building Blocks
When building a flow in Flow Builder, a combination of the following tools are used.

**RESOURCES:** Resources are containers for holding data values – like input obtained from the user, data queried from Salesforce, a global constant, calculated field, etc.

**ELEMENTS:** Elements are what define the behavior of the flow. These are building blocks for defining the various actions that need to be taken at each step. For example, Screen, Create Records, Get Records, Apex Action, etc.

**CONNECTORS:**  Connectors are the paths defined between the various elements that represent the order of execution.

**START ELEMENT:** The ‘Start’ element marks the beginning of a flow. When a new flow is created, it is added automatically.

**FAULT PATH:** Flow also supports error handling. Fault paths can be added to elements that can fail. For example, an ‘Update Records’ element which can fail can be linked with a core action that sends an email using a ‘fault’ connector.


## Flow Use Cases
### Example Use Cases for Screen Flows

**GATHER FEEDBACK:** Create and use a survey form for gathering customer feedback.

**MANAGE LEADS:** Capture and categorize leads based on incoming inquiry calls.

**SET UP APPOINTMENTS:** Schedule an appointment with a customer using the Date/Time screen field type.

**REFRESH ZIP CODE:** Refresh the zip code on a screen in a flow when a user revisits the screen after navigating to the previous screen.

**CUSTOMER SUPPORT:** Use a guided process with screen flows to streamline handling of customer support issues.

**SHARE RECORDS:** A share record can be created to automatically share a lead to a group or user based on record data.


### Example Use Cases for Record-Triggered Flows

**ADD LINE ITEMS:** Add opportunity line items dynamically based on opportunity data and other related records.

**RELAY CASE UPDATES:** Automatically create a record of a custom object and send an email when a case is updated.

**SEND EMAIL LATER:** Automatically send an email at a dynamically scheduled time using a scheduled path in a record-triggered flow.

**AGGREGATE FIELDS:** Update a “Count” field on the parent record when a child record is deleted.


### Example Use Cases for  Platform Event-Triggered Flows

**UPDATE STATUS:** Automatically update a record when a platform event is received such as the shipping status of an order.

**CREATE INVOICE:** An invoice record can be created based on a published event from an integrated external platform after a successful off-site purchase.

**REGISTRATION:** Create a “registrant” record in Salesforce using details from a registration form submitted from a website.

**NEWS FEED:** Subscribe to and receive latest news or alerts from a news feed.


### Example Use Cases for Schedule-Triggered Flows

**SEND GREETINGS:** Automate sending of greetings to contacts who are celebrating their birthdays.

**EXPIRY DATES:** Send tiered reminder emails two weeks and one week before a contract expires.

**TRACK PROGRESS:** Notify manager when no progress is detected in an opportunity for ten days.

**ASSIGN RECORDS:** Assign a lead to another owner if it has not been opened by the current owner three days after it has been assigned.

**MAINTENANCE:** Delete “Log” records that are older than three years at the start of each month.


### Example Use Cases for Autolaunched Flows

**SCHEDULED ACTIONS:** Create an Email Message based on an email template once a scheduled email alert is run.

**INVOKE FROM APEX:** Programmatically invoke a flow that is used to share a record.

**CHANGE OWNERS:** Transfer all accounts of one user to another on the click of a custom button.

**EXTEND PROCESS:** Call a flow that creates multiple tasks in an invoked process based on opportunity stage.



























