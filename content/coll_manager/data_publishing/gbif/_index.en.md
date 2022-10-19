---
title: "Publishing Data to GBIF"
authors: ["Ed Gilbert","Katie Pearson"]
editors: ["Katie Pearson"]
date: 2021-10-07
weight: 50
keywords: ["aggregator","gbif","data publishing"]
---

{{< notice info >}}
  This document describes how to publish the data from your collection to global aggregator [GBIF](https://www.gbif.org).
{{</ notice >}}

Collections managed as "live datasets" within a Symbiota portal can immediately publish to GBIF without issues. Collections that make use of an in-house management system (e.g. Specify, Ke-Emu, etc.) and only publish a snapshot of their data to a Symbiota instance can also use the portal to publish their data to GBIF, but only if: 1) they are not publishing their data through another means (e.g. IPT installation, VertNet, etc.), and 2) an occurrenceID GUID is included in the data being pushed from their in-house database to the Symbiota dataset. If the collection is using the Symbiota publishing tool built into Specify, the occurrenceID GUID will be automatically included in the data upload from Specify. 

{{< notice note >}}
  Your portal must be set up as a GBIF Publishing Installation to publishing your data to GBIF. This can be done by your portal manager.
{{</ notice >}}

1. [Use these instructions](https://biokic.github.io/symbiota-docs/coll_manager/data_publishing/endorsement/) to set up an institutional account with GBIF so that there is a direct publishing agreement established between GBIF and the institution. Since the institutional account may be used to list multiple collection datasets associated with that institution (e.g. https://www.gbif.org/publisher/4c0e9f60-c489-11d8-bf60-b8a03c50a862 ), you should coordinate with other collections within your institution, if applicable. Note that the institutional datasets can be published to GBIF using different publishing resources. For instance, the zoological collections could import their data from VertNet IPT (http://ipt.vertnet.org) or their institutional IPT, vascular plant data from the SEINet https://swbiodiversity.org, and lichens from CNALH (https://lichenportal.org).
   * If you are sure your institution is not yet registered, complete the registration form and follow the instructions provided by GBIF. 
   * If your institution is already registered, review the GBIF metadata for your organization and existing datasets and contact GBIF to make any necessary changes. Be sure that none of the existing datasets contain the same data you are trying to publish. If they do, make the appropriate arrangements with GBIF so that the old dataset can be archived BEFORE re-publishing the new dataset.
2. Login to your Symbiota portal, go to your Administrator Control Panel (via My Profile => Specimen Management tab => click your collection name), and click on "Edit Metadata and Contact Information" link in the Administration Control Panel. Verify your collection name and description (these will be used within the GBIF page), check the GBIF box to the right of "Publish to Aggregators", and click the "Save Edits" button. If you do not see a GBIF publishing checkbox, contact your portal manager and ask them to configure the portal for GBIF publishing.  
3. Return to the Administrator Contol Panel and click on the "Darwin Core Archive Publishing" link in the Administration Control Panel. Click "Create/Refresh Darwin Core Archive" button to package up your data within a Darwin Core Archive data package. 
4. Enter your institution's GBIF publication key and click the Validate Key button. If you key validates, more instructions will be displayed along with a Submit Data button. The GBIF Publisher Key should have the following format: xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx (e.g. 4c0e9f60-c489-11d8-bf60-b8a03c50a872). You can also enter the full URL to your GBIF publishing page, and the key will be automatically extracted. 
5. Before you can submit data, you will need to contact GBIF help desk (helpdesk@gbif.org) and request for the portal's GBIF user account to be given permission to create and update datasets within your institution's publishing instance. The GBIF username associated with the Symbiota portal installation is displayed in paragraph above the Submit Data button. Click on the GBIF email address to automatically generate a message within your email client.
6. Once you hear back from GBIF affirming that the portal has permission to submit data to your publisher, click the Submit Data button. A link to your GBIF dataset will be immediately displayed, though it may take an hour or so for your data to be loaded, indexed, and available.

{{< youtube aDbw9RF4w08 >}}
