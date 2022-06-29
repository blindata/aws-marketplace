---
layout: default
title: Pairing Agent with Blindata Core
parent: Agent
nav_order: 3
last_modified_date: 2021-02-26T16:12
---

# Pairing with Blindata Core

---

<div style="display: flex; flex-direction: row-reverse; align-items: flex-start;">
   
    <div style="flex-grow: 2; margin-right: 1.5em;">
        <p>Once the  Agent has been installed, it must be associated with the Blindata tenant with which you want to use it. This procedure is called pairing and is used to:</p>
        <ol>
            <li>Allow the agent to provision the database schema that will contain the data of the tenant with which you are pairing</li>
            <li>Allow the exchange of identifiers for the identification of the tenant</li>
            <li>Test the reachability at the network level; the agent must be able to invoke the Armored API in order to complete the operation.</li>
        </ol>
    </div>
</div>


## Pairing procedure from Blindata Core

  <div style="flex-grow: 2; margin-right: 1.5em;">
        <p>
In Settings> Agent section in Blindata Core, you will find the registry of all the agents installed for a specific tenant. The first step of the procedure is to create an agent by specifying:</p>
        <ol>
            <li>
agent name: this name will be used to identify the agent within the platform</li>
            <li>Agent URL: URL through which the browser can interact with the agent (in this case the public address given by Aws)
</li>
        </ol>
        <div style="display: flex; flex-direction: column; align-items: center;">
    <img src="{{site.baseurl}}/assets/images/CreateAgent.png" style="width: 1000px;">
   
</div>
    </div>



---
