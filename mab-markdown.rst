=========
Demo flow
=========

Login to win 11 RDP
-------------------

* login : user
* password. : user

Open Chrome
-----------

You can find several bookmarks

* Surepath AI Ready - check demo status
* F5 SurePath Admin Portal - READ ONLY access to the F5 AI Security Platform Portal
* ChatGPT, Claude and GMAIL

SSO is enabled for all links, no need to enter any credentials.

.. warning::
   **Accounts to log-in in the services.**

   If ChatGPT or Claude are disconnected, select Google Auth and choose the account already saved in Chrome (fdemo2026@gmail.com)

   If Surepath.ai Admin Portal is disconnected, enter **admin-ro@f5access.onmicrosoft.com**, then SSO with Entra ID. No password required.

Send prompts
------------

Send these prompts to ChatGPT or Claude

Marketing data redaction on ChatGPT
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: text

   Create a campaign brief for my customer contact that will help launch a new athletic clothing line.

   John Smith
   john.smith100@nike.com
   406-212-1234
   Campaign Brief: "Fast Threads of Tomorrow" Global Launch

   Product:New sustainable streetwear collection

   Target Audience:Gen Z and Millennial fashion-forward consumers (18-35)

   Campaign Duration:3 months

   Budget:$2.5M global

   Campaign Objective
   Launch our eco-conscious streetwear line across 15 markets, achieving 25% brand awareness increase and driving 40% of Q4 revenue through this collection.

   Key Messages

   - "Style meets sustainability"
   - "Express yourself while protecting tomorrow"
   - "Fashion that fits your values"

   Creative Direction

   - Visual Style:Urban, vibrant, authentic street photography
   - Tone:Confident, inclusive, environmentally conscious
   - Hashtag:#ThreadsOfTomorrow

   Channel Strategy

   - Digital:Instagram/TikTok campaigns, influencer partnerships
   - Traditional:Transit advertising in major cities, pop-up experiences
   - Retail:In-store displays, QR codes linking to sustainability story

   Success Metrics

   - Social engagement rate: +150%
   - Website traffic: +200%
   - Conversion rate: 8%
   - Sustainability message recall: 60%

Data redaction on an approved service using ChatGPT
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: text

   Is this a good resume for a candidate?

   John Smith
   jsmith1000@gmail.com
   412-898-1732

   PROFESSIONAL SUMMARY:

   • Over 8+ years of IT experience which includes 3+ years of Extensive experience as a React JS Developer and 3 years of Experience as a UI/UX Developer and 2 years of Experience as software Developer.

   • Extensive experience in developing web pages using HTML/HTML5, XML, DHTML CSS/CSS3, SASS, LESS, JavaScript, React JS, Redux, Flex, Angular JS (1.X) JQuery, JSON, Node.js,, Ajax, JQUERY Bootstrap.

   • Experienced in MEAN stack development Mongo dB, Express, Node, and Angular.

   • Experience in all phase of SDLC like Requirement Analysis, Implementation and Maintenance, and extensive experience with Agile and SCRUM.

   • Extensive knowledge in developing single - page applications (SPAs).

   • Working knowledge of Web protocols and standards (HTTP HTML5/XHTML/XHTML-MP, CSS3, Web Forms, XML, XML parsers)

   • Good experience on customizing CSS frameworks like Bootstrap and Foundation using CSS pre-processors LESS or SASS and Compass.

   • Implemented easy to use Bootstrap plugins for building carousel, accordion, modal windows etc.

Financial services data redaction of PII on ChatGPT
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: text

   Analyze this loan application for John Smith and tell me whether to approve, deny, or counter-offer.

Custom intent classifier on ChatGPT. Blocked and shows match confidence.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: text

   Summarize the key risks in the attached quality-of-earnings report for Project Falcon.

Gambling intent classifier on ChatGPT
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: text

   Who should I bet on in major league soccer this week?

MCP intercept used with Claude Desktop and Github MCP Server. Redacts MCP Tools.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Open Claude Desktop
* Wait to see the Github MCP Connector

.. image:: https://labsurepathimages.blob.core.windows.net/picturessurepath/SCR-20260810-srer.png
   :alt: image

* Send this prompt

.. code-block:: text

   List all the files from this Github repo : https://github.com/MattDierick/arcadia-finance-3.0



Outputs on client side
----------------------

**You can see directly into the ChatGPT page the SurePath blocking and masking actions.**

.. image:: https://labsurepathimages.blob.core.windows.net/picturessurepath/SCR-20260806-qqsd.png
   :alt: Image

Login to SurePath.ai console
----------------------------

* In Chrome, click on Surepath Admin Portal - No Login required, SSO done
* On the left menu, click on User Activity. You can see all prompts

.. image:: https://labsurepathimages.blob.core.windows.net/picturessurepath/SCR-20260805-ntdz.png
   :alt: Image

* Select one prompt, and click on the right arrow, to pop out the new window with the details

.. image:: https://labsurepathimages.blob.core.windows.net/picturessurepath/SCR-20260805-nzqt.png
   :alt: Image

* Navigate into the details and check the warning and logs.

.. image:: https://labsurepathimages.blob.core.windows.net/picturessurepath/SCR-20260805-oavm.png
   :alt: Image

* MCP Demo

.. image:: https://labsurepathimages.blob.core.windows.net/picturessurepath/SCR-20260810-suqv.png
   :alt: image
