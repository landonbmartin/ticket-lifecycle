<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>Ticket Lifecycle Stages</h2>
<ol>
  <li>Intake</li>
  <li>Assignment & Communication</li>
  <li>Working the Issue</li>
  <li>Resolution</li>

<h2>Lifecycle Stages</h2>

<!-- <img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/> -->

<h3>Intake</h3>

<p>
  <ul>
    <li>From the <b>End User's</b> side (Karen Karen), they create a ticket through osTicket's local host site and fill their information, select a Help Topic</li>
    <ul>
</br>
      <img width="700" alt="Open a New Ticket" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/f9a135ed-e342-4eb0-b68b-ffa242fc6bde">
    </ul>
</br>
    <li>The End User then writes ticket through the <b>Issue Summary</b> and adds a subject and details of the ticket much similar to writing an email</li>
    <ul>
      <li>In this example, Karen creates the ticket under the Help Topic of a Business Critcal Outage (made from our configuration of osTicket) explaining the mobile banking application is suffering a 404 error</li>
</br>
      <img width="700" alt="Mobile Banking Example" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/b859a818-4732-4086-92bb-201380faa35c">
    </ul>
</br>
    <li>Karen then creates the ticket and is sent to <b>Agent</b> Jane Doe who views it from the local help desk login</a></li>
    <ul>
      <li><b>Note</b>: Priorities have not been set for other incoming tickets such as ticket #980890 where end user Ken is requesting an upgrade to Adobe Reader. SLA plans need to be set for these tickets hence why they are all under the priority state of "Normal"</li>
</br>
      <img width="800" alt="View all tickets - Priority Normal" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/02c5be75-7acd-48fb-b4db-dc4ce1773e74">
    </ul>
</br>
  </ul>
</p>

<h3>Assignment & Communication</h3>

<p>
  <ul>
    <li>The Business Critical Outage ticket by Karen numbered #699069 is assigned to the Agent Jane Doe. From Jane's perspective, this is how the ticket first looks.</li>
    <ul>
</br>
      <img width="700" alt="Jane Assigned Ticket" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/e27a5c72-cc9d-4df1-a34a-551796277fc1">
    </ul>
</br>
    <li>By going to the link next to <b>Priority</b>, you are able to set the priority of the ticket to Low, Normal, High, or Emergency</li>
    <ul>
</br>
      <img width="600" alt="Ticket Priority Level" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/06e9df51-6ecb-4d0b-9755-7da088bf3c75">
    </ul>
</br>
    <li>By going to the greyed out link --Unassigned-- next to <b>Assigned to</b>, you can assign the ticket to a Team or Agents. Note if we were to assign it to an Agent outside of Agent Jane's Department, it will not appear in their feed.</li>
    <ul>
</br>
      <img width="600" alt="Ticket Assigning" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/5b001f9d-1b48-45c0-b568-39caf70d728f">
    </ul>
</br>
    <li>By going to the link next to <b>SLA Plan</b> to set the SLA Plan from Default SLA to one our SLA Plans we have created in configuration. For this Business Critical Outage ticket, it'll be set to SEV-A</li>
    <ul>
</br>
      <img width="600" alt="Ticket SLA" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/ad058ce8-f439-487c-a3ab-d86713f0d7d6">
    </ul>
</br>
    <li>By going to the link next to <b>Department</b> to set the Department. For this Business Critical Outage ticket, it'll be set from Support to System Administrators</li>
    <ul>
</br>
      <img width="600" alt="Ticket Department" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/69e20dc5-7144-4d3b-ab10-af53e5a6634d">
    </ul>
</br>
    <li>The Ticket Thread is updated when we make the changes to ticket</li>
    <ul>
</br>
      <img width="800" alt="Ticket Thread" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/5ef884e1-d96b-46ba-b997-5afbb76fe175">
    </ul>
</br>
    <li>The Agent can message the End User through the Ticket Thread to update the User on the ticket as well as set the status of the ticket (which is left as <b>Open</b> since we need to work it out)</li>
    <ul>
</br>
      <img width="800" alt="Ticket Message Reply" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/568b4ce0-5534-4ea8-b4ea-71d9be4c5b0f">
    </ul>
</br>
  </ul>
</p>

<br />

<h3>Working the Issue and Resolution</h3>

<p>
  <ul>
    <li>Following from our Assignment of Departments and Communication with the End User, the issue in our hypothetical Critical Banking Outage ticket has been resolved thanks to System Engineering. The Agent should now communicate the issue with the End User using the Ticket Thread and set the status of the ticket from Open to <b>Resolved</b>. Upon posting the Reply, the ticket is <b>Closed</b>.</li>
    <ul>
</br>
      <img width="800" alt="Ticket Resolved" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/12d8d74b-bdb6-4c9f-83a8-092778bf4934">
    </ul>
</br>
    <li>Closed tickets can be found under the Closed section in our Tickets tab, where information and status of the tickets are archived. It is good practice for Agents to study Closed tickets to improve their experience in working with them</li>
    <ul>
</br>
      <img width="800" alt="Ticket Closed" src="https://github.com/landonbmartin/ticket-lifecycle/assets/148168629/03451e05-8e50-4cd7-b53b-c37d8d3024af">
    </ul>
</br>
  </ul>
  
</p>

<br />
