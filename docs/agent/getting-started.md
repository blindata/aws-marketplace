---
layout: default
title: Getting started
parent: Blindata Agent
nav_order: 3

---
# Set-up Agent

<div style="display: flex; flex-direction: row-reverse; align-items: flex-start;">
    <div style="flex-grow: 2; margin-right: 1.5em;">
        <p>
        Blindata Agent must be able to communicate with all external systems for which you want to automate the activities of metadata collection and data quality monitoring as well as with the main Blindata instance. Therefore, it will be necessary to set-up the machine where the Agent is installed with the appropriate network configurations.
        </p>
    </div>
</div>


# Configurations


<div style="display: flex; flex-direction: row-reverse; align-items: flex-start;">
    <div style="flex-grow: 2; margin-right: 1.5em;">
        <p>
        The installation of the Blindata Agent must be perfected with the following configurations:
        </p>
        <ol>
            <li><b>Datasource URL</b>: the connection string to the database</li>
            <li><b>Datasource username</b>:the username of the user that can interacat with the database for the creation of schemas and tables for creation, modification and deletion of data. Make sure that the user has the right permissions</li>
            <li><b>Datasource password</b>: the password of the user with which the agent will interact with the database</li>
            <li><b>Remote base URL</b>: Used in the CORS configuration, it indicates the URL from which requests are accepted. If not specified, the remote base URL is used as default. It is the url accessed from the browser interface, for example https://blindata.mydomain.com.</li>
            <li><b>Encryption secret</b>: String of 32 characters that will be used by the encryption algorithm of the credentials of the connections stores by the agent  
            </li>
        </ol>
         <p>
        The Blindata Agent agent connection is http, see related pages below to enable https connection
        </p>
    </div>
</div>


# Start Agent

<div style="display: flex; flex-direction: row-reverse; align-items: flex-start;">
    <div style="flex-grow: 2; margin-right: 1.5em;">
        <p> 
        The agent is started with the following command:
        </p>
        <p>
        java -Dloader.path=path/to/blindata-agent/lib/
        -jar blindata-agent-"VERSION".jar
        --spring.datasource.url=jdbc:postgresql://"host":"port"/postgres
        --spring.datasource.username=postgresql
        --spring.datasource.password=password
        --blindata.agent.remote.base-url=https://blindata.mydomain.com
        --blindata.agent.remote.allowed-origin=https://allowed-origin.mydomain.com
        --blindata.agent.encryption.secret=#encryption key
        </p>
        <p>The -Dloader.path option must be specified only if the agent must use custom drivers to connect to external systems. If there is no need to use custom drivers, the option can be omitted.</p>
        <p>Alternatively you can modify the file application.properties located in the same folder as the jar file with the previous commands.</p>
    </div>
</div>


**Related pages:**

- [Enable https connection]({{ site.baseurl }}{% link docs/administration/https.md %})
