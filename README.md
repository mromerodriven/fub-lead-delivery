<p align="center">
<img src="https://i.imgur.com/oPA6CqN.png" height="80%" width="80%"/>
</p>

<h1>Lead Delivery Speed Boost Thru Automation</h1>
In this tutorial, we walk through the steps I took to speed up the lead delivery process using FUB, Slack, and Zapier. <br />

<h2>Environments and Technologies Used</h2>

- Follow Up Boss
- Slack Communication App
- Zapier Automations

<h2>High-Level Steps</h2>

- Step 1: Create the rules for lead delivery within your organization
- Step 2: Create the custom fields and tags in FUB
- Step 3: Have a dedicated channel in Slack for lead delivery
- Step 4: Create the automation in Zapier

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/ruRuNWL.jpg" height="80%" width="80%"/>
</p>
<p>
The rules were simple. The leads were delivered round-robin. The recipient had 2 minutes to claim the lead. Anyone was free to claim "NEXT" on a lead that wasn't theirs incase the recipient missed the window or passed on the lead. That's it. The next lead went to the next person.
</p>
<br />

<p>
<img src="https://i.imgur.com/74z8Df1.png" height="80%" width="80%"/>
</p>
<p>
In the admin account, you'll want to create three custom fields for your ISA's. We'll use these fields to auto-populate Slack when delivering a lead. 
</p>
<br />

<p>
<img src="https://i.imgur.com/W0av9Yw.png" height="80%" width="80%"/>
</p>
<p>
<img src="https://i.imgur.com/ESSterq.png" height="80%" width="80%"/>
</p>
<p>
Next, you'll need to create your trigger tags that Zapier will pick up to know when to deliver the lead.
</p>
<br />

<p>
<img src="https://i.imgur.com/h1lO8Ek.png" height="80%" width="80%"/>
</p>
<p>
Create a dedicated Slack Channel for your lead deliveries.
</p>
<br />

<p>
<img src="https://i.imgur.com/K8uxHCz.png" height="80%" width="80%"/>
</p>
<p>
In Zapier, you'll want to create your automation flow. The first trigger will be "ISA lead available NAME". This is going to pull the ISA notes from the Custom Fields we created in earlier steps, and will post to Slack with a link back to the file. I have this setup to pick up whichever ISA is the one that is creating the lead notification.
</p>
<br />

<p>
<img src="https://i.imgur.com/iRl1KdO.png" height="80%" width="80%"/>
</p>
<p>
I duplicated this path rule for each ISA that we had on the team.
</p>
<br />

<p>
<img src="https://i.imgur.com/3vMSJ6f.png" height="80%" width="80%"/>
</p>
<p>
For each Slack message, this was the template. The UID for the corresponding agent could be found in Slack (that is, the part that starts with @U*****PZ). Once you've created this, it's just a matter of duplicating this for each agent on the team. <br>
<br>
This completes the first part of the lead notification process. <br>
  <br>
The second part is when the agent claims the lead, the ISA assigns the lead to agent using another tag that will add them as a collaborator. 
</p>
<br />

<p>
<img src="https://i.imgur.com/vOGd7G9.png" height="80%" width="80%"/>
</p>
<p>
This automation is triggered by the tag "ISA ASSIGNED TO NAME". Same rules apply to the path to determine the ISA that is initiating the assignment of the lead.
</p>
<br />

<p>
<img src="https://i.imgur.com/9hyN9ZX.png" height="80%" width="80%"/>
</p>
<p>
The message in Slack is a little different. Just enough to indicate to whom the lead has been assigned to.
</p>
<br />

<p>
<img src="https://i.imgur.com/cejCfyV.png" height="80%" width="80%"/>
</p>
<p>
One other step I add here is to automate the process of adding the agent as a collaborator to the file.
</p>
<br />

<p>
<img src="https://i.imgur.com/e7c01i2.png" height="80%" width="80%"/>
</p>
<p>
ALL DONE! You should have a system that outputs similar to this. This has saved this organization a tremendous amount of time.
</p>
<br />

