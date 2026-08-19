Check and learn from the user activity logs
===========================================

* In Chrome, click on Surepath Admin Portal - No Login required, SSO done
* On the left menu, click on User Activity. You can see all prompts

You can see all the requests from all the users of this tenant (WW F5ers). 

.. note:: Some requests can have ``Intent`` or other categories to N/A, no worries, this is due to the Powershell script simulating your user identity. Discard them.

.. image:: ../../pictures/user-activity.png

* Select one prompt, and click on the right arrow, to pop out the new window with the details

.. image:: ../../pictures/right-arrow.png
   :alt: Image

* Navigate into the details and check the warning and logs.

.. image:: ../../pictures/event-details-1.png

.. image:: ../../pictures/event-details.png
   :alt: Image

* For the MCP Demo, when you send the prompt with Claude Desktop with the Github MCP server, find the request in the list and click on the details.

You can see a new tab ``Tools``. These are the MCP tools that are running on the MCP server. 

.. image:: ../../pictures/mcp-tool-output.png
   :alt: image

Click on the message to see the tools used with the prompt.

.. image:: ../../pictures/detail-mcp.png
   :alt: image