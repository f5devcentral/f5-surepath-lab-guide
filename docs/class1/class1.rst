Class 1 - F5 AI Security - Surepath.ai READ ONLY
################################################

Lab Maintainers:

  Matthieu Dierick <m.dierick@f5.com>

|

In this class, you will learn how to use the F5 Surepath.ai solution. Everything is pre-configured, so you can easily explore and learn about all of Surepath.ai's capabilities:

* Interception
* Detection
* Masking
* Blocking
* Control
* Reporting

SurePath AI is a network-level governance platform that enables safe, compliant, and high‑velocity adoption of Generative AI (GenAI) across the enterprise. 
Rather than blocking public AI outright or relying only on coarse WAAP controls, SurePath AI intercepts GenAI traffic, applies fine‑grained policy (access control, content controls, and PII detection), and provides an auditable record of all workforce AI use. 
The result is accelerated AI productivity with reduced risk of data exposure, policy violations, and shadow AI.

----

How it works
------------
Policy model
^^^^^^^^^^^^
SurePath AI applies least-privilege. The Default Policy sets your baseline for everyone. Group Policies are additive, granting access to additional public services, private models, data sources, or exceptions to sensitive-data handling for specific user populations. 
Within policy you configure public service access using the Public Service Catalog (our curated list of GenAI destinations); 
sensitive-data handling through Content Controls (rules that detect risky content such as harmful content, code, prompt injection, and confidential data) and PII Detection (entity-based detection for personal data) with actions such as Monitor, Warn, Tag, Mask, Delete, Synthesize, or Block. 
Policies also control access to private portal resources including models, Data Sources, and Assistants.

Controls and end-user experience
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Content Controls detect high-risk requests, confidential data, harmful content, prompt injection, and code. Depending on policy, users may see a contextual warning, have elements redacted or synthesized, or be blocked where allowed. 
PII Detection applies a global action to enabled entities for consistent handling of personal data. Most organizations begin with non-blocking warnings and progress to stronger actions for higher-risk groups.

How traffic reaches SurePath AI
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Only GenAI destinations are diverted to SurePath AI; all other web traffic follows its normal path. 
In the preferred model, your SASE platform performs TLS interception and forwards GenAI traffic to SurePath AI using a vendor-specific forward proxy chaining concept (often called forward-to-proxy), optionally adding an X-Authenticated-User header for seamless identity. 
Alternatively, endpoints can use a Proxy PAC URL (a browser/network auto-config file) to send only GenAI domains to the SurePath AI TLS proxy, or SASE can forward without upstream TLS interception when endpoints trust the SurePath AI Root CA (our certificate authority). 
The private portal is always accessed directly and is governed by portal policy and RBAC.

----

F5 AI Security - Surepath.ai Architecture
-----------------------------------------

High-level architectural overview showing traffic interception, policy enforcement, and platform components. Visual reference diagram for system architecture.

.. image:: /pictures/archi.png

----

**Class 1 - All modules**

.. toctree::
   :maxdepth: 1
   :glob:

   module*/module*
