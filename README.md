**Deploy Global Secure Access Client**

This project demonstrates the deployment process for the Microsoft Global Secure Access (GSA) Client, a core component of Microsoft's Secure Service Edge (SSE) architecture. The client enables identity-aware access to internal (Private Access) and internet-based (Internet Access) resources, enforcing Conditional Access policies and network micro-segmentation.

**Scenario**
A hybrid workforce requires secure access to internal line-of-business (LOB) apps and SaaS services without relying on traditional VPN infrastructure. This project simulates the configuration and deployment of the GSA Client to enable seamless and policy-governed access.

**Key Actions**
• Review GSA client use cases and endpoint requirements
• Simulate client installation and posture validation
• Align deployment with Microsoft Entra Conditional Access architecture
• Reinforce terminology such as Private Access, Traffic Forwarding Profiles, and Connectivity Points

**Learning Objectives**
• Understand the role of the GSA Client in Microsoft's modern perimeter strategy
• Clarify semantic distinctions between GSA, Private Access, and Internet Access
• Map deployment actions to the Entra Control Stack for identity governance alignment

**Entra Control Stack Layers Touched**

• Layer 1 – Authority Definition
✅ Touched: Deployment required directory-level privileges to enable Global Secure Access (preview) and download the client. Actions were conducted with elevated permissions and are audit-eligible.

• Layer 2 – Scope Boundaries
⚠️ Initiated: While Traffic Forwarding Profiles were created, true scoping via identity-based rules or conditional access was not implemented in this project.

• Layer 3 – Test Identity Validation
✅ Partially Confirmed: The GSA client was installed and authenticated as a test user. Full enforcement logic (e.g., denial under misalignment) was not tested but is architecturally supported.

• Layer 4 – External Entry Controls
❌ Not Applied: No B2B, guest, or partner access scenarios were configured or evaluated.

• Layer 5 – Privilege Channels
⚠️ Referenced but Not Formalized: While deployment leveraged privileged access, no structured role delegation or scoped administration was designed or tested.

• Layer 6 – Device Trust Enforcement
❌ Not Activated: No Conditional Access policies tied to device posture, compliance, or trust were implemented.

• Layer 7 – Continuous Verification
❌ Not Integrated: Defender integration, traffic analytics, and risk-informed policies were not tested or reviewed.
